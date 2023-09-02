# Redux와 Recoil에 대해 설명해주세요.
### Redux
Redux는 오픈 소스 자바스크립트 라이브러리의 일종으로 state를 이용해 웹 또는 앱의 상태 관리를 해 줍니다. Redux에는 3가지 원칙이 존재하는데 `동일한 데이터는 항상 같은 곳에서 가지고 온다`는 `Single source of truth`, `상태를 직접 변경해선 안 된다`는 `State is read-only`, `변경은 순수 함수로만 가능하다`는 `Changes are made with pure functions`가 있습니다. Redux의 구성 요소는 크게 5가지를 언급할 수 있습니다.
* createStore : state를 저장할 store를 생성합니다. store의 내장 함수로는 `dispath`, `getState`, `subscribe`가 있습니다.
* reducer : action을 해결하고 변경된 현재 상태를 반환합니다.
* action : state를 실질적으로 수정하며 항상 객체 타입이어야 하고 type 요소를 필수적으로 갖고 있어야 합니다.
* dispatch : reducer를 불러서 현재 state에 action을 발생시키는 역할을 하는 것으로 간단히 말해 action을 reducer에 전달합니다.
* subscribe : store가 변할 때마다 호출되는 부분으로 dispatch가 실행될 때마다 subscribe에 전달된 함수가 호출됩니다.
### Recoil
Recoil 또한 React 애플리케이션의 상태 관리를 위한 라이브러리입니다. Recoil은 atoms(공유 상태)에서 selectors(순수 함수)를 거쳐 React 컴포넌트로 내려가는 data-flow graph를 만들 수 있습니다. 여기서 atoms는 컴포넌트가 구독할 수 있는 상태의 단위이며, selectors는 atoms 상태 값을 동기 또는 비동기 방식을 통해 변환합니다.
