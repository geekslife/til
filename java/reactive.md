## History

* Reactive Programming 이란 데이터 스트림과 변경의 전파를 다루는 선언적인 프로그래밍 패러다임이다. 
* Akka, Sodium 등의 프레임워크가 등장했으며, MS에서는 에릭 마이어가 .Net용 리액티브 프로그래밍 프레임워크를 reactive extensions(Reactive X, RX) 라는 이름으로 제공했다. 이러한 리액티브 익스텐전은 다수의 언어로 포팅되었다.

[How (not) to use Reactive Streams in Java 9+](https://blog.softwaremill.com/how-not-to-use-reactive-streams-in-java-9-7a39ea9c2cb3)
* upstream(producer)의 속도가 downstream(consumer)보다 빠를 때의 대처 방안
  1. buffer it : 메모리는 금방 동이 날 것이다
  2. drop it : 데이터를 잃는다
  3. block until ... : 전체 파이프라인이 지연된다
  이러한 서로 다른 프로세싱 능력을 다루는 기술을 배압(backpressure)이라 한다.
  