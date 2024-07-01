# 제어 역전 컨테이너 / 의존성 주입

> 공식 문서를 요약하여 정리한 글입니다. 부정확한 내용이 서술되어 있을 수 있으며, 6.1 버전에 국한되어 있습니다.

[공식 문서](https://docs.spring.io/spring-framework/reference/core/beans.html)

## 레거시 방식 설정

### xml 작성

[Bean Overview](https://docs.spring.io/spring-framework/reference/core/beans/definition.html)

스프링에서 빈을 관리하기 위해서는 스프링 설정 xml 파일에서 직접 빈을 등록해주어야 한다.

## 어노테이션 기반 컨테이너 설정

[Annotation-based Container Configuration](https://docs.spring.io/spring-framework/reference/core/beans/annotation-config.html)

### `@Autowired`

의존성 관리에 등록된 빈들을 보고, 해당 필드/메소드/생성자에 알맞게 주입해준다.

생성자, setter, 필드에 작성이 가능하다.

[공식 문서에서는 생성자에 주입할 것을 권장한다.](https://docs.spring.io/spring-framework/reference/core/beans/standard-annotations.html)

[`@Autowired` 대신, J2EE에서 명세한 `@Inject`도 사용 가능하다.](https://docs.spring.io/spring-framework/reference/core/beans/standard-annotations.html)

### `@Component`

[class path scanning and managed components](https://docs.spring.io/spring-framework/reference/core/beans/classpath-scanning.html)

클래스에 등록하는 어노테이션. `@Entity`, `@Service`, `@Controller`, 어노테이션에도 해당 어노테이션이 등록되어 있다.

`@ComponentScan`으로 컴포넌트를 탐지할 경로를 등록해주면, 해당 경로 내 컴포넌트들이 자동으로 빈으로 등록된다.

## 자바 기반 컨테이너 설정

[Java-based Container Configuration](https://docs.spring.io/spring-framework/reference/core/beans/java.html)

### `@Bean`과 `@Configuration`

[Basic Concept: `@Bean` and `@Configuration`](https://docs.spring.io/spring-framework/reference/core/beans/java/basic-concepts.html)

`@Configuration`은 빈을 관리할 클래스이다. 해당 클래스는 자동으로 빈으로 등록되며, 내부 메소드에 등록된 빈들을 의존성 관리에 등록한다.

`@Configuration` 내 메소드에서 반환하는 객체가 의존성 관리에 등록된다.

빈은 메소드 이름을 기준으로 등록된다.

만약 메소드에 `@Bean`을 붙이지 않는다면, 싱글턴으로 생성하는 대신, 매 호출 시마다 새로 인스턴스를 생성한다.
