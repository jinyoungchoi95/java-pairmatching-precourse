# Todo List
## Course

- 코스는 백엔드와 프론트 앤드로 나누어진다.

## Level

- 레벨은 1부터 5레벨까지 존재한다.
- 레벨에 해당하는 미션을 포함할 수 있다.

## Crew

- 크루원의 정보는 이름과 어떤 코스인지로 나누어진다
- [ERROR] 이름은 공백이 들어올 수 없다.
- 크루원 정보를 받아 저장할 수 있다.
- 해당 코스의 크루원 정보를 반환할 수 있다.
- [ERROR] 크루원의 이름이 중복될 경우 exception이 발생해야 한다.

## Matching

- 입력된 정보를 가지고 해당 미션의 페어를 매칭할 수 있다.
- 이미 매칭된 미션인 경우 재매칭 여부를 확인할 수 있다.
- [ERROR] 없는 과정과 레벨, 미션이 들어올 경우 exception이 발생해야 한다.
- 동일한 레벨의 매칭이력이 있는 유저인 경우 다시 랜덤으로 섞어 매칭시도를 해야 한다.
- [ERROR] 3회 시도까지 매칭이 되지 않는 경우 exception이 발생해야 한다.
- 앞에서부터 순서대로 두명씩 페어를 맺을 수 있다.
- 매칭 대상이 홀수인 경우 마지막 크루원은 마지막 페어에 포함한다.

## Mission

- 각 미션에는 페어 매칭 결과가 저장되어 있다.
- 이미 페어 매칭 결과가 지정되어있더라도 초기화하여 다시 저장할 수 있다.
- 전체 미션을 초기화할 수 있다.
- 이미 미션 내에 페어가 한번 존재한 경우 이를 확인할 수 있다.
- [ERROR] 동일한 레벨에 동일한 이름의 미션이 들어올 경우 exception이 발생해야 한다.
- [ERROR] 중복된 이름의 Mission이 저장될 경우 exception이 발생해야 한다.
- [ERROR] Mission을 찾을 수 없을 경우 exception이 발생해야 한다.

## Match
- Match 정보를 받아서 해당 Match와 동일한지 확인할 수 있다.
- 홀수로 3명이 들어간 Match 객체를 생성할 수 있다.

## Command
- 요청 Command는 1, 2, 3, Q의 요청이 있다.
- [ERROR] 없는 요청 Command를 호출할 경우 exception이 발생해야 한다.