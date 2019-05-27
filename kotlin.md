### 인터페이스

* property : field + accessor
* kotlin 은 property 를 기본 지원(val:getter, var:getter+setter)한다.
* backing field : accessor 에서 참조하는 필드. 커스텀 getter/setter 구현 시 사용한다.
  * interface 는 상태를 저장하지 않기 때문에 getter/setter 선언할 수는 있으나 backing field 를 사용할 수는 없다.