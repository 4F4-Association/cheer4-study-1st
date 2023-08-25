# JSX가 무엇인가요?

## JSX
JavaScript XML의 줄임말로 React에서 사용하는 JavaScript 확장 문법입니다. HTML과 유사한 문법을 사용하며, HTML 요소에 JavaScript 객체를 내장하여 작성할 수 있습니다. 브라우저에서 직접 읽을 수 없기 때문에 babel을 사용하여 일반 JavaScript 코드로 변환해주어야 합니다.

## JSX의 특징
- HTML에서 사용하는 속성 대신 camelCase의 속성을 사용합니다. (ex. class -> className, for -> htmlFor)
- 가장 상위에 있는 HTML 태그는 오직 1개여야만 합니다.
- JavaScript는 중괄호 내에 사용해야하며 그 안에는 표현식을 사용합니다.
