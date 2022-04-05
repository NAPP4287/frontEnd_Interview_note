# 기술 면접 인터뷰 준비하기

① 나만의 주의사항

```
- 공부하면서 필기 꼼꼼하게 🔥

- 틀린 필기는 최대한 빠르게 업데이트 🚀

- 실제 면접에서 답변하는 것처럼 깔끔하게 🧹
```

<br/>

② 목차

```
- Computer Science

- JavaScript

- React

- HTML

- CSS
```

<br/>
<br/>

### Computer Science

- `프로세스와 스레드 🔥`

  - 프로세스가 뭔가요?
    - 정적인 데이터 묶음, 즉 프로그램을 메모리에 적재되면 실행이 되는데, 이때 실행 중인 프로그램을 의미
    - 프로세스는 각각 독립된 메모리 영역(Code, Data, Stack, Heap의 구조)을 할당받는다.
  - 스레드가 뭔가요?
    - 프로세스 내에서 실제로 작업을 수행하는 주체
  - 프로세스와 스레드는 어떤 차이가 있나요?
    - 프로세스는 실행중인 프로그램을 뜻하고, 스레드는 그 프로세스 안에서 작업되는 무언가를 얘기한다.
    - ex) 프로세스 : 크롬, 스레드 : 크롬에서 유튜브를 시청, 게임 다운로드 등등

- `싱글 스레드와 멀티 스레드 🔥`

  - 싱글 스레드 장점
    - 공유자원을 접근하는 동기화 문제를 신경쓰지 않아도 된다.
    - context switch 작업을 요구하지 않아서, 전환 비용이 들지 않는다.
  - 싱글 스레드 단점
    - 여러 개의 작업을 실행해야할 때, 지연된다.
  - 멀티 스레드 장점
    - 프로세스의 자원과 상태를 공유하여 효율적으로 운영이 가능하다.
    - 새로운 프로세스를 생성하는 것보다 기존 프로세스에서 스레드를 생성하는 것이 빠르다.
  - 멀티 스레드 단점
    - 하나의 스레드만 실행중일 때는 실행시간이 오히려 지연될 수 있다.
    - 스레드 스케쥴링을 신경써야 한다.

- `HTTP 🔥`

  - HTTP란 뭔가요?
    - 텍스트 기반의 통신규약으로 인터넷에서 데이터를 주고 받을 수 있는 프로토콜이다.
  - HTTP 프로토콜의 가장 큰 특징은 뭔가요?
    - HTTP 메세지는 HTTP 서버와 HTTP 클라이언트로 의해 해석이 된다.
    - 클라이언트에서 요청을 보냈을 시, 서버는 그 요청에 알맞은 응답을 보낸다.
  - URL은 뭔가요?
  - HTTP/1.1 과 HTTP/2.0의 차이는 뭔가요?
  - HTTPS는 HTTP랑 뭐가 다른가요?
  - 심화) 공개키 (비대칭키) 방식이 뭔가요?

- `CI CD 🔥`

  - CI CD란 뭔가요?
    - CI는 Contiunous Integration의 약자로, 지속적 통합을 의미하는데, 프로그래머들이 각자가 만든 코드를 통합하는 단계를 말하기도 한다.
    - CD는 Continuous Deployment의 약자로, 지속적 배포를 의미한다. 소프트웨어를 코딩한 결과를 최종 사용자에게 실행 가능하도록 하는 단계를 말하기도 한다.

- `웹팩 🔥`

  - 웹팩이란?
    - 여러개로 나누어져 있는 파일들을 하나의 자바스크립트 코드로 압축하고 최적화하는 라이브러리
  - 모듈이란?
    - 개발하는 애플리케이션이 크기가 커지면서 확장성과 유지보수를 위하여 파일을 여러개로 분리해야하는데, 이 때 각 파일 하나하나를 모듈이라고 부른다.
    - 모듈은 보통 클래스 하나 혹은, 특정 목적을 가지는 복수의 함수 구성을 뜻하기도 한다.
  - 모듈 번들링이란?
    - 세분화 되어 분리된 모듈들을 묶어주는 것을 의미한다
  - 웹팩이 등장한 이유 웹팩 사용 시에 이점
    - 파일 단위의 모듈 관리 필요성
    - 애플리케이션의 빠른 로딩 속도와 높은 성능
  - 바벨이란?
    - 입력과 출력 모두 자바스크립트 코드인 컴파일러를 의미한다.
  - 웹팩의 주요 속성 4가지
    - Entry : 빌드를 할 대상 파일 정의
    - Output : 빌드를 한 후(=웹팩으로 변환 후)의 결과물에 대한 정보를 저장
    - Loader(모듈) : entry -> output 단계에서 개입
    - Plugins

- `타입과 인터페이스 🔥`
  - 타입스크립트를 왜 쓰나요? (본인이 느낀점)
    - 유연한 자바스크립트가 잡아내지 못 하는 에러를 타입스크립트에선 타입만 지정해주면 빠르게 확일 할 수 있기 때문에
  - 타입과 인터페이스의 차이를 아나요?
    - 타입은 선언 병합이 불가능하고, 인터페이스는 가능하다.
  - 프로젝트 진행 시에 어떤 상황에서 타입을 쓰고 어떤 상황에서 인터페이스를 썼나요?
    - 절대적으로 하나의 type만 존재해야할 때는 타입을 사용했지만, 인터페이스는 새로운 속성을 추가할 시, 편리하게 사용하였다.

<br/>
<br/>

### Javascript

- `프로그래밍 🔥`

  - 프로그래밍이란 뭐라고 생각하나요?
    - 특정목적을 위하여 컴퓨터가 처리하는 일 순서를 컴퓨터가 이해할 수 있는 언어로 작성하는 작업
  - 컴파일러는 뭐고 인터프리터는 뭔가요?
    - 프로그래밍 언어로 작성된 코드를 컴퓨터가 이해할 수 있게 컴퓨터 언어로 변환해주는 변환기
    - 컴파일러 : 작성된 프로그램 전체를 목적 프로그램으로 번역한 후, 링킹 작업을 통해 컴퓨터에서 실행 가능한 실행 프로그램을 생성
    - 인터프리터 : 작성된 프로그램을 한 줄 단위로 받아들여 번역하고, 번역과 동시에 프로그램을 한 줄 단위로 즉시 실행시키는 프로그램
  - 자바스크립트란 🔥
    - 웹페이지를 풍부하게 만들어주는 스크립트 혹은 프로그래밍 언어이다.
  - 자바스크립트의 특징은 뭐가 있나요?
    - 객체기반 언어이지만 상속과 클래스 개념은 존재하지 않는다.
    - 컴파일 과정이 없기 때문에 다른 언어들에 비해 빠른 시간안에 코드를 작성할 수 있다.
    - HTML문서 내에 기술되고 HTML 문서와 함께 수행된다.

- `변수 🔥`

  - 변수란 무엇인가요?
    - 하나의 값을 저장할 수 있는 저장공간을 변수라고 한다.
  - 식별자란 무엇인가요? fire
    - 자바스크립트에서 이름을 붙일 때 사용하는 단어
  - 변수를 선언한다는 것은 어떤 것을 의미하나요?
    - 저장공간이라는 변수에 이름을 붙임으로써 지정된 값을 대입해 주는 것을 의미한다.
  - var 키워드는 뭔가요?
    - 변수 중복 선언 허용
    - var 키워드 생략 허용
    - 함수 레벨 스코프로 인해 함수 외부에서 선언한 변수는 모두 전역 변수로 된다.
  - 호이스팅이 뭔가요? firefirefirefire
    - 변수 선언이 어디에 있든 상관없이 다른 코드보다 먼저 실행되는 특징을 호이스팅이라고 한다.
  - var, let, const 차이점
    - var vs let, const : 중복 선언이 불가능 하다 / 모든 코드 블록을 지역 스코프로 인정하는 블록 레벨 스코프를 따른다.
    - let vs const : let은 선언 단계와 초기화 단계가 분리되어 진행되지만 const는 동시에 진행된다.
  - TDZ firefirefire
    - 선언 단계와 초기화 단계 사이를 일시적 사각 지대라고 부른다.
  - 식별자 네이밍 규칙은 어떤 것들이 있나요?
    - 식별자는 특수문자를 제외한 문자, 숫자, 언더스코어(\_), 달러 기호($)를 포함할 수 있다.
    - 단, 식별자는 특수문자를 제외한 문자, 언더스코어(\_), 달러 기호($)로 시작해야 한다. (숫자 X)
    - 예약어는 식별자로 사용할 수 없다.
  - 네이밍 컨벤션은 어떤 것들이 있나요?
    - 하나 이상의 영어 단어로 구성된 식별자를 만들 때 가독성 좋게 단어를 한눈에 구분하기 위해 규정한 명명 규칙
    - Camel Case / Pascal Case
  - 리터럴이 뭔가요?
    - 데이터(값) 그 자체를 뜻한다. 즉, 변수에 넣는 변하지 않는 데이터를 의미
    - const a = 1일 때 1이 리터럴이다.

- `데이터 타입 🔥`

  - 데이터 타입의 종류는 어떤 것들이 있나요? fire
    - 기본형 : number, undefined, string, boolean, null 등
    - 참조형 : array, object, funtion, date 등
  - 심벌 타입은 뭐죠?
    - ES6에서 도입된 데이터 타입으로 변경 불가능한 원시 타입의 값
  - 데이터 타입은 왜 필요할까요? fire
    - 값을 저장할 때 확보해야 하는 메모리 공간의 크기를 결정하기 위해
    - 값을 참조할 때 한 번에 읽어 들여야 할 메모리 공간의 크기를 결정하기 위해
  - 정적 타이핑이 뭔가요?
    - 코드를 작성할 때 컴퓨터적 구조를 명시해주는 것을 정적 타이핑
  - 동적 타이핑이 뭔가요?
    - 따로 코드에 데이터 타입을 명시하지 않아도 컴퓨터가 알아서 해석하는 것을 동적 타이핑

- `타입변환과 단축 평가 🔥`

  - 명시적 타입 변환이 뭔가요?
    - 개발자가 의도적으로 데이터 타입을 바꾸는 것
  - 명시적 타입 변환 함수를 예를 들어볼 수 있나요?
    - toString(1) -> '1'
  - 암묵적 타입 변환이 뭔가요?
    - 자바스크립트 엔진이 자동으로 데이터 타입을 변환시키는 것
  - truthy / falsy 한 값이 뭔가요?
    - truthy : falsy한 값 그 이외의 것들
    - falsy : 0 / Nan / undefined / '' / null / false

- `배열 🔥`

  - 자바스크립트의 배열은 자료구조의 배열과 같나요?
    - 다르다. 엄연히 말하자면 자바스크립트의 배열은 일반적인 배열 동작을 흉내낸 특수 객체이다.
  - 배열의 메서드는 어떤 종류가 있나요?
    - pop, push, unshift, shift, splice, slice, concat 등등
  - 고차 함수에 대해서 아나요?
    - 함수를 인자로 전달 받거나, 함수를 반환하는 함수를 고차함수라고 한다.
  - forEach 메서드와 map메서드의 차이점에 대해 알고 있나요?
    - forEach : 배열의 요소마다 한 번씩 주어진 함수를 실행 시킨다.
    - map : 배열 내의 모든 요소 각각에 대하여 주어진 함수를 호출한 결과를 모아 새로운 배열을 반환한다.

- `객체 리터럴 🔥`

  - 자바스크립트에서 객체란 뭘까요?
    - key와 value로 구성된 property
  - 함수와 메서드의 차이점에 대해 알고 계신가요?
    - 함수는 메서드를 포함하는 개념이라고 볼 수 있다.
    - 메서드는 객체의 키값이 함수인 것을 메서드라고 한다.
  - 자바스크립트에서 객체를 생성하는 방법은 어떤 것들이 있나요?
    - 기본 객체의 생성자 함수 이용 : new Object()
    - 객체 리터럴 이용 : const test = {a : 1, b : 2}
    - 생성자 함수 이용 : 함수를 만들어서 this를 빈 객체에 바인딩하기

- `원시 값과 객체 비교 🔥`

  - 값에 의한 전달이 뭔가요?
    - 인수로 전달되는 변수가 가지고 있는 값을 함수 내의 매개변수에 복사하는 방식 (깊은 복사)
  - 참조에 의한 전달이 뭔가요?
    - 인수로 변수의 값을 전달하는 것이 아닌, 해당 변수의 주소값을 전달하는 방식 (얕은 복사)

- `함수 🔥`

  - 자바스크립트에서 함수를 정의하는 방법은 몇가지가 있나요?
    - 함수 선언식 / 함수 표현식
  - 함수 선언문과 함수 표현식은 어떤 차이가 있나요?
    - 함수 선언식은 호이스팅에 영향을 받지만, 함수 표현식은 호이스팅에 영향을 받지 않는다.

- `스코프 🔥`

  - 스코프가 뭔가요? firefirefire
    - 유효범위 : 어느 범위까지 참조 하는지를 뜻한다.
  - 스코프에는 어떤 종류가 있죠? firefire
    - 전역 스코프 : 스크립트 전체에 참조되는 것
    - 지역 스코프 : 정의된 함수 내에서만 참조 되는 것
  - 렉시컬 스코프를 아나요? 안다면 렉시컬 스코프는 무엇을 의미하나요? fire
    - 함수를 어디서 선언하였는지에 따라 상위 스코프를 결정하는 것
  - 전역 변수로 변수를 선언하면 생기는 문제점은 무엇이 있을까요?
    - 파일이 분리되어있다 하더라도 하나의 전역 스코프를 공유하기 때문에 다른 파일 내에서 동일한 전역 변수나 함수를 사용할 시, 예상치 못한 결과를 야기할 수 있다.

- `생성자 함수에 의한 객체 생성 🔥`

  - 생성자 함수가 뭔가요?
    - 객체를 생성하는 함수 -> new 연산자를 통해서 객체를 생성
  - 객체 리터럴로 만들 때와는 무슨 차이가 있죠? 왜 생성자 함수를 사용하나요?
    - 객체 리터럴은 본체에 필요한 물품을 끼워넣는 것
    - 생성자 함수는 같은 객체를 생성하기 위한 큰 틀 같은 것
    - 객체 리터럴과 달리 생성자 함수는 동일한 프로퍼티와 메소드를 가지는 객체를 생성할 때 유용하게 사용할 수 있기 때문에
  - 생성자 함수가 객체(인스턴스)를 생성하는 과정에 대해 간략하게 설명해줄 수 있나요?

    - const Car = (color) => {
      this.color = color;
      }

    const testCar = new Car('red');

- `함수와 일급 객체 🔥`

  - 일급 객체가 뭔가요?
    - 다른 객체들에 일반적으로 적용 가능한 연산을 모두 지원하는 객체
  - 자바스크립트에서 함수가 일급 객체라면, 일급 객체로 뭘 할 수 있나요?
    - 고차함수를 만들 수 있다.
    - 콜백을 할 수 있다.
  - 꼬리 질문) 함수형 프로그래밍이 뭔가요? firefire
    - 외부의 요인에 영향을 받지 않기 때문에 언제나 같은 아웃풋이 철저한 프로그래밍
  - 꼬리 질문) 순수 함수가 뭔가요? 일반 함수와는 어떤 차이가 있죠? firefire
    - 외부 요인에서부터 철저히 독립적인 성격 때문에 변질되는 것 없이 예상되는 값이 나오는 함수를 의미한다.
    - 일반 함수는 변이 되는 요인이 있을 때, 함수의 성질이 변질 될 수 있다.

- `프로토타입 🔥`

  - 객체지향 프로그래밍은 무엇을 의미하나요? fire
    - 프로그래밍에서 필요한 데이터를 추상화시켜 상태와 행위를 가진 객체를 만들고 그 객체들 간의 유기적인 상호작용을 통해 로직을 구성하는 프로그래밍 방법
    - 상태와 행위를 가진 객체들을 레고 블럭처럼 조립해서 하나의 프로그램을 만드는 것
  - 객체지향 프로그래밍의 특징에 대해 말해볼 수 있나요? fire
    - 추상화
    - 캡슐화
    - 상속
    - 다형성
  - 자바스크립트는 객체지향 프로그래밍 언어인가요?
    - 자바스크립트 객체를 생성하는 생성자 함수를 제공하고 있기 때문에 객체지향 프로그래밍 언어라고도 불리지만 정확히는 프로토타입 기반의 프로그래밍 언어라고들 많이 얘기한다.

- `strict mode 🔥`

  - strict mode가 뭔가요?
    - 엄격한 문법을 검사하는 것을 의미
  - strict mode를 통해 무엇을 예방할 수 있죠?
    - javascript에서 묵인했던 에러들을 엄격하게 다룸으로써, 세세한 에러들을 신경 쓸 수 있다.

- `빌트인 객체 🔥`

  - 빌트인 객체가 뭔가요? 종류는 어떤게 있죠?
    - 인스턴스를 생성할 수 있는 생성자 함수 객체 (Math, Reflect, JSON을 제외한 모든 객체)
    - Object, String, Number 등등 존재
  - 래퍼 객체에 대해서 알고 있나요?
    - 원시 타입의 프로퍼티에 접근하려고 할 때 생성되는 임시 객체

- `this 🔥`

  - this가 뭔가요? fire
    - javascript의 예약어로, 자신이 속한 객체 또는 자신이 생성할 인스턴스를 가리키는 자기 참조 변수
  - this 바인딩이란? fire
    - 식별자와 값을 연결하는 과정을 말하는데, this 바인딩은 this와 this가 가리키는 객체를 바인딩한다.
  - this는 동적으로 바인딩이 된다고 하는데 바인딩되는 객체가 어떻게 다르나요?
    - 컴파일시에 메모리를 할당하는 정적 바인딩과는 다르게 실행시에 메모리 할당을 한다.

- `실행 컨텍스트 🔥`

  - 실행 컨텍스트에 대해 말해보세요 firefire
    - 코드가 실행되기 위해 필요한 정보들을 가진 범위를 추상화하기 위해 객체 형태로 나타낸 것

- `클로저 🔥`

  - 클로저에 대해서 아나요? firefirefire
    - 내부함수가 외부함수 context에 접근할 수 있는 것을 의미한다.
  - 클로저를 사용하면 뭐가 좋죠? firefire
    - 함수가 종료될 시, 실행 컨텍스트 또한 종료되면서 정보에 접근할 수 없게 되는데 클로저를 사용했을 때 정보를 쉽게 접근할 수 있다.

- `클래스 🔥`

  - 자바스크립트에서 클래스가 생기기 전에는 어떤 방식으로 객체지향 패턴을 구현했나요?
    - 생성자 함수를 이용하였다.
  - 그럼 생성자 함수와 클래스는 어떤 차이가 있나요?
    - new와 함께 호출하지 않으면 반드시 에러가 발생한다.
    - 클래스는 항상 strict mode로 실행된다.
    - 클래스의 메소드는 열거할 수 없다.
  - 클래스 정의
    - 그냥 객체가 아닌, 특정 메소드나 데이터를 가지고 있는 청사진, 혹은 틀이다.
  - 클래스의 상속
    - extends 사용

- `스프레드 문법 🔥`

  - spread 문법이 뭔가요?
    - 하나로 뭉쳐 있는 여러 값들의 집합을 펼쳐서 개별적인 값들의 목록으로 만드는 것
  - 어떤 상황에서 사용할 수 있죠?
    - 함수 호출문의 인수 목록
    - 배열 리터럴의 요소 목록
    - 객체 리터럴의 프로퍼티 목록

- `구조 분해 할당 🔥`

- 구조 분해 할당이 뭔가요?
  - 배열이나 객체의 속성을 해체하여 그 값을 개별 변수에 담을 수 있게 하는 표현식
- 구조 분해 할당은 크게 어떤 종류가 있나요?

  - 객체에서의 구조 분해 할당
  - 배열에서의 구조 분해 할당

- `브라우저 렌더링 과정 🔥`

  - 브라우저의 렌더링 과정에 대해 설명해보세요 fire
    - 브라우저는 HTML, CSS, 자바스크립트, 이미지 폰트 파일 등 렌더링에 필요한 리소스를 요청하고 서버로부터 응답 받음
    - 브라우저의 렌더링 엔진은 서버로부터 응답된 HTML과 CSS를 파싱하여 DOM과 CSSOM을 생성하고 이들을 결합하여 렌더 트리를 생성
    - 브라우저의 자바스크립트 엔진은 서버로부터 응답된 자바스크립트를 파싱하여 AST를 생성하고 바이트코드로 변환하여 실행. 이때 자바스크립트는 DOM API를 통해 DOM이나 CSSOM을 변경할 수 있다. 변경된 DOM과 CSSOM은 다시 렌더 트리로 결합됨
    - 렌더 트리를 기반으로 HTML 요소의 레이아웃을 계산하고 브라우저의 화면에 HTML 요소를 페인팅
  - 브라우저의 렌더링 과정에 자바스크립트는 어떻게 동작하나요? fire
    - script 태그를 만나게 될 때에도 DOM 생성이 중단
    - 이후 서버에서 자바스크립트 파일을 응답 받으면, 자바스크립트 엔진에 제어권이 넘어감
    - 자바스크립트 엔진은 자바스크립트 파싱과 실행을 처리
    - 자바스크립트 코드를 해석하여 AST(Abstract Syntax Tree, 추상적 구문 트리)를 생성
    - 이후 AST를 바탕으로 바이트코드를 생성하고 실행
  - <script></script> 태그를 <body></body> 태그 밑에 둬야하는 이유가 있을까요?
    - HTML을 읽는 과정에 스크립트를 만나면 중단 시점이 생기고 그만큼 Display에 표시되는 것이 지연된다.
    - DOM 트리가 생성되기전에 자바스크립트가 생성되지도 않은 DOM의 조작을 시도할 수 있다.

- `DOM 🔥`

  - DOM이 뭔가요?
    - 웹브라우저가 html 문서를 인식하는 방식
    - HTML과 XML 문서에 접근하기 위한 인터페이스
  - DOM을 구성하는 건 뭐가 있나요?
    - HTML, Body, head, title 태그 등등

- `이벤트 🔥`

  - 마우스 이벤트 타입에는 뭐가 있나요? click 말고 클릭을 대체할 수 있는 이벤트가 있나요?
    - click, mousedown, mouseup, dbclick 등등
    - click 대신 mousedown 혹은 mouseup을 사용할 수 있다.
  - 그 외에 알고 있는 대표적인 이벤트가 있나요?
    - keydown : key를 눌렀을 때 발생
    - focus : 요소에 포커스가 이동되었을 때 발생
    - change : 요소의 값이 변경되었을 때 발생
    - scroll : 스크롤 바를 움직였을 때 발생
  - 이벤트 핸들러를 등록하는 방식에는 어떤 것들이 있나요?
    - HTML 요소의 속성으로 등록
    - DOM 요소 프로퍼티로 등록
    - addEventListener로 등록
  - 이벤트 전파(propagation)에 대해서 알고 있나요?
    - 이벤트가 호출되면 최상위 루트에서 자식 엘리멘트들을 타고 이벤트 타깃까지 내려가는 캡쳐 단계가 일어나고 다시 반대로 이벤트의 타킷으로부터 최상위 루트까지 올라가는 버블 단계가 일어난다.
  - 이벤트 위임(delegation)에 대해서 알고있나요? fire
    - 하위 요소마다 이벤트를 붙이지 않고 상위 요소에서 하위 요소의 이벤트들을 제어하는 방식
  - e.preventDefault 에 대해 알고 있나요?
    - 현재 이벤트의 기본 동작을 중단
  - e.stopPropagation
    - 현재 이벤트가 상위로 전파되지 않도록 중단

- `타이머 🔥`

  - 호출 스케쥴링이 무엇인가요?
    - 일정한 시간이 지난 후에 원하는 함수를 호출하는 것
  - 타이머 함수에는 어떤 것들이 있나요?
    - setTimeout : 지정한 시간 지난 후 지정한 함수 한번만 실행
    - clearTimeout : 반환받은 id 값을 이용하여 setTimeout을 취소
    - setInterval : 지정한 시간 간격을 두고 지정한 함수 계속 실행
    - clearInterval : 반환받은 id 값을 이용하여 setInterval을 취소
  - 이벤트가 과도하게 호출되어 성능에 문제를 일으킬 경우에 할 수 있는 어떤 일을 통해 해결할 수 있나요?
    - 디바운스
    - 쓰로틀
  - 디바운스에 대해서 알고 있나요?
    - 연속해서 발생하는 이벤트에 호출하지 않다가 일정 시간이 경과한 이후에 이벤트 핸들러가 한번만 호출되도록 한다.
  - 쓰로틀에 대해서 알고 있나요?
    - 짧은 시간 간격으로 이벤트가 연속해서 발생하더라도 일정 시간 간격으로 이벤트 핸들러가 최대 한 번만 호출되도록 한다.

- `비동기 프로그래밍 🔥`

  - 동기와 비동기의 차이점에 대해서 설명해줄 수 있나요? firefire
    - 동기는 순차적, 직렬적으로 테스크를 수행하고, 비동기는 병렬적으로 테스크를 수행한다.
  - 이벤트 루프와 태스크 큐에 대해서 알고 있나요? firefirefire
    - 이벤트 루프 : 여러 스레드가 사용되는 구동 환경이 자바스크립트 엔진과 연동하기 위해 사용되는 장치
    - 태스크 큐 : 컴퓨터의 기본적인 자료 구조 중 한 가지로, 먼저 집어 넣은 데이터가 먼저 나오는 FIFO(First In First Out) 구조로 저장하는 형식

- 마이크로태스크 큐에 대해서 알고 있나요? firefire

  - 비동기 함수가 실행되면, Web API가 호출된다. Web API는 비동기 함수의 콜백함수를 콜백큐에 넣는다. 비동기 콜백에 따라 Promise는 마이크로태스크 큐로, setTimeout은 태스크 큐로 가게된다. 이벤트 루프는 Call stack이 비어있는지 확인하고, 마이크로 태스크 큐에 가장 오래 담겨있던 콜백함수를 콜스택으로 보낸다. 콜스택이 비었다면 그 후에 태스크 큐를 확인하여 콜백함수를 콜스택으로 밀어넣는다.

- 태스크 큐와 마이크로태스크 큐 중 어떤 것이 먼저 실행되나요? firefire
  - 마이크로태스크 큐가 우선적으로 실행된다. (콜백함수는 setTimeout()의 콜백함수보다 먼저 처리된다.)

<br />

- `Ajax 🔥`

  - Ajax가 뭔가요 어떤 것을 담당하고 있죠?
    - javascript의 라이브러리 중 하나로, 비동기식 자바스크립트와 xml이라고 보면된다.
    - 클라이언트와 서버간에 XML 데이터를 주고받는 기술
  - Ajax를 사용하면 기존 방식과 어떤 차이가 있을까요?
    - 서버처리가 완료될 때까지 기다리지 않고 처리가 가능하다.
    - 비동기식 처리 방법
  - JSON 이 뭔가요?
    - Javascript Object National의 약자로 데이터를 저장하거나 전송할 때 사용하는 Data 교환 형식
  - JSON이 제공하는 정적 프로토타입 메서드에 대해 몇가지 말해볼 수 있나요?
    - null, number, string, array, object, boolean
  - Ajax로 HTTP 요청을 보내기 위해서는 어떤 방법을 사용할 수 있나요?
    - XMLHttpRequest, fetch
  - XMLHttpRequest와 fetch 메서드의 차이는 무엇이라고 생각하시나요? fire
    - promise 기반이냐 아니냐의 차이

- `REST API 🔥`

  - REST API가 뭔가요?
    - HTTP URI를 통해 자원을 명시하고, HTTP Method (POST, GET, PUT, DELETE)를 통해 해당 자원에 대한 CRUD OPERATION을 적용하는 것을 의미한다.
  - REST API의 구성은 어떤 것이 있나요?
    - URL
    - HTTP Method
    - Representations
  - HTTP 요청 메서드에 대해서 아는대로 얘기해보세요
    - GET
    - POST
    - PUT
    - DELETE
  - HTTP 상태 코드를 아는대로 말해주세요 fire
    - 2xx : 성공
    - 3xx : 리다이렉션
    - 4xx : 클라이언트 에러
    - 5xx : 서버 에러

- `Promise 🔥`

  - 콜백이란 뭐라고 생각하나요? fire
    - 다른 함수의 매개변수로 함수를 전달하고, 어떠한 이벤트가 발생한 후 매개변수로 전달한 함수가 다시 호출되는 것
  - 프로미스가 뭔가요? fire
    - 비동기 처리에 사용되는 객체
  - 프로미스 생성 방법
    - new Promise((resolve, reject) => {})
  - 프로미스의 상태를 나타내는 것은 어떤 것들이 있나요? fire
  - Pending
  - Fullfilled
  - Rejected
  - 프로미스 빌트인 객체가 제공하는 정적 메서드에 대해 알고 있나요? fire
    - promise.resolve
    - promise.reject
    - promise.all

- `제너레이터와 async await 🔥`

  - 제너레이터란 뭔가요? 일반 함수와는 어떤 차이가 있죠?
    - 제너레이터 함수는 중간에 원하는 부분을 멈추었다가 다시 실행할 수 있게 하는 함수
  - 제너레이터의 구조
  - async/await 가 뭔가요? 기존의 Promise와는 어떤 차이가 있죠? fire
  - Promise와 async/await의 차이점 한 줄 요약 fire

<br/>
<br/>

### React

- `리액트는 라이브러리인가요 프레임워크 인가요?🔥`

  - 리액트는 라이브러리이다.
  - 라이브러리 : 라이브러리를 가져다가 사용하고 호출하는 측에 주도권을 가지고 있는 것
  - 프레임워크 : 이미 만들어진 틀에 따라 개발자가 어플리케이션 코드를 짜게하는 것

- `리액트를 사용하는 이유🔥🔥`

  - component 단위 작성 : 컴포넌트는 개별적인 뷰 단위로써, 유지보수 및 재생산성이 용이하다.
  - JSX : javascript 확장 구문으로, HTML과 javascript 파일을 따로 관리하지 않아도 된다는 편의성을 가지고 있다.

- `virtual DOM에 대해서 아나요?🔥🔥`

  - DOM : HTML 혹은 XML을 파싱한 것으로 유저들에게 브라우저를 통해서 직접적으로 보여주는 화면을 제공하는 것이다.
  - virtual Dom : DOM이 생성되기 전, 이전 상태 값과 수정사항을 비교하여 달라진 부분만 DOM에게 한 번에 전달하여 딱 한 번만 렌더링 하는 것이다.

- `React에서 함수형 컴포넌트와 클래스형 컴포넌트의 차이 🔥`

- `props와 state의 차이🔥`

- `Props가 컴포넌트간에 전달받는 것이라고 했는데 자식에서 부모로도 전달할 수 있는가 🔥`

- `FLUX에 대해서 아나요? 🔥🔥`

- `리덕스에 대해서 아나요? 🔥🔥`

- `리덕스의 기본 원칙은? 🔥🔥`

- `React에서 state의 불변성을 유지하라는 말이 있는데 이에 대해 설명해달라 🔥`

- `리듀서 내부에서 불변성을 지키는 이유는? 전개 연산자의 단점을 해결할 수 있는 방법은 무엇인가 🔥`

- `리액트 사용시에 부수효과로 인해 생기는 문제점이 있다면 🔥🔥`

- `부수 효과를 일으키는 함수 (불순 함수)`
- `부수 효과를 일으키지 않는 함수 (순수 함수)`

- `컴포넌트의 라이프 사이클 메서드 🔥🔥`

- `Hooks의 종류 🔥🔥`

- `useState`
- `useEffect`
- `useReducer`
- `useMemo`
- `useCallback`
- `useRef`
- `커스텀 Hooks`
- `useMemo와 useCallback의 차이를 아나요 🔥🔥`

- `리액트에서 setState는 비동기 동작인가요 동기 동작인가요? 🔥`

- `setState가 비동기 동작을 취했을 때 얻을 수 있는 이점은 무엇인가요? 🔥`

- `useLayoutEffect는 무엇인가요? 🔥`

- `리액트의 성능개선 방법에 대해서 설명해주세요`

- `컴포넌트에서 이벤트를 실행시키기 위해서는 어떻게 핸들링해야 하나요?🔥`

- `SPA가 뭔가요?🔥`

- `SPA의 단점`
- `SSR이 뭔가요?🔥`

- `SEO가 뭔가요?🔥`

- `TTV, TTI`
- `하이드레이션에 대해 알고 있나요 🔥`

- `Next의 렌더링 수행 방식 🔥`

- `Next를 구성하는 기본 설정 파일에 대해서 알고 있나요? 🔥`

- `사전 렌더링을 위해 사용해 본 함수가 있나요 🔥`
