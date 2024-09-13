# Code Convention

## 1. Naming 규칙

#### 1.1 변수명, 함수명
- camelCase에 따라 변수명과 함수명을 정의한다.
- 첫단어는 소문자로 표기하고, 이어지는 단어의 첫글자만 대문자로 표기하는 방법
- - 예) `userCart`, `userCartList`

  #### 1.2 패키지 이름
  - 패키지 이름은 소문자로 구성한다.

  #### 1.3 클래스, 인터페이스
  - pascalCase에 따라 클래스와 인터페이스를 정의한다.
  - 단어의 첫 글자만 대문자로 표기한다.
- 예) `UserFoam`, `StockInfo`

#### 1.4 클래스 이름은 명사를 사용한다.

#### 1.5 인터페이스 이름은 명사/형용사를 사용한다.

#### 1.6 메서드 이름은 동사/ 전치사로 시작한다.

#### 1.7 상수는 대문자와 언더스코어로만 구성한다.
- 예) `public final float RISK_FREE_WEIGHT = 10.95;`

## 2. 포맷
#### 2.1 중괄호 `{` `}`
- if, for, while, else 문에 코드가 없거나 한 문장이라도 중괄호를 생략하지 않습니다.

## 3. 선언

#### 3.1 소스파일당 1개의 탑레벨 클래스를 담기
- 굳이 한 파일 안에 선언해야 한다면 내부 클래스로 선언
Ex)
**잘못된 예**
```
// User.java
class User{}
class Edge{}
```
**옳은 예**
```
class User{
  class Edge{}
}
```