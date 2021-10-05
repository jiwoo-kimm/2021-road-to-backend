# Spring Bean

> Spring IoC container에서 관리하는 객체

- configuration metadata를 바탕으로 생명주기와 상호 의존 관계가 설정된다.
- Scope가 따로 주어지지 않는 이상 기본적으로 Singleton으로 관리된다.
- container와 생명주기가 같다.

### Spring IoC container

> The `BeanFactory` provides the configuration framework and basic functionality, and the `ApplicationContext` adds more enterprise-specific functionality.


### Configuration Metadata

- `@Component`, `@ComponentScan`
- `@Configuration`, `@Bean`
- `AnnotationConfigApplicationContext` accepts annotated classes with `AnnotatedBeanDefinitionReader` and generate `BeanDefinition`
