# Do it! Django
`점프 투 장고`를 보고 공부한 내용을 정리합니다

## Django란?
장고는 웹 프로그램을 쉽고 빠르게 만들어 주는 웹 프레임워크다
* 보안 튼튼
* 다양한 기능 보유

---
### CSRF
CSRF(Cross Site Request Forgery)는 웹 사이트 취약점 공격을 방지하기 위해 사용하는 기술이다  
1. 장고가 CSRF 토큰 값을 세션을 통해 발행
2. 웹 페이지에서 폼 전송시, 해당 토큰을 함께 전송
3. 작성된 데이터가 제대로 전달되는지 검증

**csrf_token을 사용하기 위해서는 CsrfViewMiddleware 미들웨어가 필요한데,  
이 미들웨어는 settings.py의 MIDDLEWARE 항목에 디폴트로 추가되어 있으므로 별도의 설정이 필요 없다

