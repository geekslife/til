# Spring Framework

## Spring MVC

### [@RestController](https://doublesprogramming.tistory.com/105)
  * 기존 MVC 는 DispatcherServlet -> HandlerMapping -> Controller => View 순서로 응답 전송
  * @Controller 메서드에 @ResponseBody 를 지정하면 바로 응답 전송
  * Spring 4 부터 @Controller + @ResponseBody = @RestController 제공함으로써 API 작성이 보다 간편해짐
