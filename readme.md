## 그리디 Greedy 란?
- 탐욕법
- 당장 좋은 것만 선택
- 단순하고 강력한 문제해결 방법

### 예제
- 거스름돈
- 음식점에서 계산을 도와줍니다.
- 거스름돈으로 500원, 100원, 50원, 10원
- 손님에게 거슬러줘야 할 돈이 N원일 때
  - 거슬러줘야 할 돈(change)은 항상 10의 배수입니다.
- 거슬러줘야 할 동전의 최소 개수를 구하세요.
- ex) change : 1,260원

# 숫자 크기비교
- big_number
- 숫자 3개를 입력받기
- 입력받은 숫자 정렬하기
- 정렬된 숫자 크기를 출력해주세요.

# 숫자 크기비교2 - 큰 수의 법칙
- big_number2
- 다양한 수로 이루어진 배열이 있을 때
- 주어진 수를 M번 더하여 가장 큰 수를 만드는 법칙
- 특정한 수가 연속해서 K번 초과해서 더할수는 없다.

- 예제
- [2,4,5,4,6], M=8, K=3
- 6 + 6 + 6 + 5 + 6 + 6 + 6 + 5 = 46

[입력조건]
- 첫째 줄에 N (몇 개:`2~1000`), M(`1~10000`), K(`1~10000`)
- 둘째 줄 N개 자연수 입력하는데, 각 자연수는 공백으로 구분한다.
- 입력으로 주어지는 K는 항상 M보다 작거나 같다.
  - 예시) 5 8 3
  - 2 4 5 4 6
[출력조건]
- 첫째 줄에 큰수의 법칙에 따라 더해진 답을 출력한다.
  - 46


# 돈 출력하기
- change_money
- 숫자를 입력받으세요 (~원)
- 입력받은 숫자를 coin_list에 비교하여 큰것부터 개수를 반환해주세요.

# 돈 출력하기2 - 거스름돈
- change_money2
- 거스름돈으로 500원, 100원, 50원, 10원
- 손님에게 거슬러줘야 할 돈이 N원일 때
  - 거슬러줘야 할 돈(change)은 항상 10의 배수입니다.
- 거슬러줘야 할 동전의 최소 개수를 구하세요.
- ex) change : 1,260원

# 가장 큰 수 출력하기
- number_card_game
- 숫자 몇개 받을지 입력받으세요
- 해당 숫자만큼 숫자를 입력해주세요
- 입력받은 숫자들 중 가장 큰 수를 출력해주세요

# 작은 수 중 큰 값 출력 - 숫자 카드 게임
- minimum_maximum
- 여러개 숫자 카드 중 가장 높은 숫자 한 장을 뽑는 게임

1. 카드 N(row) X M(column) 형태로 놓여있다.
2. 뽑고자 하는 행(row)을 선택한다.
3. 그 다음 선택된 행의 카드 중 가장 낮은 숫자의 카드를 뽑아야 한다.
4. 따라서, 처음 카드 골라낼 행 선택할 때, 3번 룰을 고려하여 최종적으로 가장 높은 카드를 뽑도록 전략을 세워야 한다.


```
3 1 2
4 1 3
4 6 7
```

[입력조건]
- 첫째 줄 N M 입력받습니다. (1~100)
- 둘째 줄부터 각 카드에 적힌 숫자가 주어진다. (1~10000)
```
3 3
3 1 2
4 1 3
4 6 7
```

[출력조건]
- 게임 룰에 맞는 숫자 출력 
2
- (입출력 예시2)
```
2 4
7 3 1 8
3 3 3 4
```
out : 3

# 1이 될때까지
- just_number1
- 어떤 수 N을 1이 될 때까지 다음 두 과정 중 하나를 반복적으로 선택해서 수행하려고 한다
- 단, 두번째 연산은 N이 K로 나누어떨어질 때만 선택할 수 있다.

1. N에서 1뺀다.
2. N을 K로 나눈다.

- 예시) N=17, K=4,
n = 16, n = 4, n = 1
실행횟수 3

- 과정을 수행하는 최수횟수를 구하는 프로그램을 작성하세요.

[입력조건]
- 첫째 줄에 공백으로 구분된 자연수
- N은 항상 K보다 크거나 같다.

[출력조건]
- 1이 될때까지 2가지 과정을 수행하는 최소값

[예시]
- 입력 : 25 5 / 출력 : 2
- 입력 : 17 4 / 출력 : 3