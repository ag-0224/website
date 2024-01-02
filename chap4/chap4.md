# 고급 CSS

## Transition

1. Transition은 어떤 상태에서 다른 상태로 가는 변화를 애니메이션화 하는 것이다.
2. transition은 state가 없는 곳에 적용해야한다.
3. state와 style이 적용된 태그 모두 있는 곳에 적용해야한다.
4. all을 기본으로 사용하나 원하는 것만 적용 시키고 싶을 때는 원하는 요소만 적어준다.

## cubic-bezier

1. 애니메이션 속도를 사용자가 지정할 수 있도록 해주는 것이다.

## keyframes

1. 애니메이션을 만들고 싶을 때 @keyframes 함수명{} 으로 작성하고 style이 적용된 태그에 animation: 함수명 이라고 적는다.
2. 단계가 2개일 때는 from to 여러개 일때는 %를 활용한다.

## Media query

1. 오직 css만을 이용해서 스크린의 사이즈를 알 수 있는 방법이다.
2. @media 조건식 {} 을 통해서 선언된다.
3. and를 통해서 조건식을 연결한다.
4. 모바일에서만 작동되는 query들이 존재한다.
