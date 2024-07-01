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
- [클래스와 메소드는 얼마나 작아야 하는가?](https://softwareengineering.stackexchange.com/questions/125357/keep-my-classes-and-methods-as-small-as-possible)
- [SOLID, KISS, YANGI](https://poikilo.github.io/2020/03/02/design-concept/)
- [Primitive Opsession](https://m.blog.naver.com/knix008/220693514074)
- [static method는 언제 써야 하는가](https://stackoverflow.com/questions/2671496/when-to-use-static-methods)
- [[Java] 리팩토링 중 private static이 나오는 이유](https://ddududdudu.github.io/blog/2019/11/18/java-private-static-method/)
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
- [class는 얼마나 많아야 많은 걸까?](https://softwareengineering.stackexchange.com/questions/304197/how-many-classes-are-too-many)
- [응집도와 결합도에 대해서](https://lazineer.tistory.com/93)
- [[java] enum으로 다형성을 구현하는 2가지 방법](https://velog.io/@ljinsk3/Enum%EC%9C%BC%EB%A1%9C-%EB%8B%A4%ED%98%95%EC%84%B1%EC%9D%84-%EA%B5%AC%ED%98%84%ED%95%98%EB%8A%94-%EB%B0%A9%EB%B2%95)
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

# 테스팅

## 사이트

- [JUnit5 User Guide](https://junit.org/junit5/docs/current/user-guide/)
- [Mockito Docs](https://javadoc.io/doc/org.mockito/mockito-core/latest/org/mockito/Mockito.html)
- [assertj 주요 기능 오버뷰](https://sun-22.tistory.com/86)
- [shoulditestprivatemethods.com - feat.kent beck](https://shoulditestprivatemethods.com/)

## 궁금했던 것들

- [유닛테스트 네이밍 컨벤션](https://middleearth.tistory.com/39)
