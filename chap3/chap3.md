# CSS 문법 정리

## css 파일을 html 파일에 추가하는 방법

1. link를 통해 외부 파일로 추가할 수 있다.
2. head내에서 style태그를 통해 css를 추가할 수 있다.

## css를 태그에 적용시키는 방법

1. 원하는 태그를 지정하고 원하는 속성값을 사용하면 된다.
2. 속성이 겹치는 경우 마지막으로 선언된 속성이 적용된다. (브라우저는 위에서 아래로 순차적으로 읽기 때문이다.)
3. 속성 이름은 공백과 \_을 허용하지 않는다. -를 사용하도록 하자.

## margin

1. margin은 box의 border로부터 바깥에 있는 공간이다.
2. margin요소를 추가하지 않을 경우 브라우저는 기본값으로 추가한다.
3. margin의 방향을 명시하지 않을 경우 모든 방향에 적용된다.
4. margin 10px 10px 10px 10px의 경우 시계 방향으로 적용된다.

## padding

1. padding은 box의 border로부터 안쪽에 있는 공간이다.
2. margin과 마찬가지로 상하좌우로 적용이 가능하다.

## inline과 block

1. block은 옆에 다른 요소가 올 수 없다.
2. inline은 옆에 다른 요소가 올 수 있다.
3. 대부분의 box는 block이다.
4. inline은 height와 width가 없다. block은 있다.

## id

1. id를 통해서 개별적으로 지정하여 요소를 적용해 줄 수 있다.
2. 태그 attribute에 id를 추가하고 #id이름 으로 지정하는 것이 가능하다.
3. css에서의 id와 html에서의 id가 같아야 적용이 된다.
4. \*은 모든 요소에 적용할 수 있도록 해준다.

## class

1. class를 통해서 효과를 적용하면 id로 적용할 때보다 중복을 피할 수 있다.
2. tag에 class attribute를 선언하고 .이름 을 통해서 효과를 적용한다.
3. class는 여러개를 적용시킬 수 있다.

## inline-block

1. block 요소 옆에 다른 요소가 오는 것을 위해서 만들어졌다.
2. 반응형 디자인이 불가능하여 창 크기가 달라지면 모든 것이 달라진다. 그래서 잘 사용하지 않는다.

## flex box

1. inline-block의 한계를 극복하기 위해서 만들어졌다.
2. 자동으로 위치를 게산해서 출력해준다.
3. justify-content는 주축에 적용되는 것이다.
4. align-items는 교차축에 적용되는 것이다.
5. flex-wrap을 통해 화면의 크기가 줄었을 때 요소를 겹치게 할 것인지 아래로 내릴 것인지 결정해준다.
6. flex-direction을 통해서 주축과 교차축을 서로 전환시킬 수 있다.
7. flex box를 적용시키기 위해서는 부모에게만 명시하고 자식에게는 명시할 필요가 없다.

## position

1. fixed를 하면 커서를 내려도 박스가 움직이지 않는다. (메뉴창을 구현할 때 주로 사용한다.)
2. static은 레이아웃이 박스를 처음 위치하는 곳에 두는 것을 말한다.
3. absolute는 원하는 좌표로 이동시켜준다. 부모가 relative가 아니면 body를 기준으로, relative면 부모를 기준으로 움직인다.
4. relative는 element가 처음 위치한 곳을 기준으로 위치를 조정하고 싶을 때 사용한다.

## pseudo selectors

1. id를 통해서 지정하는 것보다 pseudo selector를 활용하면 더 깔끔하게 적용시킬 수 있다.
2. first-child, last-child를 통해서 각각 첫번째, 마지막 tag에 효과를 지정시킬 수 있다.

## nth-child

1. nth-child()에 원하는 요소의 순서를 집어 넣으면 n번째 요소에 적용 시킬 수 있다.
2. ()안에 수식을 적용시킬 수 도 있다. ex 2n+1

## 여러가지 pseudo selector들

1. p span은 p내에 있는 span에 적용시키라는 것이다.
2. div > span은 자식 바로 아래 span에 효과를 주는 것이다.
3. p + span은 p 바로 다음 span에 효과를 적용시키라는 것이다.
4. p ~ span은 p 무조건 다음이 아니어도 span에 효과를 적용시키도록 해준다.
5. attribute에도 효과를 적용시킬 수 있다.
6. input[placeholder~="name"]은 name을 포함한 placeholder에 효과를 적용시키라는 것이다.

## status

1. 각 상태일 때 효과를 적용시키는 것이 가능하다.
2. hover는 마우스가 올라가 있는 상태를 의미한다.
3. focus는 마우스 뿐 아니라 키보드로도 선택이 가능케 한다.
4. visited는 방문했던 웹사이트면 효과를 적용시켜준다.
5. focus-within은 focused인 자식을 가진 부모 element에 적용시켜준다.
6. 여러 조건을 연계하여 적용시키는 것이 가능하다.

## color

1. css에서 color는 중요한 역할을 한다.
2. color는 #fcce00, teal, rgb, rgba 방법으로 정의할 수 있다.

## 변수

1. :root{}를 통해서 변수를 지정할 수 있다.
2. --변수명 로 변수를 선언할 수 있다.
3. 변수를 선언할 때에는 공백을 허용하지 않으므로 -를 사용한다.
