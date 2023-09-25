# 애니메이션 관리

<br>

## 입력 매핑

<br>

### Source FlipBook을 설정하는 Set FlipBook

<br>

<img src="./images/InputMapping.png" width = 500>

<br>

### WASD로 방향에 따른 FlipBook의 변환

<br>

<img src="./images/InputMapping2.png" width = 500>

- Side Idle 상태에서 서로 반대편을 바라보기 위해 A와 D 입력의 Z Rotation이 180도 달라야 한다

<br>

### WASD 키보드 이벤트 보다는 Axis Mapping을 이용하는 것이 좋다

<br>

<img src="./images/InputMapping3.png" width = 500>

<br>

### AxisMapping을 통한 WASD의 입력 매핑

<br>

<img src="./images/InputMapping4.png" width = 500>

<img src="./images/InputMapping5.png" width = 600>

<br>

## 매크로

<br>

### 더 간편하게 비교하는 Compare[Type] 매크로

<br>

<img src="./images/Macro.png" width = 500>

<br>

### 블루프린터 에디터 좌측의 매크로 추가하기

<br>

<img src="./images/Macro2.png" width = 500>

<br>

### 함수 VS 매크로
- 매크로는 그저 만들어둔 코드를 복사해서 붙여넣는 것이다
- 함수는 블루프린트 클래스를 상속받은 경우 오버라이딩을 할 수 있다
- 매크로는 Delay 처럼 노드의 실행 흐름을 늦출 수 있지만 함수는 한 번 실행되면 끝까지 지연 없이 실행되어야 한다

<br>

## 애니메이션 갱신

<br>

### EDirection 추가

<br>

<img src="./images/AnimationUpdate.png" width = 500>

<br>

### Enum과 함수를 통한 애니메이션 갱신

<br>

<img src="./images/AnimationUpdate2.png" width = 600>

<img src="./images/AnimationUpdate.png3" width = 600>

<br>

### 키보드 입력을 알 수 있는 방법

<br>

<img src="./images/AnimationUpdate4.png" width = 600>

<br>

### 움직임과 Idle을 동시에 구현하기

<br>

<img src="./images/AnimationUpdate5.png" width = 600>

<img src="./images/AnimationUpdate6.png" width = 600>

<br>

## 공격 애니메이션

<br>

### 입력 이벤트 리팩토링

<br>

<img src="./images/AttackAnimation.png" width = 600>

<img src="./images/AttackAnimation2.png" width = 600>

- UpdateInput 함수 추가

<br>

### Action Mapping 추가하기

<br>

<img src="./images/AttackAnimation3.png" width = 600>

<br>

### 공격 애니메이션 추가하기

<br>

<img src="./images/AttackAnimation4.png" width = 600>

- 하지만 이렇게 되면 공격 애니메이션이 멈추지 않게 된다

<br>

### FlipBook의 길이를 알 수 있는 Get FlipBook Length

<br>

<img src="./images/AttackAnimation5.png" width = 600>

- FlipBook의 길이만큼 Delay한 후에 bAttack을 False로 만들어준다면 1회 공격 후 애니메이션이 멈추게 된다

<br>

## State 패턴

<br>

### 값에 따라서 옵션을 설정해주는 Select

<br>

<img src="./images/State.png" width = 500>

- Select를 통해 코드를 간략하게 만들 수 있다

<br>

### ***모든 상태를 Boolean 변수로 관리하다 보면 너무 많아지게 돼 관리가 힘들어진다***

<br>

### EState 만들기

<br>

<img src="./images/State2.png" width = 500>

<br>

### EState를 통해 함수 바꾸기

<img src="./images/State3.png" width = 600>

<img src="./images/State4.png" width = 600>

<img src="./images/State5.png" width = 600>

- Select와 Enum을 통해 코드를 간략하게 만들 수 있다