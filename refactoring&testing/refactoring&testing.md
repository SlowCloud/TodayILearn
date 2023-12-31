
# 리팩터링

## 사이트

- [리팩터링 구루 - 리팩터링 관련 정보 사이트](https://refactoring.guru/ko/design-patterns/catalog)
- [patterns-dev.github.io - 디자인 패턴 모음](https://patterns-dev-kr.github.io/)
- 우아한 객체지향
  - [유튜브 자료](https://www.youtube.com/watch?v=dJ5C4qRqAgA)
  - [슬라이드 자료](https://www.slideshare.net/baejjae93/ss-151545329)
  - [우아한 객체지향 1단계 - 객체 참조](https://github.com/eternity-oop/Woowahan-OO-01-object-reference)
  - [우아한 객체지향 2단계 - 도메인 서비스](https://github.com/eternity-oop/Woowahan-OO-02-domain-service)
  - [우아한 객체지향 3단계 - 도메인 이벤트](https://github.com/eternity-oop/Woowahan-OO-03-domain-event)

## 궁금했던 것들

- [indent depth(들여쓰기)](https://tjdtls690.github.io/studycontents/java/2022-11-06-indent_depth/)
  - [keep indentation level low](https://softwareengineering.stackexchange.com/questions/220461/keep-indentation-level-low)
- [private 메소드가 너무 많아져도 되는 걸까?](https://stackoverflow.com/questions/21505410/code-organization-with-many-private-methods)
  - 충분히 SRP를 지키고 있고, 다른 주제에 대한 일을 하는 게 아니라면 많아도 된다.
  - 마음에 들지 않는다면, inner class로 한번 더 구별하는 것도 좋다고 생각한다.
  - 지금까지의 경험으로는, 메소드에서 유연성을 챙기는 건 좋은 선택이 아니었다.  
  중복되는 코드를 줄이는 건 좋다. 하지만 비슷한 일을 하는 메소드를 억지로 줄이지는 않아야 한다. 
- [클래스와 메소드는 얼마나 작아야 하는가?](https://softwareengineering.stackexchange.com/questions/125357/keep-my-classes-and-methods-as-small-as-possible)
- [SOLID, KISS, YANGI](https://poikilo.github.io/2020/03/02/design-concept/)
- [Primitive Opsession](https://m.blog.naver.com/knix008/220693514074)
- [static method는 언제 써야 하는가](https://stackoverflow.com/questions/2671496/when-to-use-static-methods)
- [[Java] 리팩토링 중 private static이 나오는 이유](https://ddududdudu.github.io/blog/2019/11/18/java-private-static-method/)
- getter에 대해서
  - [getter는 무조건 지양해야 하는가?](https://tecoble.techcourse.co.kr/post/2020-04-28-ask-instead-of-getter/)
  - getter는 언제 쓰는가?
    - IMO. 데이터로부터 가공된 정보가 아니라 그 데이터 자체가 필요하다면 getter를 쓰는 게 좋은 것 같다.
    - 사실 남용하지만 않으면 그냥 getter로 다 열어버려도 상관없는 게 아닐까?
    - 객체에 대한 기능들을 묶어두는 용도로 클래스를 쓰는 거라고 생각하면 정말로 상관없는 것 같다.
    - 자세한 기능구현을 숨기고 한 곳에 모아두는 용도라고 생각하면 진짜 상관없을 것 같다.
  - [getter는 어떻게 쓰는가](https://stackoverflow.com/questions/54506230/ddd-aggregate-should-getters-be-really-avoided)
  - [디미터 원칙](https://dkswnkk.tistory.com/687)
- [private constructor는 언제 쓰는 것이 좋은가?](https://stackoverflow.com/questions/2062560/what-is-the-use-of-making-constructor-private-in-a-class)
- [테스트가 어려운 객체는 잘못 설계된 객체인가?](https://jojoldu.tistory.com/687)
  - 테스트가 쉬운 객체는 어떤 객체인가?
  - 테스트가 쉬운 객체를 짜는 방법은?
- [equals와 hashcode는 같이 재정의해야 한다](https://tecoble.techcourse.co.kr/post/2020-07-29-equals-and-hashCode/)
- [일급 컬렉션을 쓰는 이유](https://tecoble.techcourse.co.kr/post/2020-05-08-First-Class-Collection/)
- 정적 팩토리는 언제, 왜 써야 하는가?
  - [정적 팩토리 메소드에 대한 설명](https://johngrib.github.io/wiki/pattern/static-factory-method/)
  - [생성자 VS 정적 팩토리](https://www.baeldung.com/java-constructors-vs-static-factory-methods)
  - [정적 팩토리를 쓰는 이유에 대한 좋은 예시](https://stackoverflow.com/questions/929021/what-are-static-factory-methods)
  - [정적 팩토리 메소드 컨벤션](https://sun-22.tistory.com/84)
- [[java] record의 구조](https://blog.hexabrain.net/399)
- [Stream vs Loop](https://www.baeldung.com/java-streams-vs-loops)
- [[Intellij] 스크래치 파일에 대해](https://velog.io/@min-zi/IntelliJ-%EC%9D%B8%ED%85%94%EB%A6%AC%EC%A0%9C%EC%9D%B4-Scratch-File)
- [Stream 내 if는 filter로 바꾸기](https://www.baeldung.com/java-8-streams-if-else-logic)
- [메소드 리팩터링 방법](https://wikidocs.net/600)
- [오버 엔지니어링에 대해서](https://velog.io/@young_pallete/%EC%98%A4%EB%B2%84%EC%97%94%EC%A7%80%EB%8B%88%EC%96%B4%EB%A7%81%EC%97%90-%EB%8C%80%ED%95%9C-%EB%8B%A8%EC%83%81)
  - [오버 엔지니어링은 불필요한가?](https://minslovey.tistory.com/117)
- [class는 얼마나 많아야 많은 걸까?](https://softwareengineering.stackexchange.com/questions/304197/how-many-classes-are-too-many)
- [응집도와 결합도에 대해서](https://lazineer.tistory.com/93)
- [[java] enum으로 다형성을 구현하는 2가지 방법](https://velog.io/@ljinsk3/Enum%EC%9C%BC%EB%A1%9C-%EB%8B%A4%ED%98%95%EC%84%B1%EC%9D%84-%EA%B5%AC%ED%98%84%ED%95%98%EB%8A%94-%EB%B0%A9%EB%B2%95)
- DDD
  - [애그리거트](https://mininkorea.tistory.com/40)
  - [DDD - 애그리거트](https://jaehoney.tistory.com/223)
- 내부 클래스를 쓰는 것은 나쁜가?
  - [내부 클래스는 어떨 때 쓰는 걸까?](https://stackoverflow.com/questions/18396016/when-to-use-inner-classes-in-java-for-helper-classes)
  - [내부 클래스의 장단점](https://inpa.tistory.com/entry/JAVA-%E2%98%95-%EB%82%B4%EB%B6%80-%ED%81%B4%EB%9E%98%EC%8A%A4Inner-Class-%EC%9E%A5%EC%A0%90-%EC%A2%85%EB%A5%98#1._%ED%81%B4%EB%9E%98%EC%8A%A4%EB%A5%BC_%EB%85%BC%EB%A6%AC%EC%A0%81%EC%9C%BC%EB%A1%9C_%EA%B7%B8%EB%A3%B9%ED%99%94)
  - [nested class와 inner class의 차이](https://tworab.tistory.com/49)
  - inner class는 outer class의 요소들을 직접 참조할 수 있다. 이를 적극적으로 활용할 수 있다면 내부 클래스를 만드는 게 좋다!
- [객체지향 연관성](https://itwiki.kr/w/%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5_%EC%97%B0%EA%B4%80%EC%84%B1)
  - 분류화, 집단화, 일반화, 특수화
- TDD, 바텀업이냐 탑다운이냐
  - [한 해외 개발자의 탑다운 TDD 시도 경험](https://medium.com/@ambye/top-down-vtdd-1f3aebf9b22)
    - 분리했던 책임이, 더 낮은 단계에서 다시 결합하는 경험을 했다고 함.

## 결론을 내리지 못한 것들

- 내부 클래스를 쓰는 것은 나쁜가?
  - 외부에서 사용되어야 하지만, 특정 클래스의 내부 요소들에 대해 깊이 관여하는 경우(많은 value들을 요구, 값을 자주 참조, 또는 특정 클래스에 한정적인 데이터를 보유하는 경우?) nested class를 사용한다?
  - inner class는 outer class의 요소들을 직접 참조할 수 있다. 이를 적극적으로 활용할 수 있다면 내부 클래스를 만드는 게 좋다!
    - --> 너무 적게 쓰이는 getter들을 만들지 않아도 된다!!
    - 그러면 DTO도 inner class로 손보면 편한 작업이 가능하지 않을까?
  - 단순 메소드 정리의 용도로 사용하는 경우도 있던데, 이것도 잘 활용하고 있는 게 맞는가?
- 객체의 깊이가 깊어져도 되는가?
  - 래핑이 너무 많이 이루어져도 되는가?
- "거대한 객체"의 기준은 무엇인가?
  - IMO. SRP를 지키기만 한다면, "거대한 클래스"가 아니다?
  - 메소드가 한 가지 일만 함을 나타냄은, 프로세스를 최대한 잘게 쪼갠 것임을 의미한다?
  - 클래스가 한 가지 일만 함을 나타냄은, 한 가지 주제에 대한 메소드, 또는 객체에 대한 데이터와 그에 관련한 메소드만을 가짐을 의미한다?
- 클래스를 쪼개서 늘어나는 클래스들은 어떻게 관리하는가?
  - ~~IMO. 클래스를 쪼개고, 외부에서 사용할 필요가 없는 클래스는 default 접근자를 먹인다.~~
    - [[java] 클래스를 숨기는 방법](https://stackoverflow.com/questions/6642909/providing-java-library-but-hiding-some-classes)
    - [[java] public, protected, default, private](https://mainia.tistory.com/5574)
  - default를 써봤는데, default로 감춰진 클래스들이 구별이 안 되어서 유지보수가 더 힘들다고 느꼈다.
- IMO. getter를 쓰면 된다. record는 필요할 때에만 쓰자.
  - 인자로 넘겨받는 정보는 최소한의 정보여야 하는가?
    - DTO 객체를 받지 말고, DTO 내에서 필요한 정보만 꺼내 받는 식으로?
    - 이건 여러 상황을 겪어봐야 알 것 같다.
  - 반환값은 원시값 또는 record 객체로 제한하는 것이 좋은가?
  - 원시값을 감싸는 객체들은 record로 만드는 것이 좋은가?

## 기타 의견

- 메소드에서 유연성을 챙기는 건 좋은 생각이 아니라는 것을 느꼈다. 비슷한 메소드가 많다고 줄여보려고 하지 말고, 그냥 메소드를 늘리는 게 맞는 것 같다.
  - 중복되는 코드를 너무 많이 만들어도 된다는 말은 아니다.
  - 메소드 하나가 유연하게 일을 하는 게 아니라 한 가지 일만 하게 하고, 중복되는 로직은 내부에서 잘 리팩토링해야 한다.
  - 리팩토링 역시 과하게 진행하지 말고, 중복되는 로직도 잘게 쪼개어 필요한 만큼만 분리하는 작업이 필요하다. 지나치게 과하게 진행되면 수정이 힘들고, 가독성이 떨어지기도 한다.
  - 기준은 유지보수하기 편한 정도를 기준으로. 리팩토링을 해보고 괜찮다 싶으면 사용하고, 딱히 나아진 점이 없다 싶으면 되돌린다.
- 클래스 역시 마찬가지다. 클래스를 수정에 유연하게 하지 말고, 확장에 유연하게 만드는 게 좋은 것 같다.
  - 종단 클래스는 수정하지 말고, 새 객체를 만들거나, 해당 객체를 abstract로 바꾸고 상속하거나, 인터페이스를 활용하는 게 좋은 것 같다.
- 데이터 객체, 관계 객체, 행위 객체 3가지로 나누면 좋을 것 같다.
  - 데이터 객체, 관계 객체는 DB 테이블 설계와 비슷하게 설계하고, 행위 객체는 어떠한 큰 프로세스 단위에서 사용되는 메소드와 객체들을 모아서 명령하듯 실행하는 객체로 구별하면 될 것 같다.
  - 행위 객체는 내부적으로 사용되는 자잘한 행위 객체들을 가져도 된다. 프로세스 단위에 따라 그 크기가 달라질 것 같다.
  - 객체 설계에 데이터 모델링과 정규화를 활용해보는 것도 좋을 것 같다.
  - [데이터 모델링](https://dataonair.or.kr/db-tech-reference/d-guide/da-guide/?mod=document&uid=277)

## 예시
```
// 아래 코드의 예시는 숫자야구 게임

// 적은 추상화, 잘게 나눠진 메소드
// game에 inputView, outputView와 같은 외부 객체를 주입할 필요가 없음
// 각 메소드마다 적은 케이스들로 쉽게 테스트 가능
while(!game.end()) {
	String numbers = inputView.getNumbers();
	StrikeAndBall strikeAndBall = game.check(numbers);
	outputView.printStrikeAndBall(strikeAndBall);
}
outputView.printTryCount(game.getTryCount());

// 지나친 추상화, 많은 일을 하는 메소드
// inputView, outputView와 같은 객체들을 주입해주어야 함
// 하나의 메소드에 많은 케이스들에 대한 검증이 필요함. 테스트가 어려워짐
outputView.printResult(game.process());
```

```
// 프로세스를 한 주제를 중심으로 객체로 추상화하였음. game이 여러 데이터 객체를 활용하는 행위 객체가 됨
// 메소드를 너무 잘게 쪼개면 임시로 값을 저장할 내부 필드가 너무 많아지나..? 그러면 필드를 쓰지 말고 반환하게 해야지
// 그럼 아래에서는 isGameEnd를 그냥 외부로 옮기는 게 맞을까? 아니면 그냥 메소드 위치가 안 맞는 걸지도
// game이 아니라 strikeAndBall에 물어봐야지
// 이러면 또 분기 문제인가?
// class Game { Answer answer, int tryCount, boolean isGameEnd }
while(!game.end()) {
	String numbers = inputView.getNumbers();
	StrikeAndBall strikeAndBall = game.check(numbers);
	outputView.printStrikeAndBall(strikeAndBall);
  game.count();
}
outputView.printTryCount(game.getTryCount());
/*
while(true) {
	String numbers = inputView.getNumbers();
	StrikeAndBall strikeAndBall = game.check(numbers);
	outputView.printStrikeAndBall(strikeAndBall);
  if(strikeAndBall.isThreeStrike()) break;
  game.count();
}
outputView.printTryCount(game.getTryCount());
*/
/*
while(true) {
	String numbers = inputView.getNumbers();
	StrikeAndBall strikeAndBall = game.check(numbers);
	outputView.printStrikeAndBall(strikeAndBall);
  if(game.end(strikeAndBall)) break;
  game.count();
}
outputView.printTryCount(game.getTryCount());
*/
// 일단 요구사항이나 보고 고민을 해보자고 이런 건
// 일단 게임이 끝났는지를 묻는 건 strikeAndBall에 묻는 게 맞고, 횟수를 세는 건 어떻게 할지 고민해보자
// 일단 각 필드끼리 상호작용하지 않았으니 분리하는 게 맞는 듯?

// game의 내부 필드를 분리하여 구현한 모습. 게임에 관한 로직이 구체적으로 드러나 있다.
int cnt = 1;
while(true) {
	String numbers = inputView.getNumbers();
	StrikeAndBall strikeAndBall = answer.check(numbers);
	outputView.printStrikeAndBall(strikeAndBall);
  if(strikeAndBall.isThreeStrike()) break;
  cnt++;
}
outputView.printTryCount(cnt);
```

```
// 어떤 것을 사용하는 것이 좋은가?

// 적은 메소드, 유연한 작업 처리
today.is(Today.Calender.WEEKEND); // (calender) -> calender.apply(localDate)
today.is(Today.Calender.WEEKDAY);
today.is(Today.Calender.MONDAY);

// 많은 메소드, 한가지 작업만 처리
// 내부적으로는 위와 똑같이 구현됨
today.isWeekend(); // () -> is(Calender.WEEKEND)
today.isWeekday();
today.isMonday();
```

```
// 어떤 것을 사용하는 것이 좋은가? 22
// 함수지향이라면 고민하지 않아도 될 문제였을 것 같다.

// 많은 객체들, 다형성/추상화
backendCrews = backendCrewReader.read();
frontendCrews = frontendCrewReader.read();

// 적은 객체, 메소드로 처리
backendCrews = crewReader.readBackend();
frontendCrews = crewReader.readFrontend();
```

```
// 어떤 것을 사용하는 것이 좋은가? 333

// 자료구조로 처리
Map<Book, Price> priceOfBooks;

// 관계 객체로 처리
record PriceOfBook(Book book, Price price) {}
List<PriceOfBook> priceofBooks;
```

```
// 어떤 것을 사용하는 것이 좋은가? 4444

// 값을 꺼내서 주기
// 의존성 없음
// 값에 대한 검증이 되지 않음
outputView.printName(name.getName());

// 일단 넘겨받고 내부에서 값을 꺼내 쓰기
// 의존성이 생김
// 검증된 값을 넘겨받음
outputView.printName(name); // System.out.println(name.getName());
```

# 테스팅

## 사이트

- [JUnit5 User Guide](https://junit.org/junit5/docs/current/user-guide/)
- [Mockito Docs](https://javadoc.io/doc/org.mockito/mockito-core/latest/org/mockito/Mockito.html)
- [assertj 주요 기능 오버뷰](https://sun-22.tistory.com/86)
- [shoulditestprivatemethods.com - feat.kent beck](https://shoulditestprivatemethods.com/)

## 궁금했던 것들

- [난수는 테스트가 가능한가?](https://softwareengineering.stackexchange.com/questions/356456/testing-a-function-that-uses-random-number-generator)
  - 정확히 무엇을 테스트하고 싶은지를 확실시해라.
  - 난수의 정규분포를 계산하고 싶은 게 아니라면, 모킹을 활용해라.
- private field testing
  - [리플렉션](https://hudi.blog/java-reflection/)
    - [테스트를 위해 private field에 접근하는 방법](https://stackoverflow.com/questions/27857612/access-a-private-field-for-a-junit-test)
    - 권장하지 않는 편.
  - [guava를 이용한 private method 테스트](https://yearnlune.github.io/java/java-private-method-test/#visiblefortesting)
  - [assertj를 이용한 private 필드 검사](https://www.baeldung.com/java-extract-values-assertj)
- [static 메소드를 테스트하는 3가지 방법](https://www.javaindeed.com/3-best-practices-to-test-a-code-that-calls-static-methods/)
  - [static 메소드 모킹하기](https://unluckyjung.github.io/testcode/2021/12/20/Mockito-StaticMethod-Mocking/)
  - 대체로 권장하지 않는 편.
- [유닛테스트 네이밍 컨벤션](https://middleearth.tistory.com/39)
- BDD(Behavior Driven Development)
- [DCI 패턴](https://johngrib.github.io/wiki/junit5-nested/)
- [객체지향은 함수형보다 테스트하기 어려운가?](https://softwareengineering.stackexchange.com/questions/351815/why-is-unit-testing-harder-in-object-oriented-programming-compared-to-functional)