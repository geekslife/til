#Database

## 이것저것

### [Prepared Statement](https://en.wikipedia.org/wiki/Prepared_statement)
  같거나 유사한 DB 구문이 반복될 때 매우 효율적인 DBMS의 기능 중 하나로.. SQL 구문이 템플릿 형태로 제공되는 형태이다.
  1. Prepare: 쿼리를 템플릿 형태로 생성하고 DB 로 보낸다.
  1. DBMS 는 이러한 구문 템플릿을 컴파일하고 결과를 저장해둔다.
  1. Execute: 애플리케이션이 구문 템플릿의 파라미터에 대한 값을 제공하면, DBMS는 구문을 실행한다.
  구문의 직접 실행대비 장점: 1) 빠르다 2) SQL Injection 에 안전한다
