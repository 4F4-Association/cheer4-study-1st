# Prototype에 대해 설명해 주세요.
JavaScript의 prototype은 객체 지향 프로그래밍에서의 상속을 가능하게 하는 메커니즘입니다. 프로토타입 객체는 생성자 함수와 동시에 생성되며 이 생성자 함수로 생성한 객체는 이 프로토타입 객체를 ‘[[prototype]]’ 이라는 내부슬롯에 저장합니다. 객체의 속성을 조회할 때 해당 객체에 그 속성이 없다면  ‘[[prototype]]’ 이 가리키는 프로토타입 링크를 따라가 프로토타입 객체의 프로퍼티나 메소드를 차례대로 검색합니다. 이것을 프로토타입 체인이라고 합니다. 프로토 타입에 매서드를 추가하는 방법은 다음과 같습니다.  

***`class`***
```js
class Dog {
    constructor(name) {
        this.name = name;
    }
    
    bark() {
        console.log(`${this.name} says woof`);
    }
}
```
***`생성자 함수`***
```js
function Dog(name) {
    this.name = name;
}

Dog.prototype.bark = function() {
    console.log(`${this.name} says woof`);
};
```

