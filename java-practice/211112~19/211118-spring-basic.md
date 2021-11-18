# Spring Framework란?
자바 플랫폼을 위한 오픈소스 애플리케이션 프레임워크로서 엔터프라이즈급 애플리케이션을 개발하기 위한 모든 기능을 종합적으로 제공하는 경량화된 솔루션입니다.

Spirng Framework는 경량 컨테이너로 자바 객체를 담고 직접 관리합니다. 객체의 생성 및 소멸 그리고 라이프 사이클을관리하며 언제든 Spring 컨테이너로 부터 필요한 객체를 가져와 사용할 수 있습니다.

# Spring Framework는 IOC기반이다. IOC란?

IOC는 Inversion of Control의 약자로 말 그대로 제어의 역전입니다. 그럼 제어의 역전이란 무엇일까요?     
일반적으로 지금까지 프로그램은
_객체 결정 및 생성 -> 의존성 객체 생성 -> 객채 내의 메소드 호출_ 하는 작업을 반복했습니다. 
이는 각 객체들이 프로그램의 흐름을 결정하고 각 객체를 구성하는 작업에 직접적으로 참여한 것입니다.

즉, 모든 작업을 사용자가 제어하는 구조인 것입니다.
하지만 IOC에서는 이 흐름의 구조를 바꿉니다. IOC에서의 객체는 자기가 사용할 객체를 선택하거나 생성하지 않는다.
또한 자신이 어디서 만들어지고 어떻게 사용되는지 또한 모릅니다. 자신의 모든 권한을 다른 대상에 위임함으로 써 제어권한을 위임받은 특별한 객체에 의해 결정되고 만들어집니다.

즉, _제어의 흐름을 사용자가 컨트롤 하지 않고 위임한 특별한 객체에 모든 것을 맡기는 것입니다_.

IOC란 기존 사용자가 모든 작업을 제어하던 것을 특별한 객체에 모든 것을 위임하여 객체의 생성부터 생명주기 등 모든 객체에 대한 제어권이 넘어 간 것을 IOC, 제어의 역전 이라고 합니다.

# IOC의 구성요소 DI와 DL?

### DL(Dependency Lookup) - 의존성 검색

컨테이너에서는 객체들을 관리하기 위해 별도의 저장소에 빈을 저장하는데 저장소에 저장되어 있는 개발자들이 컨테이너에서 제공하는 API 를 이용하여 사용하고자 하는 빈 을 검색하는 방법입니다.

### DI(Dependency Injection) - 의존성 주입 

의존성 주입이란 객체가 서로 의존하는 관계가 되게 의존성을 주입하는 것입니다. 객체지향 프로그램에서 의존성 이란 하나의 객체가 어떠한 다른 객체를 사용하고 있음을 의미합니다. 

그렇다면 IOC에서의 DI는 무엇일까요?
바로 각 클래스 사이에 필요로 하는 의존관계를 빈 설정 정보를 바탕으로 컨테이너가 자동으로 연결해 주는 것입니다.

# Spring Framework의 특징 AOP

_AOP_(Aspect Oriented Programming)란 말 그대로 관점 지향 프로그래밍입니다.
OOP는 객체지향 원칙에 따라 관심사가 같은 데이터를 한곳에 모아 분리하고 낮은 결합도를 갖게하여 독립적이고 유연한 모듈로 캡슐화를 하는 것을 일컫습니다. 하지만 이러한 과정 중 중복된 코드들이 많아지고 가독성, 확장성, 유지보수성을 떨어 뜨립니다. 이러한 문제를 보완하기 위해 나온 것이 AOP입니다.

AOP에서는 핵심기능과 공통기능을 분리시켜 핵심 로직에 영향을 끼치지 않게 공통기능을 끼워 넣는 개발 형태 이며 이렇게 개발함에 따라 무분별하게 중복되는 코드를 한 곳에 모아 중복 되는 코드를 제거 할 수 있어지고 공통기능을 한 곳에 보관함으로써 공통 기능 하나의 수정으로 모든 핵심기능들의 공통기능을 수정 할 수 있어 효율적인 유지보수가 가능하며 재활용성이 극대화됩니다.

# Spring Framework의 구조
 

### *Spring Core*

Spring Core는 Spring Container을 의미합니다. core라는 말 그대로 Container는 Spring Framework의 핵심이며 그중 핵심은 Bean Factory Container입니다.  그 이유는 바로 Bean Factory는 IOC패턴을 적용하여 객체 구성 부터 의존성 처리까지 모든 일을 처리하는 역할을 하고 있기 때문입니다.

### *Spring Context*

Spring context는 Spring Framework의 context 정보들을 제공하는 설정 파일입니다. Spring Context에는 JNDI, EJB, Validation, Scheduiling, Internaliztaion 등 엔터프라이즈 서비스들을 포함하고 있습니다.

### *Spring AOP*

Spring AOP module은 Spring Framework에서 관점지향 프로그래밍을 할 수 있고 AOP를 적용 할수 있게 도와주는 Module입니다. 해당 AOP에 대한 내용은 위에서 설명 했기 때문에 넘어 가도록 하겠습니다.

### *Spring DAO*

DAO란 Data Access Object의 약자로 Database Data에 접근하는 객체입니다. Spring JDBC DAO는 추상 레이어를 지원함으로써 코딩이나 예외처리 하는 부분을 간편화 시켜 일관된 방법으로 코드를 짤 수 있게 도와줍니다.

### *Spring ORM*

ORM이란 Object relational mapping의 약자로 간단하게 객체와의 관계 설정을 하는 것입니다. Spring에서는 Ibatis, Hibernate, JDO 등 인기있는 객체 관계형 도구(OR도구)를 사용 할 수 있도록 지원합니다.

### *Spring Web*

Spirng에서 Web context module은 Application module에 내장되어 있고 Web기반의 응용프로그램에 대한 Context를 제공하여 일반적인 Web Application 개발에 필요한 기본적인 기능을 지원합니다. 그로인해 Jakarta Structs 와의 통합을 지원하고 있습니다.

### *Spring MVC*

Spring에서는 MVC에서는 Model2 구조로 Apllication을 만들 수 있도록 지원합니다. MVC (Model-View-Controller) 프레임 워크는 웹 응용 프로그램을 작성하기위한 완전한 기능을 갖춘 MVC를 구현합니다. MVC 프레임 워크는 전략 인터페이스를 통해 고급 구성 가능하며 JSP, Velocity, Tiles, iText 및 POI를 포함한 수많은 뷰 기술을 지원하고 있습니다.


