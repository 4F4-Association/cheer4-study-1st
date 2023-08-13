# CORS에 대해 설명해주세요. 
### 1. CORS란?
CORS(Cross-Origin Resource Sharing)는 교차 출처 리소스 공유를 뜻합니다. 이는 추가 HTTP 헤더를 사용하여, 한 출처에서 실행 중인 웹 애플리케이션이 다른 출처의 선택한 자원에 접근할 수 있는 권한을 부여합니다.
### 2. CORS가 필요한 이유는?
웹 애플리케이션은 리소스가 자신의 출처(도메인, 프로토콜, 포트 번호)와 다를 때 Cross Origin HTTP 요청을 실행하는데 기본적으로 브라우저는 보안적인 이유로 Cross Origin HTTP 요청을 제한합니다. 이때 추가 HTTP 헤더를 이용해 Cross Origin HTTP 요청의 리소스 접근을 선택적으로 가능하게 만드는 매커니즘이 바로 CORS입니다.
