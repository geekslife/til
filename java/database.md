# Database

## JPA

* [Proxy](https://yellowh.tistory.com/125): 지연 로딩을 위해 영속성 컨텍스트에 없는 엔티티를 EntityManager.getReference()로 호출하면 프락시 객체를 만들어 반환한다.
* [즉시로딩,지연로딩,컬렉션래퍼](https://yellowh.tistory.com/126): XToOne 은 즉시로딩, XToMany 는 지연로딩이 기본. 엔티티가 영속화될 때 컬렉션의 경우 컬렉션 래퍼가 만들어지고, 지연로딩인 경우 실제 컬렉션에서 실제 데이터 조회 시점에 DB 조회 및 초기화를 수행한다.
* [N+1](https://meetup.toast.com/posts/87)
  - Lazy 컬렉션 멤버와 Eager 멤버가 있을 때, 컬렉션을 조회하면 연관된 모든 Eager 멤버에 대해 N번의 조회 쿼리가 발생한다.
  - 해결 방안
    * [Fetch Join](https://yellowh.tistory.com/133) : 연관된 엔티티를 한번에 같이 조회
    * Lazy : XToOne 의 글로벌 페치 전략을 Lazy 로 변경. 영속성 컨텍스트를 벗어나서 시도하면 LazyInitializationException 이 발생하는데, Open Session In View(OSIV)를 적용해서 해결한다.


### [Prepared Statement](https://en.wikipedia.org/wiki/Prepared_statement)
  같거나 유사한 DB 구문이 반복될 때 매우 효율적인 DBMS의 기능 중 하나로.. SQL 구문이 템플릿 형태로 제공되는 형태이다.
  1. Prepare: 쿼리를 템플릿 형태로 생성하고 DB 로 보낸다.
  1. DBMS 는 이러한 구문 템플릿을 컴파일하고 결과를 저장해둔다.
  1. Execute: 애플리케이션이 구문 템플릿의 파라미터에 대한 값을 제공하면, DBMS는 구문을 실행한다.
  구문의 직접 실행대비 장점: 1) 빠르다 2) SQL Injection 에 안전한다
