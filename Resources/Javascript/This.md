# `this`란 무엇인가요?

this란 현재 실행 중인 코드에서 참조하는 객체를 가리킵니다. 이 값은 실행 컨택스트에 따라 달라집니다. 
보통 함수가 호출되면 보통은 전역 객체인 window를 가리키지만, 클래스 내부의 메서드에서는 new키워드로 생성된 인스턴스를 가리킵니다. 그리고 이벤트 핸들러 내부에서는 해당 이벤트를 발생시킨 DOM요소를 가리킵니다. 또한 화살표 함수는 함수 호출이 아닌 정의할 때의 실행 컨텍스트를 유지합니다.
만약 클래스 내부에 선언한 메서드에 이벤트 핸들러가 있을 경우, 그 함수가 호출되었을 때 this는 DOM요소를 가리킵니다. 때문에 만약 메서드 내부에서 프로퍼티를 사용하기 위하여 this를 DOM요소가 아니라 클래스 인스턴스의 this를 가리키도록 하고 싶을 때는 bind 메서드를 사용할 수 있습니다.