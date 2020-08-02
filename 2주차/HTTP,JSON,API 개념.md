# HTTP, JSON, API 개념

# HTTP
**Hyper
Text
Transfer
Protocol**

**Hyper Text** : 참조를 통해 한 문서에서 관련된 다른 문서들로넘나들며 원하는 정보를 얻을 수 있게 해주는 텍스트 ex) 유튜브 

**Transter Protocol** : 인터넷을 통해서 정보를 주고받을 때 지켜야하는 규칙

**HTTP의 요청 메소드**

* **GET** URL에 표시된 리소스를 가져오기
* **POST** body에 정보를 담아 서버에 입력
* **PUT** URL에 표시된 리소스와 바꿔 치기
* **PATCH** PUT과 다르게 일부만 수정
* **DELETE** URL에 표시된 특정 리소스를 삭제

## JSON

**Java Script Object Notation** - Key : Value 형식을 갖고 있음. 데이터 교환 과정에서 사용한다!

**JSON의 특징**

* 기존 XML보다 가볍다. - JSON이 더 보편적이다!
* 많은 프로그래밍 언어가 지원한다.
* 전송 시 : 직렬화 과정을 거친다.
* 수신 시 : 역직렬화 과정을거친다.

## API

**Application Programming Interface**

Application(서비스)들이 제공해주는 데이터들에 접근하고 사용할 수 있도록 도와주는 도구 - TV의 리모콘 같은 존재!

**API의 종류**

* **SOAP** Simple Object Access Protocol
* **REST** Representational State Transfer

* **GraphQL** Graph Query Language

**REST**

REST는 하나의 아키텍쳐

소프트웨어 아키텍처 : 소프트웨어를 설계하는 지침과 원칙

물론 꼭 전부 다 지켜야 하는 법은 아니기 때문에 완전히 Restful한 API는 많지않다.

**REST의 구성요소**

* **자원** GET,PATCH 

* **행위** GET, PATCH

* **표현** JSON 형식으로 표현