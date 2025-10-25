# Spring Framework

## What is Spring Framework?
 Spring Framework is a powerful, open-source **Java Framework** used to build **enterprise-grade application** - especially web and backend systems. \
 It provides a comprehensive infrastructure for developing Java applications efficiently and cleanly.

---

## Inversion of Contol (IOC)?
 Normally in programming, you control the flow of your application — you create objects, call their methods, and decide what happens next. \
 With IoC, that control is “inverted” — meaning the framework (Spring) controls the object creation and their lifecycle instead of you. \
 In short: 
 > IoC means you give up control of object creation and management to the Spring container.

--- 

## Dependency Injection (DI)?
 Dependency Injection is how IoC is actually implemented. \
 It means Spring automatically injects (provides) the required dependencies into a class, instead of you manually creating them.

### Types of DI
| Type | Example | Common Use|
| --- | --- | --- |
| Constructor Injection | `@Autowired public UserService(UserRepository repo)` | Preferred — safe for immutability and testing |
| Setter Injection | `@Autowired public void setRepo(UserRepository repo)` | When dependency is optional |
| Field Injection | `@Autowired private UserRepository repo;` | Simple, but less testable |

--- 

## Spring Beans
A Spring Bean is simply an object that is managed by the Spring IoC (Inversion of Control) container. \
In other words:
> Any class whose object is created, configured, and managed by Spring is called a Spring Bean.