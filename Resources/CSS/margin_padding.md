# margin과 padding의 차이를 설명해 주세요.

html 요소의 content를 감싸는 테두리, 즉 border를 기준으로 margin은 바깥쪽 영역, padding은 안쪽 영역을 의미합니다. 
padding은 border 안쪽의 border와 content 사이의 여백을 나타내는 영역, margin은 border의 바깥의 주변 요소와의 거리를 나타냅니다. 
따라서 margin에 값을 줄 경우 요소 사이의 거리가 멀어지고, 반대로 padding에 값을 주면 border와 content 사이의 거리가 멀어집니다.
margin과 padding은 둘 다 대상이 되는 요소의 display속성이 block 또는 inline-block인 경우에만 적용이 되며, 상우하좌를 하나하나 다 쓰거나 상하 또는 좌우 등으로 축약해서 쓸 수도 있습니다.
그러나 margin에는 음수값과 브라우저가 자체적으로 계산하는 값인 auto가 적용되지만 padding에는 적용되지 않습니다.
또한 padding을 사용할 때는 기본적으로 대상 요소의 기본 너비에 padding값만큼 더해져 요소의 총 너비와 높이가 결정이 됩니다. 만약 대상 요소의 너비 및 높이를 padding에 영향을 받지 않고 설정하고 싶은 경우, 요소의 box-sizing:border-box 속성을 사용하면 됩니다.

 
