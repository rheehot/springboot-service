# SpringBoot-Web
## - 교재 


<img src="./img/Book.jpg" width="400" height="600">

**스프링 부트와 AWS로 혼자 구현하는 웹 서비스 - 이동욱 지음**      


## 개발환경
 ---

| - |버전|
|---|---|
|운영체제|Window 10|
|개발 툴|IntelliJ|
|JDK|JDK 14|
|Gradle|4.10.2|
        * Gradle version downgrade
        p.74 http://bit.ly/382Q7d7
## DAY 1
---
- **Intellij로 프로젝트 만들기**
    - gradle project에서 springboot project로 변경하기 
- **Test code 작성하기**
    - TDD : 테스트가 주도하는 개발, 테스트 코드를 먼저 작성
        1. RED : 항상 실패하는 테스트 작성
        2. GREEN : 테스트가 통과하는 프로덕션 코드를 작성
        3. REFACTOR : 테스트가 통과하면 프로덕션 코드를 리팩토링 합니다.
    - 단위테스트 : 기능 단위의 테스트 코드를 작성

- **Test code를 작성해야하는 이유**
    - 단위 테스트는 **개발 단계 초기에 문제를 발견**
    - 단위 테스트는 개발자가 나중에 코드를 리팩토링하거나 라이브러리 업그레이드 등에서 **기존 기능이 올바르게 작동하는지 확인 가능** ex)회귀 테스트
    - 단위테스트 **기능에 대한 불확실성을 감소**
    - 단위테스트는 시스템에 대한 **실제 문서를 제공**, 단위 테스트 자체가 문서로 사용 가능 
- **Test code 작성 프레임워크**
    - xUnit , java => JUnit 

- **@SpringBootApplication**
    - 스프링 부트의 자동 설정, 스프링 Bean읽기와 생성 모두 자동으로 설정 
    - 시작 위치부터 설정을 읽어 가지 때문에 프로젝트의 최상단에 위치 
    - SpringApplication.run => 내장 WAS실행  
    
      => '언제 어디서나 같은 환경에서 스트링 부트를 배포' 
      
      => 서버에 톰캣을 설치할 필요가 없고 스프링 부트로 만들어진 JAR로 실행 
