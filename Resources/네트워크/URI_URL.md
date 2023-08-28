# URI와 URL 차이에 대해 설명해 주세요.
<img width="600" alt="URI-URL-URN_2x" src="https://github.com/4F4-Association/cheer4-study-1st/assets/111393185/eda43a53-d26d-480d-b19f-229e9285715e">

*이미지 출처: [Networking Basics: What’s the Difference Between URI, URL, and URN?](https://www.cbtnuggets.com/blog/technology/networking/networking-basics-whats-the-difference-between-uri-url-and-urn).*

### URI

- Uniform Resource Identifier의 약자이며 논리적 및 물리적 리소스를 식별하는 고유한 문자열 시퀸스
- 주요 표준 서브셋에는 URL과 URN가 있음
- 모든 URL은 URI이지만, 모든 URI가 URL은 아님
- URL과 URN 둘 다 아닌 URI라는 것은 정의상 있을 수 있지만, 실제 웹 표준과 일반적인 사용 사례에서는 거의 존재하지 않음


### URL

- Uniform Resource Locator의 약자이며 리소스의 위치를 가리키는 문자열 
- 특정 리소스의 위치와 해당 리소스에 접근할 수 있는 프로토콜(예: HTTP, FTP)을 지정
- 예: **`http://www.example.com/index.html`**

### URN

- Uniform Resource Name 리소스를 유일하게 식별하기 위한 영구적인 이름을 나타내는 문자열
- 리소스의 실제 위치나 어떻게 접근할 수 있는지와 같은 정보를 포함하지 않음
- URN으로 전환하기 위해서 엄청난 작업량이 필요하고 URL에서 URN으로의 전환이 급한일도 아니기 때문에 거의 사용되지 않고있음
- 예: **`urn:isbn:0451450523`**
