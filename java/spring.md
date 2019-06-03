# Spring Framework

## AOP

* [AOP 정리](https://addio3305.tistory.com/86)

## Spring Boot

* [Spring Boot Test](https://meetup.toast.com/posts/124) : Toast Meetup 에서 정리한 Spring Boot 테스트 기능 소개
  - TestRestTemplate : MockMvc 와 달리 Servlet Container 를 생성하므로 클라이언트의 입장에서 테스트를 수행함

## Spring MVC

* [@RestController](https://doublesprogramming.tistory.com/105)
  - 기존 MVC 는 DispatcherServlet -> HandlerMapping -> Controller => View 순서로 응답 전송
  - @Controller 메서드에 @ResponseBody 를 지정하면 바로 응답 전송
  - Spring 4 부터 @Controller + @ResponseBody = @RestController 제공함으로써 API 작성이 보다 간편해짐


## Spring Security

* 
