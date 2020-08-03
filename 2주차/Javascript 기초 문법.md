# Javascript 기초 문법

**참고**
* W3C School
* MDN Document
* 생활코딩 WEB2 - Javascript
* ofcourse

**Javascript**

* 웹페이지를 동적으로 만들 때 사용하는 언어

* 객체기반의 스크립트 언어

* 할 수 있는 일이 굉장히 많다

Browse API - DOM, 위치정보, audio, 화면공유 등 Browser 에서 제공하는 API들

2D, 3D 그래픽 작업 - NullSchool

클라이언트 뿐만 아니라 서버도 JS로 가능 - Node.js
 
* 스크립트 언어 + 인터프로터 방식 (파이썬과 동일)

입력 후 바로 결과 확인이 가능하다!

브라우저에 내장된 엔진으로 즉시 해석된다.

* **사용법 1**: HTML 내부에서 <스크립트> 태그내에 사용 

* **사용법 2**: js파일로 만들고 <스크립트 src = "파일경로">를 사용해서 불러오기

**변수**

* **사용가능한 데이터 타임** : Boolean, Null, Undefined, Number, String, Symbol, Object

* **var** : 권장하지 않는 변수 선언 방식

Hoisting

Function scope 변수

중복 선언 가능

예측하기 어려운 코드를 만들 수 있다.

* **let** : block scope 변수

* **const** : 변하지 않는 데이터를 저장

for in 문

for of 문

while 문

**조건문**

promt를 사용 = 사용자로 부터 input 받음

EX)
> let number = promt("점수를 입력하세요", 0);

if 문을 사용하여 조건을 부여하여 원하는 output 값을 얻음.

**DOM 다루기**

* DOM : Document Object Model

* 웹페이지에 접근 할 수 있게 해주는 일종의 인터페이스
* JavaScript와는 별개
* Javascript에 DOM을 조작할 수 있는 API가 존재

1. Node 선택하기
2. 속성 변경하기

* 함수 - 기본적인 형태

* 함수 - 익명함수

* 함수 - 화살표 함수 : function 대신에 화살표 추가