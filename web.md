# Web

## Media

* [Media Capture & Record](https://developers.google.com/web/fundamentals/media/recording-audio/)

## [JSON Web Token(JWT)](https://blog.outsider.ne.kr/1160)

* JSON 기반의 인증 토큰 규격
* JOSE_Header.ClaimSet.Signature 형태로 된 구성
  * JSON Object Signing & Encryption Header: type + algorithm
  * Claim Set: 사용자 정보
  * Signature : <JOSE>.<ClaimSet>을 인코딩한 값
* 일반적인 인증 과정:
  * 로그인시 access token 과 refresh token 을 발급
  * access token 만료시 refresh token 으로 재발급
