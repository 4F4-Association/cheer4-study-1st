# 자바스크립트의 이벤트 버블링에 대해서 설명하세요.
### 1. 이벤트 버블링이란?
이벤트 버블링이란 특정 요소에 이벤트가 발생할 경우 해당 요소의 부모 요소에도 이벤트가 전파되는 현상으로 최상단의 부모 요소(루트)에 도달할 때까지 반복됩니다.
### 2. 이벤트 버블링을 막고 싶다면?
event.stopPropagation()를 사용해 부모 요소에 대한 이벤트 전파를 막을 수 있습니다. 하지만 이벤트 버블링은 각 하위 요소에서 이벤트 핸들러를 각각 세팅하지 않고도 부모 요소에서 이벤트를 인지해 상위 요소 한 곳에서 핸들링을 하기 용이하게 하는 활용점이 존재하므로 이벤트 버블링을 막을 땐 신중하게 생각할 필요가 있습니다.
