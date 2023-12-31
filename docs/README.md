# 기능 목록

## 입력 기능

### 구입 금액 입력 기능

- 구입 금액은 1000원 단위로 입력되어야 한다.

### 당첨 번호 입력 기능

- 당첨 번호는 쉼표를 기준으로 구분되는 1 ~ 45 까지의 6개의 정수를 입력받아야 한다.

### 보너스 번호 입력 기능

- 보너스 번호는 당첨 번호와 별개로 1 ~ 45 까지의 1개의 정수만 입력받아야 한다.
- 각 당첨 번호 간 및 당첨 번호와 보너스 번호 간 중복된 값은 입력받을 수 없다.

## 검증 기능

### 입력값 검증 기능

- 입력받은 모든 값은 각 검증 로직을 통해 해당 값이 조건에 부합하는 지 확인해야 한다.

## 비교 기능

### 번호 비교 기능

- 구매한 로또의 갯수만큼 로또 번호를 당첨 번호와 비교해야 한다.
- 5개가 일치한 경우, 로또 번호 중 보너스 번호의 존재 여부를 확인해야 한다.
- 당첨된 로또 게임의 수를 각 일치 번호 수 및 보너스 당첨 수로 저장되어야 한다.

## 출력 기능

### 로또 번호 출력 기능

- 구입한 로또 수량과 수량에 맞는 각 로또 번호가 배열의 형태로 출력되어야 한다.
- 각 로또 번호 배열은 중복되지 않은 1 ~ 45의 정수 6개로 이루어져야 한다.
- 각 로또 배열의 요소는 오름차순으로 정렬되어야 한다.

### 당첨 통계 출력 기능

- 당첨 통계에서는 3개 일치부터 6개 일치까지 로또의 각 당첨 경우의 수 와 당첨금,해당 경우의 수 별로 당첨된 갯수를 오름차순으로 출력해야 한다.
- 당첨 통계의 마지막에서는 수익률을 출력해야 한다.
- 수익율은 소수점 첫째 자리까지 출력되어야 한다.

## 예외 관련 기능

### 예외 발생 기능

- 예외가 발생할 경우, throw 문을 사용해야 한다.
- 입력된 구입 금액이 1000원으로 나누어지지 않을 경우 예외를 발생시킨다.
- 입력된 당첨 번호가 1 ~ 45 까지의 6개의 중복되지 않는 정수가 아닐 경우 예외를 발생시킨다.
- 입력된 보너스 번호가 1 ~ 45 까지의 정수가 아닌 경우 예외를 발생시킨다.
- 입력된 당첨 번호간 중복이 발생하거나, 당첨 번호와 보너스 번호 간 중복이 발생할 경우 예외를 발생시킨다.

### 예외 처리 기능

- 예외가 발생된 후, "[ERROR]" 로 시작하는 관련 에러 메세지를 출력하고 해당 부분부터 다시 입력을 받아야 한다.
