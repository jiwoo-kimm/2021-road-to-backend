## Layered Architecture

- 소프트웨어 시스템을 계층화하여 복잡도와 관심사를 분리한다.
- 각 계층은 하나의 책임에만 집중함으로써 응집도는 높이고 상호 결합도는 낮춘다.
- 특히 Application Layer와 Domain Layer의 기술(How)에 관한 의존성을 최소화하여, 순수한 비즈니스 로직에 집중할 수 있도록 하는 것이 목표다.
- 상위 계층만 하위 계층의 공개 API에 접근하여 작업을 요청한다.

<br>

### Presentation Layer

- 유저(외부 행위자)와의 상호작용을 책임진다.
- 유저에게 정보를 보여 주고 요청을 해석한다.
- controller (REST API 정의)

<br>

### Application Layer

- 수행할 작업과 그 순서를 정의하며 계층 간 상호작용을 제어한다.
- 비즈니스 로직과 data access 로직이 포함되지 않으며, 하위 계층의 작업을 호출하여 orchestrate 한다.
- service (어플리케이션 행위 추상화)

<br>

### Domain Layer

- 핵심 비즈니스 로직을 표현한다.
- model, domain, entity, repository

<br>

### Infrastructure Layer

- 상위 계층의 역할을 기술적으로 지원한다.
- 변경·대체하기 쉬워야 한다.
- framework, database, email system, message queues, 기술 구현체

