# Promise가 무엇인가요?
### 1. Promise의 정의
Promises는 비동기 처리에서 사용되는 자바스크립트 내장 객체다. 비동기란 앞선 코드의 요청 및 처리가 종료될 때까지 다음 코드의 동작이 멈춰 있지 않고 바로 동작을 실행하는 특징을 의미한다.<br/>만약 서버에서 데이터를 요청하는 코드 뒤에 서버에서 받은 데이터를 화면에 출력하는 코드가 있는 상황에서 비동기에 대한 처리를 해 두지 않으면 서버에서 데이터를 완전히 보내 주기 전에 화면에 출력하는 코드가 실행돼 오류가 발생한다. 이러한 상황을 방지하기 위해 비동기를 동기처럼 실행하게 만드는 처리가 필요하며 이러한 처리의 대표적인 예가 Promise다.
### 2. Promise의 생성
Promise는 <code>new Promise()</code>로 생성할 수 있다. Promise 객체는 두 개의 콜백함수를 인자로 받을 수 있으며 첫 번째 인자 <code>resolve</code>는 Promise가 성공적으로 반환값을 받았을 때 실행되는 콜백함수, 두 번째 인자 <code>reject</code>는 Promise가 실패했을 때 실행되는 콜백함수를 의미한다.
### 3. Promise의 상태 3가지
앞서 설명한 성공적으로 반환값을 받은 경우와 실패했을 경우는 각각 정확한 명칭을 가지고 있다.
1) 대기(pending) : Promise가 생성된 직후의 상태로 이 단계를 벗어나면 이행 또는 거부 둘 중 하나의 상태로 전환된다.
2) 이행(fulfilled) : <code>resolve</code>가 실행된 상태로 Promise가 성공적으로 진행된 상태를 의미한다.
3) 거부(rejected) : <code>reject</code>가 실행된 상태로 Promise 실행에 오류가 발생한 상태를 의미한다.

Promise가 <code>fulfilled</code>인지 <code>rejected</code>인지에 따라 메소드를 이용해 다른 후속 조치를 취할 수 있다. 이 메소드는 체이닝이 가능해 연이어 사용할 수 있다.<br/>
1) <code>then</code> : <code>fulfilled</code>일 때 Promise에서 성공적으로 받아낸 결과값을 도출해내고 추후 동작을 추가할 수 있는 메소드다.
2) <code>catch</code> : 이름 그대로 오류를 잡아내는 메소드로 <code>rejected</code>일 때 추후 동작을 추가할 수 있는 메소드다.
