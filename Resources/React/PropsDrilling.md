# Props Drilling 이란 무엇인가요?

### props
- 상위 컴포넌트에서 하위 컴포넌트로 값을 전달할 때 사용하는 속성

### props drilling
- props를 오로지 하위 컴포넌트로 전달하기 위한 컴포넌트들을 거치며 props를 전달하는 과정

### 문제점
props drilling의 규모가 커질수록
- 코드의 가독성이 저하
- 유지 보수의 어려움
- 오류 발생시 props의 추적의 어려움
- drilling만을 위한 다른 컴포넌트들도 리렌더링 되어 웹 성능 저하

### 대안
- React의 Context API
- 전역 상태관리 라이브러리 (redux, recoil...)
