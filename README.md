# TodayILearn

매일 새로 알게 된 내용을 정리하고, 레퍼런스를 관리하는 문서

## Git

### 사이트

- [Github Cheat Sheet - training.github.com](https://training.github.com/downloads/ko/github-git-cheat-sheet/)
- [git-tips](https://github.com/mingrammer/git-tips)
- [github docs](https://docs.github.com/ko)

### 액션

- [github action guide](https://docs.github.com/ko/actions)

## Java

### Stream

- [skip과 limit](https://observerlife.tistory.com/5)
- [java 9의 iterate](https://www.daleseo.com/java9-stream-iterate/)
- [Java 17 Stream Documentation](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/stream/Stream.html)

### Reflection

- [Java 17 Reflect Documentation](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/reflect/package-summary.html)

### Flux / reactor

함수형 / 선언형 / 반응형 프로그래밍 지원

## Intellij

- [유용한 단축키](https://blog.jetbrains.com/ko/2020/03/11/top-15-intellij-idea-shortcuts_ko/)
- [가장 많이 쓰인 단축키 15개](https://blog.jetbrains.com/ko/2020/03/11/top-15-intellij-idea-shortcuts_ko/)
- [라이브 템플릿 작성하기](https://www.jetbrains.com/help/idea/using-live-templates.html)

## Kotlin

- [Getting Started](https://kotlinlang.org/docs/home.html)

## Spring

Jakarta EE를 기반으로, 빠르게 웹 서버를 배포할 수 있도록 만들어진 프레임워크.

가장 대표적인 기능은 의존성 주입.

- [Spring Projects](https://spring.io/projects/)
- [Spring Quickstart](https://spring.io/quickstart/)
- [Spring Guide](https://spring.io/guides/)

### [의존성 주입](/spring/dependency_injection.md)

### 캐싱

- [Spring Cache Documentation](https://docs.spring.io/spring-framework/reference/integration/cache/annotations.html)

스프링 프레임워크 3.1부터 지원한다.

JSR-107로 등록된 JCache 어노테이션도 지원한다.

### 스프링 생태계

#### 스프링 부트

스프링 프레임워크의 웹 배포를 훨씬 빠르게 할 수 있도록 도와주는 생태계.

MyBatis와 같은 여러 라이브러리/의존성들의 흩어진 설정 파일들을 한 곳에서 설정할 수 있게 해주고,
스프링 프레임워크의 DI와 같은 기본 설정들도 자동으로 처리해주며,
내장 톰캣 서버를 제공하여 스프링 서버를 즉시 실행할 수 있게 해 준다.

#### 스프링 시큐리티

- [Spring Security Documentation](https://docs.spring.io/spring-security/reference/index.html)

사용자 인증/인가를 도와주는 스프링 생태계.

기본적인 보안 필터를 지원해주며, 추가적인 필터를 작성하여 커스텀 시큐리티 처리가 가능하다.

제대로 작업해둔다면, 컨트롤러에서 `@AuthenticationPrincipal`로 사용자 정보를 가져올 수 있다.

#### JPA

스프링 공식 문서에서는 JPA에 대해 소개하지 않는다.

JPA는 Jakarta EE의 공식 명세서나, Hibernate와 같은 구현체의 가이드를 참고하는 것을 추천한다.

- [스프링 JPA Repository 공식 가이드](https://docs.spring.io/spring-data/jpa/reference/)
  - JPA 기반 스프링 리포지토리 작성 방식을 알고 싶다면, 해당 가이드를 추천
- [Jakarta Persistence 공식 명세서](https://jakarta.ee/specifications/persistence/3.2/jakarta-persistence-spec-3.2)
  - JPA의 전체 기능을 알고 싶다면, 해당 명세서를 추천
- [하이버네이트 공식 문서](https://hibernate.org/orm/documentation/6.5/)
  - [하이버네이트 ORM 공식 가이드](https://docs.jboss.org/hibernate/orm/6.5/introduction/html_single/Hibernate_Introduction.html)
  - [하이버네이트 ORM 유저 가이드](https://docs.jboss.org/hibernate/orm/6.5/userguide/html_single/Hibernate_User_Guide.html)

### Gradle

- [Gradle 유저 가이드](https://docs.gradle.org/current/userguide/userguide.html)

### JSP와 서블릿, 그리고 톰캣

## HTML

- [시맨틱 태그](https://www.w3schools.com/html/html5_semantic_elements.asp)

## Vim

- [Vim 소개글](/vim/introduction.md)
- [Vimium - 크롬/파이어폭스 확장 프로그램](https://blog.ull.im/review/2018/11/22/vimium.html)
  - 키보드로 웹서핑하기
- [Vim Cheatsheet](https://vim.rtorr.com/lang/ko)
- [플러그인 설치하기](vim/plugin.md)
- [IdeaVim 활용과 커스터마이징](https://www.slideshare.net/imkimkevin/android-studio-vim-ideavim-94820340)

### 매핑

- [키보드 매핑](https://preppiepjh.tistory.com/entry/Vim-%ED%99%9C%EC%9A%A9-%ED%82%A4%EB%B3%B4%EB%93%9C-%EB%A7%B5%ED%95%91)
- [키 노테이션](https://hidekuma.github.io/vim/the-vim-key-notations/)

## Markdown

- [markdownguide.org](https://www.markdownguide.org/)

## 정규표현식

- [정규표현식 - 위키피디아](https://en.wikipedia.org/wiki/Regular_expression)
  - 여기에 문법이 잘 정리되어 있다.

## 협업 및 도구

- Trello
- Jira
- [기능명세서 작성 방법](https://velog.io/@pengoose_dev/%ED%94%84%EB%A6%AC%EC%BD%94%EC%8A%A4-%EA%B8%80%EC%93%B0%EA%B8%B0-1-%EA%B8%B0%EB%8A%A5%EB%AA%85%EC%84%B8%EC%84%9C)

## 개발 방법론

- 폭포수 방식
- DDD
- TDD
- BDD

<details>
<summary>기타</summary>

## 리팩터링/테스팅

코드를 쓰면서 들었던 리팩터링/테스팅에 관한 의문 또는 궁금했던 점, 알게 된 용어 등등을 모아보았습니다.

나름대로 내린 결론은, '더 유지보수하기 편한 쪽을 선택해라' 였습니다.

- [리팩토링](refactoring&testing/refactoring&testing.md#리팩터링)
- [테스팅](refactoring&testing/refactoring&testing.md#테스팅)

## 성장

- [지속 가능한 성장 스킬](https://f-lab.kr/blog/sustainable-developer-growth-skills)
- [개발자가 되고 싶은 이들이 자주하는 질문에 대한 이야기](https://catsbi.oopy.io/5d96b825-84ab-4419-9b03-720e7f591a29)

### 사이트

- [Stack Overflow](https://stackoverflow.com/)

### 사이트/테크 블로그

- [어썸 데브로그](https://github.com/awesome-devblog/awesome-devblog)
- [Incheol's TECH BLOG](https://incheol-jung.gitbook.io/docs/)
- [겔로그](https://velog.io/@gehwan96)
- [네이버 D2](https://d2.naver.com/home)
- [카카오 테크 블로그](https://tech.kakao.com/blog/)
- [JohnGrib's Wiki](https://johngrib.github.io/)
- [고퀄리티 개발 컨텐츠 모음](https://github.com/Integerous/goQuality-dev-contents)

### 부트캠프

- [삼성 SW 아카데미](https://www.ssafy.com/ksp/jsp/swp/swpMain.jsp)
- [우아한테크코스](https://techblog.woowahan.com/)

### 공채

- [카카오 영입 사이트](https://careers.kakao.com/index)
- [네이버 커리어 - 공채 사이트](https://recruit.navercorp.com/main.do)

### 강연

- [어느 날 고민 많은 주니어 개발자가 찾아왔다 - 인프콘 2022](https://www.youtube.com/watch?v=QHlyr8soUDM)
</section>
