# 흐름 제어

<br>

## Branch, Sequence, Flip Flop

<br>

### Branch
- 조건에 대한 True, False에 따라서 분기하여 실행된다
- 댠축키: B + 좌클릭

### Sequence

<img src="../images/UE5_BluePrint/Sequence.png" width = 600>

- 코드를 순서대로 실행한다

### Flip Flop

<img src="../images/UE5_BluePrint/FlipFlop.png" width = 600>

- 코드가 번갈아가면서 실행된다

## Min, Max, Clamp

<br>

### Min

<img src="../images/UE5_BluePrint/Min.png" width = 600>

### Max

<img src="../images/UE5_BluePrint/Max.png" width = 600>

### Clamp

<img src="../images/UE5_BluePrint/Clamp.png" width = 600>

- min, max 값을 넘어서지 않도록 한다

<br>

## For Loop, While Loop

### For Loop

<img src="../images/UE5_BluePrint/For.png" width = 600>

### While Loop

<img src="../images/UE5_BluePrint/While.png" width = 600>

### For Loop With Break

<img src="../images/UE5_BluePrint/ForBreak.png" width = 600>

<br>

### 연습문제: 구구단

<img src="../images/UE5_BluePrint/Gugudan.png" width = 600>

<br>

## Gate, MultiGate, Do Once, Do N

<br>

### Gate

<img src="../images/UE5_BluePrint/Gate.png" width = 600>

- 통과할 수 있는 문처럼 작동한다
- Open이면 통과하고 Close면 통과하지 않는다

### MultiGate

<img src="../images/UE5_BluePrint/MultiGate.png" width = 600>

- Sequence 처럼 Out이 순차적으로 동작한다
- Loop를 통해서 반복할 수 있다
- Reset: 처음부터 다시 실행
- Random: Out 중에서 랜덤으로 동작한다

### Do Once
- 한 번만 실행한다

### Do N
- N번 실행한다

<br>

## Enum

- 콘텐츠 브라우저 안에서 우클릭 -> BluePrints -> Enmeration

<img src="../images/UE5_BluePrint/Enum.png" width = 600>

- 생성 후 다음과 같은 Enum Type을 만들 수 있다

<img src="../images/UE5_BluePrint/Switch.png" width = 600>

- Switch 문을 통해서 Enum 값에 따라 코드를 분기시킬 수 있다
- Enum To String과 Print String을 통해서 Enum 값을 출력할 수 있다.