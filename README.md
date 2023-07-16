# Back-Interview
백엔드 면접 질문 정리

## 네트워크 / ETC

### HTTP와 HTTPS의 차이점은 무엇인가요?

- HTTP : Hyper Text Tranfer Protocol로, 인터넷에서 웹 페이지를 전송하는 데 사용되는 프로토콜입니다.
- HTTPS : HTTP의 보안 버전으로, 데이터를 암호화하여 안전한 통신을 제공합니다.

### 네트워크에서 TCP와 UDP의 차이점은 무엇인가요?

- TCP는 연결 지향적이고 신뢰성 있는 데이터 전송을 보장하는 프로토콜입니다. 느리지만 신뢰성이 필요한 애플리케이션에 적합합니다.
- UDP 비연결성 프로토콜로, 신속한 전송은 가능하나 신뢰성과 순서보장을 하지 않습니다.

### 세션과 쿠키의 차이점은 무엇인가요?

- 쿠키는 클라이언트 측에 저장되며, 보안에 취약
- 세션은 서버측에 저장되며, 보안적으로 더 안전

### 캐시의 동작원리를 설명해주세요

- 캐시는 빠른 데이터 액세스를 위해 사용되는 고속 저장 장치입니다.
- 주로 CPU와 주 메모리 사이에 위치하며, CPU가 데이터에 접근할 때 먼저 캐시를 확인 후 존재 하면 즉시 액세스하고 없는 경우 주메모리에서 가져와 캐시에 저장한 후 액세스

### 동기와 비동기 프로그래밍의 차이점은 무엇인가요?

- 동기 프로그래밍은 한 작업이 완료될 때까지 다음 작업이 기다려야하지만 비동기 프로그래밍은 한 작업이 완료되기를 기다리지 않고 다음 작업을 진행하는 방식입니다.

### 시간 복잡도와 공간 복잡도는 무엇인가요?

- 시간 복잡도 : 알고리즘의 실행 시간이 입력 크기에 따라 어떻게 증가하는지를 나타내는 것이고, 주로 Big O표기법으로 표현됩니다.
- 공간 복잡도 : 알고리즘이 실행되는 동안 필요한 메모리 공간의 양을 나타내며 마찬가지로 Big O표기법으로 표현됩니다.

### 스레드와 프로세스의 차이점은 무엇인가요?

- 프로세스는 운영체제로부터 자원을 할당받은 독립적인 실행단위 입니다. 각 프로세스는 독립된 주소 공간과 자원을 가지며, 다른 프로세스와는 별개로 실행됩니다.
- 스레드는 하나의 프로세스내에서 실행되는 여러 실행흐름으로, 주소 공간을 공유하고 자원을 공유할 수 있습니다. 프로세스의 자원을 공유하기 때문에 경량화되어 프로세스보다 빠른 실행이 가능합니다.

### 소프트웨어 개발 생명주기에 대해 설명해주세요

- SDLC는 소프트웨어 개발 과정을 단계적으로 관리하는 방법론입니다. 주요 단계로는 요구사항 분석, 설계, 개발, 테스트, 배포 및 유지보수가 있습니다. 이 방법론은 소프트웨어 프로젝트를 계획하고 추진하기 위해 표준화된 절차를 제공하며, 품질 관리와 개발자들 간의 협업을 원할하게 합니다.

### 데드락이란 무엇이고 어떤 상황에서 발생할 수 있나요?

- 데드락은 여러 프로세스나 스레드가 서로가 점유한 자원을 기다리며 무한히 대기하는 상태를 말합니다.
- 데드락은 네가지 필요 조건이 동시에 충족할때 발생합니다. 이 조건은 상호 배제, 점유 대기, 비선점, 순환 대기 입니다. 이 조건들이 동시에 충족되면 프로세스나 스레드들이 락이나 자원을 무한히 대기하며, 시스템의 작업을 진행할 수 없게 됩니다.

### 클라우드란?

- 인터넷을 통해 서버, 데이터베이스, 저장소, 소프트웨어 등의 컴퓨팅 서비스를 제공하는 기술입니다.
- 필요한 컴퓨팅 리소스를 필요한 만큼 확장하거나 축소할 수 있는 유연성을 제공합니다.

### 스프링과 장고의 장단점

- 스프링 : 대규모 애플리케이션 개발에 많이 사용되고 다양한 모듈과 라이브러리가 개발되어있습니다.
- 장고 : 신속한 개발과 간편한 사용성을 강조합니다.

### 스케일 업과 스케일 아웃의 차이점은 무엇인가요?
- 스케일 업은 단일 서버 또는 시스템의 성능을 향상시키기 위해 해당 서버의 하드웨어 성능을 업그레이드 하는 방식입니다. 스케일 아웃은 성능을 향상시키기 위해 여러 서버 또는 시스템을 추가하는 방법입니다. 스케일 업은 단일 서버 내에서 성능을 향상시키는 반면, 스케일 아웃은 여러 서버를 활용하여 성능을 분산 시키는 차이가 있습니다.

### 머신러닝과 딥러닝의 차이점은 무엇인가요?
- 머신러닝 : 인공지능의 한 분야로, 데이터 기반으로 모델을 학습하고 예측, 분류 패턴 인식등을 수행하는 방법입니다.
  - 머신 러닝은 주어진 데이터에서 통계적 학습 알고리즘을 사용하여 모델을 학습하고 결과를 도출합니다.
- 딥러닝 : 인공 신경망을 기반으로 한 머신 러닝의 한분야입니다.
  - 딥러닝은 복잡한 계층 구조의 신경망을 사용하여 데이터로부터 특징을 추출하고 모델을 학습합니다.

### 웹 서버와 애플리케이션 서버의 차이점은 무엇인가요?
- 웹 서버 : 클라이언트로 부터 HTTP 요청을 받아 정적인 웹 페이지를 제공하는 서버입니다. 동적인 처리가 필요한 경우에는 애플리케이션 서버에 요청을 전달합니다.
- 애플리케이션 서버 : 웹 서버와 연동하여 동적인 콘텐츠를 생성하고 전달합니다. 웹 서버와 애플리케이션 서버는 보통 협업하여 웹 어플리케이션을 구성합니다.

## Java

### 자료구조와 알고리즘에 대한 설명

- 자료구조 : 데이터를 구조화하고 저장하는 방식을 의미합니다.
     - Ex ) 배열, 리스트, 스택, 큐 등
- 알고리즘 : 문제를 해결하기 위한 절차나 방법
     - Ex ) 정렬, 검색, 그래프 탐색 알고리즘 등

### 알고리즘의 최선, 평균, 최악 시간 복잡도는 무엇인가요?
- 소요되는 시간의 상한을 나타냅니다.
- 최선은 가장 빠르게, 최악은 가장 느리게, 평균은 입력 데이터의 분포나 특성을 고려하여 예측된 평균 실행 시간을 나타냅니다.

### 스택과 큐의 차이점

- 스택(Stack / LIFO) : 후입선출의 데이터 구조로 데이터를 삽입과 삭제할 때 상단에서 이루어집니다.
- 큐(Queue / FIFO) : 선입선출의 데이터 구조로, 데이터를 삽입하고 삭제할 때 앞에서 이루어집니다.

### 정적 바인딩과 동적 바인딩의 차이점은 무엇인가요?

- 정적 바인딩 : 컴파일 시간에 메서드나 함수의 호출이 어떤 코드와 연결될지 결정되는 방인딩 방식입니다.
- 동적 바인딩 : 실행 시간에 메서드나 함수의 호출이 어떤 코드와 연결될지 결정되는 바인딩 방식입니다.

### 객체

- 객체 지향 프로그래밍의 가장 기본적인 단위이자 시작점이다.
- 우리 주변에서 흔히 볼 수 있는 모든 실재하는 대상을 객체라고 한다.
- 눈에 보이는 유형의 대상뿐 아니라 보이지 않는 논리, 사상, 철학, 개념, 공식 등 무형의 대상들도 포함될 수 있다

### 클래스와 객체의 차이점

- 클래스 : 객체를 만들어내기위한 설계도
- 객체 : 클래스의 인스턴스로 클래스에 정의된 속성과 동작을 가지고 있습니다.

### 객체지향 프로그래밍의 특징

- Object-Oriented Programming(OOP)
- 객체들의 유기적인 협력과 결합으로 파악하고자 하는 컴퓨터 프로그래밍의 패러다임
- 프로그램들을 독립적인 객체들의 집합으로 구성하는 방법론. 각각의 객체는 상태와 행동을 가지며, 상호작용하면서 프로그램이 동작
- 4가지 특징
    - 추상화 : 중복되는 코드를 제외하고 단일 객체에 정의함으로써 코드를 고도화하는것, 객체의 속성중 중요한 부분에 중점을 두어 개략화 하는것
    - 상속 : 기존의 클래스를 재활용하여 새로운 클래스를 작성하는 자바의 문법요소
    - 캡슐화 : 서로 연관있는 속성과 기능들을 하나의 캡슐로 만들어 데이터를 외부로부터 보호하는것 (접근제어자, getter/setter)
    - 다형성 : 어떤 객체의 속성이나 기능이 그 맥락에 따라 다른 역할을 수행할 수 있는 객체 지향의 특성(오버라이딩, 오버로딩)

### JVM의 구조와 Java의 실행방식

- 구조
    - 클래스로더
    - 실행 엔진
    - 런타임 데이터 에어리어
    - JNI + Native Method Library

- 실행 방식
    - 자바 컴파일러가 .java 코드를 읽어 .class로 변환
    - 클래스 로더를 통해 JVM으로 로딩
    - 실행 엔진을 통해 해석
    - Runtime data area에 배치되어 실질적 수행

### GC

- 가비지 컬렉션은 프로그램에서 더 이상 사용되지 않는 동적으로 할당된 메모리를 자동으로 해제하는 메모리 관리 기법

### 컬렉션 프레임워크

- 객체, 데이터들을 효율적으로 관리 할 수 있는 자료구조들이 있는 라이브러리

- Collection 인터페이스 
    - List 인터페이스 : 순서가 있는 집합 자료구조로 데이터의 중복을 허용 ( 순서 O, 중복 O )
    - Set 인터페이스 : 순서가 없는 집합 자료구조로 데이터의 중복을 허용하지 않습니다. ( 순서 x, 중복 X )
- Map 인터페이스 : 키와 값의 한쌍으로 이루어지는 데이터의 집합으로, 순서가 없으며 키는 중복을 허용하지 않지만, 값은 중복을 허용

### 어노테이션

- 인터페이스를 기반으로 한 문법, 주석처럼 코드에 달아 클래스에 특별한 의미를 부여하거나 기능을 주입

### 오버라이딩, 오버로딩의 차이

- 오버라이딩은 상위 클래스의 메서드를 재정의
- 오버로딩은 같은 클래스 내의 동일한 이름을 가진 메서드가 매개변수의 타입, 개수가 다르게 구현할 수 있는것

### 인터페이스, 추상클래스

- 추상클래스는 객체의 추상적인 상위 개념으로 공통된 개념을 표현할 때 사용, 단일 상속만 가능
- 인터페이스는 구현 객체가 같은 동작을 한다는 것을 보장하기 위해 사용, 다중 상속 가능

### 동일성, 동등성 차이점

- 동일성 : 객체의 주소를 비교하는것
- 동등성 : 객체의 같음을 비교하는것

### 원시타입, 참조타입

- 원시타입은 Java에서 단 8개밖에 존재하지 않는 타입.
    - boolean(1byte), byte(1byte), char(2byte), short(2byte), int(4byte), float(4byte), long(8byte), double(8byte)
- 원시타입 외 모든 타입, Object 클래스 이거나 이를 상속하는 클래스

### Java8에서 추가된 기능

- Lambda(함수형 프로그래밍 지원), Stream(고차함수 지원), Optional(null-safety제공, stream과 유사) 등이 추가


### Generic<T>

- 클래스나 메서드에서 사용할 내부 데이터 타입을 컴파일 시에 미리 지정하는 방법입니다. ( 데이터 타입 일반화 )
- 클래스나 메서드에서 사용되는 객체의 타입 안정성을 높일 수 있습니다.
- 반환값에 대한 타입 변환 및 타입검사에 들어가는 노력을 줄일 수 있습니다.

### Static(정적)

- 정적(static)은 고정된이란 의미를 가지고 있습니다.
- static 키워드를 사용하여 static변수와 static메소드를 만들 수 있는데, 정적필드와 정적 메소드라고도 하며 이 둘을 합쳐 정적 멤버(클래스 멤버)라고 합니다.
- Java에서 Static 키워드를 사용한다는 것은 메모리에 한번 할당되어 프로그램이 종료될 때 해제

### RESTful API란 무엇인가요? 

- 웹 기반 소프트웨어 아키텍쳐 스타일중 하나
- 이를 준수하는 API는 자원을 고유한 URI로 표현하고 HTTP메서드(GET,DELETE,PUT,POST 등)를 사용하여 해당 자원에 대한 조작을 수행합니다.

### 디자인 패턴

- 프로그램을 설계할때 발생했던 문제점들을 객체 간 상호관계 등을 통해 해결할 수 있도록 하나의 '규약'형태로 만들어 놓은 것
 
### 싱글톤 패턴란 무엇인가요? 

- 하나의 클래스에 오직 하나의 객체 인스턴스만 가지는 디자인 패턴, 해당 인스턴스를 다른 모듈들이 어디에서든 공유하며 접근, 사용할 수 있다.  
- 싱글톤 패턴으로 만들어진 클래스는 생성자가 여러번 호출 되더라도, 실제로 생성되는 객체는 하나이고 최초 생성 이후에 호출된 생성자는 최초의 생성자가 생성한 객체를 보낸다. ( static 사용하여 별도의 메모리 영역 얻고, 한 번의 new 연산자로 인스턴스 사용 )
- 주로 공통된 객체를 여러 개 생성해서 사용하는 DBCP (Database Connection Pool)와 같은 데이터베이스 연결 모듈에 많이 사용된다.
  
  - 장점 : 메모리 낭비를 방지, 전역 인스턴스이기 때문에 다른 클래스의 인스턴스들이 데이터를 공유할 수 있다.
  - 단점 : 객체간의 독립성을 지향하는 객체지향 원칙에 위배, 멀티스레드 환경에서 객체가 1개이상 생성되어 오류 발생의 여지가 있음.
    - 싱글톤 인스턴스를 여러곳에서 많이 공유할 경우 다른 클래스의 인스턴스 간 의존성이 높아질 수 있다 -> 수정작업이나 테스트를 진행하기 어려움

----------------------------------------------------------------------------

## Spring

### Spring과 SpringBoot의 차이점
- 스프링(Spring) : 프레임워크
  - 설정 파일을 직접 작성하여 스프링 컨테이너를 구성, 필요한 빈 객체를 등록, 빈 객체 간의 의존성을 설정
  - 스프링 프레임워크를 보다 세밀하게 제어하고자 하는 경우에 사용
- 스프링 부트(Spring Boot) : 스프링 프레임워크를 기반으로 한 도구입니다.
  - Spring에서 제공하는 여러 기능들을 자동으로 설정하여 개발자가 보다 쉽게 사용할 수 있도록 해줍니다.
  - 스프링 MVC, Spring Data JPA, Spring Security 등의 기능을 자동으로 설정하며, 개발자가 별도로 설정 파일을 작성하지 않아도 사용
  - 내장 서버를 제공하여 쉽게 웹 애플리케이션을 실행
  - 빠르고 간단하게 스프링 애플리케이션을 개발하고자 하는 경우에 사용

### IOC

- 제어의 역전, 프로그램의 제어 흐름을 개발자가 제어하는것이 아닌 스프링에게 위임하는것

### DI

- 의존관계 주입, IOC의 형태로 클래스 사이의 의존관계를 빈 설정 정보를 바탕으로 컨테이너가 자동 연결하는것

### Bean

- IOC 컨테이너안에 들어있는 객체, 필요할 때 IOC 컨테이너에서 가져와 사용 @Bean으로 설정가능

### IOC 컨테이너의 역할

- 어플리케이션 실행 시점에 빈 오브젝트를 인스턴스화 하고 DI 한 후에 최초로 어플리케이션을 기동할 빈 하나를 제공

### DI의 종류

- 생성자 : 생성자 호출 시점에 딱 한번만 호출, 불변, 필수 의존관계에 사용
- Setter : 선택, 변경 가능성이 있는 의존관계에 사용, 스프링 빈을 선택적으로 등록 가능
- 필드 주입 : @Autowired 를 사용, 외부에서 변경이 불가하여 테스트 하기 힘들며, DI프레임워크 없이는 작동하기 힘들다

### MVC 패턴

- 디자인패턴, Model, View, Controller 3가지로 나누어 역할을 분리후 처리하는 패턴
- 하나의 어플리케이션, 프로젝트를 구성할 때 그 구성요소를 세가지 역할로 구분한 디자인 패턴
- 장점 : 유지보수에 유리하고, 애플리케이션의 확장성, 그리고 유연성이 증가하며, 중복코딩이라는 문제점 또한 사라지게 됨

    - Model
        - 어플리케이션의 정보, 모든 데이터 정보를 가공하여 가지고 있는 컴포넌트
        - 데이터 베이스, 처음에 정의하는 상수, 초기화 값, 변수 등을 뜻합니다.
        - View, Controller에 대한 정보를 알면 안됨
    - View
        - input 텍스트, 체크박스 항목 등과 같은 사용자 인터페이스 요소
        - 데이터 및 객체의 입력, 보여주는 출력을 담당, 데이터 기반으로 사용자들이 볼 수 있는 시각적인 UI 요소
        - Model, Controller에 대한 정보를 알면 안되며 단순히 표시하는 역할
    - Controller
        - 데이터(Model)와 사용자 인터페이스 요소(View)들을 잇는 다리역할
        - 사용자가 데이터를 클릭하고, 수정하는 것에 대한 이벤트들을 처리하는 부분을 뜻한다.

### VO

- Value Object의 줄임말로, 값을 가지고 있는 객체입니다.
- 비즈니스 값을 가져올때 사용하며, 보통 값을 수정할 수 없는것으로 합니다. DTO와 혼용해서 사용하기도 합니다.

### DTO

- Data Transfer Object의 줄임말로, VO와같이 값을 가지고 있는 객체입니다.
- VO와 차이점은 DB로 치자면 하나의 인스턴스로, 데이터 핸들링에 사용되는 객체입니다. DTO를 통해 데이터를 전달할 수 있습니다.

### DAO

- Data Access Object의 줄임말로, 실제 데이터베이스에 접속하는 객체입니다.

### AOP

- Aspect Oriented Programming, 관점 지향 프로그래밍
- 스프링 프레임워크의 핵심요소중 하나로, 비즈니스 로직과 공동 모듈을 분리하고, 핵심로직 사이사이에 공동모듈을 잘 끼워넣는것을 말합니다.
- 이때 공동모듈을 코드 밖에서 설정된다는것이 핵심입니다. 인증, 로깅, 트랜잭션 처리에 용의합니다.
- Ex ) 팩토리얼

### Intercepter, Filter

- 공통점은 Controller가 호출되기 전에 실행됩니다.
- 차이점은 Filter는 dispatcher가 호출되기 전에, Intercepter는 dispatcher가 호출되고 난 이후에 호출됩니다.
    - 인코딩이나 보안같은 WebApp에 전역적으로 처리해야 할 경우 Filter를 사용합니다.
    - 클리이언트의 요청에 따른 인증, 권한등의 디테일한 처리는 Intercepter에서 처리 합니다.

-----------------------------------------------------------------------------------------------------

## JPA

### Entity

- 실제 데이터베이스의 테이블과 1대1로 맵핑되는 클래스

### N+1 문제

- 1번의 쿼리를 날렸을 때 의도하지 않은 N번의 쿼리가 추가적으로 실행되는 것을 의미한다.
- Lazy로딩에 의해 한번에 모든 정보를 가져오지 않아서 발생하는 문제, 패치 조인을 사용해서 해결할 수 있다

### JPA 영속성 컨텍스트의 이점

- 영속성 컨텍스트는 엔티티를 영구 저장하는 환경을 의미합니다
- 1차캐시 : 조회가 가능하며, 1차캐시에 없으면 DB에서 조회하여 1차캐시에 올려놓습니다.
- 동일성 보장 : 동일성 비교가 가능합니다.(==)
- 쓰기 지연 : 트랜잭션을 지원하는 쓰기지연이 가능하며, 트랜잭션을 커밋하기 전까지 SQL을 바로 보내지 않고 모아서 보낼수 있습니다.
- 변경감지 : 스냅샷을 1차캐시에 들어온 데이터를 찍습니다. 커밋되는 시점에 Entity와 스냅샷을 비교하여 update SQL을 생성합니다.
- 지연로딩 : Entity에서 해당 Entity를 불러올때 SQL을 날려 해당 데이터를 가져옵니다.

### JPA와 Mybatis의 차이
- JPA : 코드의 가독성과 유지보수성을 높일 수 있으나, 복잡한 쿼리작성에는 알맞지 않을 수 있습니다.
- MyBatis : 수동적으로 쿼리문을 작성하지만 오타로 인한 문제가 있을 수 있습니다.


-----------------------------------------------------------------------------------------------------------------

## DB

### 트랜잭션

- 데이터베이스에서 수행되는 하나의 독립적인 단위
- 트랜잭션 하나가 전부 반영되던지 아예 반영이 안되던지 둘 중 하나

### index

- 데이터베이스 검색 속도 향샹을 위한 자료구조

### SQL과 NoSQL의 차이점
- SQL : 관계형 데이터베이스 시스템을 위한 언어로, 테이블과 스키마를 기반으로 데이터를 저장하고 관리합니다.
- NoSQL : 비 관계형 데이터베이스 시스템을 위한 개념으로, 유연한 스키마 구조를 가지며 확장성과 성능을 강조합니다.

### JOIN에 대해 아는것을 서술하세요
- 관계형 데이터베이스의 테이블 안에 있는 행들을 논리에 따라 연결할 수 있도록 하는 기법
- 데이터베이스에 저장 되어있는 데이터들은 각 테이블안에 흩어져 저장되어 있으므로, 사용자 원하는 형태로 데이터를 조작하려면 조인이 필요합니다.

### INNER JOIN(내부조인)

- 여러 애플리케이션에서 사용되는 가장 흔한 결합 방식이며 기본 조인 형식으로 간주됩니다 (INNER는 생략가능).
- 테이블 사이에 열거하는 모든 조건이 일치하는 결과 집합을 반환합니다.

### OUTER JOIN(외부조인)

- INNER JOIN이 모든조건을 만족하는 조합만을 조회한다면, OUTER JOIN은 컬럼 값이 NULL등 알 수 없는 경우에도 결과 집합을 조회 합니다.
- 조회 결과의 중심을 어디에 두느냐에 따라서 LEFT OUTER, RIGHT OUTER, FULL OUTER JOIN으로 나눌수 있습니다.

    - LEFT OUTER JOIN
        - 조인문 왼쪽에 있는 테이블의 모든 결과를 가져온 후 오른쪽의 테이블 데이터를 매칭, 매칭되는 데이터가 없을 경우 NULL값으로 표시합니다.

    - RIGHT OUTER JOIN
        - 조인문 오른쪽에 있는 테이블의 모든 결과를 가져온 후 왼쪽의 테이블 데이터를 매칭, 매칭되는 데이터가 없을 경우 NULL값으로 표시합니다.

    - FULL OUTER JOIN
        - LEFT OUTER JOIN과 RIGHT OUTER JOIN을 합친것으로, 양쪽 모두 조건이 일치하지 않는 데이터까지 모두 출력합니다.
 
### Q. TO_CHAR

### A. 오라클에서 쿼리문을 작성할 때 날짜, 숫자등의 값을 문자열로 반환

- 날짜 포맷 변경 : SELECT TO_CHAR(SYSDATE, 'YYYY-MM-DD') - 2023-06-23
  
- 소수점 변경 : SELECT TO_CHAR(123.456, 'FM990.999') - 123.456
                   SELECT TO_CHAR(0.12345, 'FM9990.99') - 0.12
  - FM : 문자열의 공백제거 숫자의 최대 길이만큼 9999. 형식을 지정합니다 (9 : 값이 없으면 표시안함, 0: 값이 없으면 "0"으로 처리)
          정수은 지정한 형식보다 값의 길이가 길면 오류, 소수 지정한 길이보다 길면 반올림
  
- 숫자의 천단위 콤마 찍기 : SELECT TO_CHAR(12367, 'FM999,999') - 123,467
                              SELECT TO_CHAR(123467, 'FML999,999') - ￦123,467

- 지정한 길이만큼 0으로 채우기 : SELECT TO_CHAR(123) - 123
                                   SELECT TO_CHAR(123, 'FM00000') - 00123

- 날짜에 0 없애기 : SELECT TO_CHAR(SYSDATE, 'MM/DD') - 06/23 (날짜 포맷 변경)
                      SELECT TO_CHAR(SYSDATE, 'FMMM/DD') - 6/23

- 임의의 구분자로 날짜형식 만들기 : SELECT TO_CHAR('""YYYY"년 "MM"월 "DD"일"') - 2023년 06월 23일
                                      SELECT TO_CHAR('""HH24"시 "MI"분 "SS"초"') - 12시 27분 32초

- 시간의 오전, 오후값 반환 : SELECT TO_CHAR(SYSDATE, 'AM') - 오전
                               SELECT TO_CHAR(SYSDATE, 'AM HH:MI:SS') - 오전 12시 30분 20초

- 날짜의 요일 반환 : SELECT TO_CHAR(SYSDATE, 'D') - 6 (1(일)~7(토))
                       SELECT TO_CHAR(SYSDATE, 'DY') - 금
                       SELECT TO_CHAR(SYSDATE, 'DAY') - 금요일

- 1년기준 몇일, 몇주 분기 반환 : SELECT TO_CHAR(SYSDATE, 'DDD') - 174 (365일 기준 몇일)
                                   SELECT TO_CHAR(SYSDATE, 'WW') - 25 (1년(52주)기준 몇주)
                                   SELECT TO_CHAR(SYSDATE, 'Q') - 2 (몇분기)

- 간편한 날짜 변환 : SELECT TO_CHAR(SYSDATE, 'MON') - 6월
                         SELECT TO_CHAR(SYSDATE, 'DL') - 2023년 6월 23일 금요일

### DECODE

- 프로그래밍의 IF-ELSE 논리를 제한적으로 구현한 DBMS 메서드
  - DECODE(컬럼, 조건1, 결과1, 조건2, 결과2... ,'DEFAULT_RESULT');

### 다양한 DBMS의 종류와 그들에 장단점

- 관계형 데이터베이스의 장점은 데이터의 일관성과 무결성을 보장,복잡한 쿼리 및 다양한 조인연산을 지원하고, 대용량 데이터 처리와 안정성에 강점을 가지고 있습니다.
  - 단점은 수직적 확장에 한계가 있으며, 대규모 분산 시스템에는 부적합할 수 있습니다. 스키마 변경이 번거로울 수 있습니다.
- NoSQL 데이터베이스의 장점으로는 확장성이 뛰어나고 수평적 확장을 지원합니다. 유연한 데이터 모델과 스키마가 없는 구조로 데이터를 저장, 대용량 데이터 처리와 높은 읽기/쓰기 처리량을 제공합니다.
  - 단점으로는 데이터의 일관성을 보장하기 힘듭니다. 다양한 쿼리 자원이 부족할 수 있습니다.
