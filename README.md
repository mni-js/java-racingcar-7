# java-racingcar-precourse

---
### 과제 제출 전 체크 리스트
- [ ] 요구 사항에 명시된 출력 형식을 따랐는가?
- [ ] 테스트 실행 가이드에 따라 모든 테스트가 성공적으로 실행되는가?
- [ ] indent depth가 2까지만 있는가?
- [ ] 삼항 연산자를 쓰지 않았는가?
- [ ] Method가 한 가지 일만 하는가?
- [ ] JUnit5와 AssertJ를 이용하여 기능 목록이 정상 작동하는지 테스트 하였는가?
---
### 구현할 기능 목록
#### 1. **자동차 이름 입력받기**
- 이름에는 한글, 영문, 기호를 모두 허용한다. 단 구분자로 사용되는 쉼표(,)는 허용하지 않는다. 
- 빈문자열도 잘못된 값으로 규정한다.
- [x] 자동차 이름을 쉼표(,)를 기준으로 구분하는 기능
- [x] 자동차 이름이 5자 이하만 가능하도록 제한하는 기능
- [x] 잘못된 값을 입력할 경우 `IllegalArgumentException`을 발생시키는 기능

#### 2. 게임의 총 진행 횟수 입력받기(몇 번 이동할 것인지)
  1) 게임 진행 횟수에는 제약을 두지 않을 것인가? 
  -> 최소 1번 이상은 진행하도록 입력을 받자 + 자연수만 입력받도록 제약을 걸자.

#### 3. 정해진 진행 횟수 동안 자동차 전진 시키기
- [ ] 각각의 자동차에 대해서 0 ~ 9 사이에서 무작위 값을 구하는 기능
  1) 총 진행 횟수 동안(for문 사용) + 각각의 자동차에 대해서(for문 사용)이면 depth가 많아질 듯 하다.
  -> 그래서 Method를 분리하라고 했나보다.
- [ ] 무작위 값이 4 이상일 경우 해당 자동차가 전진하는 기능
- [ ] 진행 차수 별 실행결과를 출력하는 기능(형태 -> 자동차 이름: 전진 칸 수((-)로 표현))

#### 4. 게임 끝! 우승자 발표하기
- [ ] 우승자를 출력하는 기능
- [ ] 우승자가 여러 명일 경우 쉼표(,)를 이용하여 구분하는 기능
  1) 전진하지 않아서 우승자가 없을 경우에는?
  -> 우승자가 없다고 출력할까.. 모두 출력할까..
