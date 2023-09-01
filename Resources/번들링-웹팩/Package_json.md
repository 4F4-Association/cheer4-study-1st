# package.json에서 dependencies와 devDependencies의 차이점은 무엇인가요?

## dependencies
애플리케이션 동작과 직접적으로 연관된 라이브러리를 설치하는 곳입니다. 배포할 때 라이브러리가 포함되어 배포됩니다.

## devDependencies
애플리케이션 동작과는 직접적인 연관이 없지만 개발할 때 필요한 라이브러리를 설치하는 곳입니다. 개발에 필요한 라이브러리이기 때문에 배포에 포함되지 않습니다.

## 장점
두 항목을 나눠서 설치하면 devDependencies는 배포에 포함되지 않기 때문에 빌드 시간을 줄일 수 있습니다. eslint, prettier와 같은 라이브러리를 devDependencies에 설치하면 좋습니다.
