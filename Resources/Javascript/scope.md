# 스코프에 대해서 설명해주세요
### 1. 스코프란?
스코프는 참조 대상 식별자를 찾아내기 위한 규칙으로 식별자를 참조할 수 있는 유효 범위를 의미합니다. 스코프는 유효 범위에 따라 종류를 분류할 수 있습니다.
### 2. 스코프의 종류
* 전역 스코프 : 코드의 어느 곳에서든 참조할 수 있는 범위로 이곳에서 선언된 변수는 <code>전역 변수</code>가 되어 어디에서도 참조가 가능합니다.
* 지역 스코프 : 코드 블록 및 함수 내 범위에 한정되어 현재 위치 및 하위 범위에서만 참조가 가능한 범위입니다. 여기서 선언된 변수는 <code>지역 변수</code>로 현재 위치 및 하위 범위에서만 참조가 가능합니다. 지역 스코프는 크게 두 개로 나눌 수 있으며 코드 블록 내에 한정된 지역 스코프를 <code>블록 레벨 스코프</code>, 함수 내에 한정된 지역 스코프를 <code>함수 레벨 스코프</code>라 합니다.
### 3. 변수 선언자에 따른 차이
<code>var</code>로 선언할 경우에 함수 레벨 스코프를 가지게 되는 반면 <code>let</code>, <code>const</code>는 블록 레벨 스코프를 가지게 됩니다. 이러한 차이로 인해 코드 블록 밖에서도 <code>var</code>로 선언한 변수는 참조가 가능한 경우가 있으므로 사용할 시 유의해야 합니다.
  
  
