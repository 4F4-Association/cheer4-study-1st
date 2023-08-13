# useEffect의 dependency array에 대해서 설명해주세요
### 1. useEffect와 dependency array
<code>useEffect</code>란 컴포넌트 내에서 Side Effect를 실행할 수 있게 하는 Hook입니다. uesEffect는 첫 번째 인자로 콜백 함수를 받고 두 번째 인자로 배열을 받는데 이 배열을 <code>dependency array</code>라고 부릅니다.
### 2. dependency array의 종류에 따른 차이
기본적으로 useEffect가 인자로 받은 콜백 함수는 컴포넌트의 첫 렌더링 시점(마운트)에 실행돼 Side Effect가 발생하며 첫 렌더링 이후에는 dependency array가 어떤 상태인지에 따라 차이가 발생합니다.
* dependency array에 특정 state값이 존재하는 경우 : 특정 state값이 바뀔 때마다 콜백 함수 실행
* dependency array가 빈 배열일 경우 : 컴포넌트의 첫 렌더링 시점에서만 콜백 함수 실행
* dependency array가 존재하지 않는 경우 : 컴포넌트가 렌더링할 때마다 콜백 함수 실행
### 추가 : Side Effect가 무엇인가요?
어떤 함수가 실행됐을 때 해당 함수에 의해 함수 스코프 외부의 값이 변경되는 것을 의미합니다. 함수 내에서 전역 변수의 값을 변경하는 것이 대표적인 예라고 할 수 있습니다.
