# ***SpringFamework IOC Container***
> ***IOC (Inversion of Control) Container***  

_일반적으로 오브젝트의 생성과 관계설정,사용,제거 등의 작업은 애플리케이션 코드단에서 이루어진다._  
_하지만 스프링의 경우 이를 독립된 컨테이너가 담당하며, 컨테이터가 코드 대신 오브젝트에 대한 제어권을_  
_갖고 있다고 해서 IoC(제어의 역전)라고 부른다._  

> ***Spring IOC Container : BeanFactory, ApplicationContext***  

_IOC 컨테이너의 가장 기초적인 역활은 오브젝트를 생성하고 관리하는 것이며,_  
_스프링 컨테이너가 관리하는 오브젝트를 'bean'이라고 한다._  

_- BeanFactory : 오브젝트의 생성과 오브젝트 사이의 런타임 관계를 설정하는 DI관점에서의 컨테이너_  
_- ApplicationContext : BeanFactory + 엔터프라이즈 애플리케이션 개발을 위한 추가 기능_  

_일반적으로 스프링의 Ioc 컨테이너는 ApplicationContext를 지칭_  

> ***스프링 IOC 컨테이너의 필수요소 2가지***  

_- POJO 클래스 : 독립적설계, 유연한관계_  
_- 설정메타정보 : Ioc컨테이너와 POJO 클래스를 연결, 제어할 수 있는 정보_  
```
스프링의 메타정보는 특정한 파일 포맷이나 형식에 제한되거나 종속되지 않으며, BeanDefinition으로 정의되는
스프링의 설정 메타정보의 내용을 표현한 것이 있다면 무엇이든 사용가능하다.
Ex) Bean 메타정보 : id, class, scope, ref 등
```
