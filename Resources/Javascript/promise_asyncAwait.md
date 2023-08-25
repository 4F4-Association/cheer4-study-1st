# `Promise`와 `async/await`의 차이는 무엇인가요?

## `Promise`
JavaScript에서 비동기 처리를 할 때 사용되는 내장 객체입니다. `Promise`가 이행되면 콜백함수인 `resolve`가 호출되고, 거부되면 콜백함수인 `reject`가 호출됩니다. `then()`과 `catch()` 메소드를 사용해 각각 `resolve`, `reject`에 대한 반환값을 얻을 수 있습니다.
```js
const promise = new Promise((resolve, reject) => {
  if (/* 조건문 */) resolve(/* 이행될 때 처리할 내용 */);
  else reject(/* 거부될 때 처리할 내용 */);
}

promise
  .then(res => console.log(res))
  .catch(err => console.log(err));
```

## `async/await`
`callback`과 `Promise`의 단점을 극복하기 위해 비교적 최근에 생긴 비동기 처리 문법입니다. 함수 앞에 `async`라는 예약어를 앞에 붙이고 함수 내부에서 HTTP 통신이 필요한 비동기 처리 코드 앞에 `await`를 붙여 사용합니다. `try-catch` 구문을 사용하여 예외를 처리합니다.
```js
const asynchronous = async () => {
  try {
    const result = await promise();
    console.log(result);
  } catch (err) {
    console.log(err);
  }
}
```
