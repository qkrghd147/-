# Fetch API

**비동기 처리**

* 들어온 요청들을 순차적으로 실행한다면?

앞에 들어온 작업이 시간이 오래 걸리는 작업일 시 뒤에 있는 작업들이 밀리게 된다.

이런 작업들을 그대로실행시키면서 뒤에 있는 코드를을 실행시키는 것이 바로 비동기처리이다!

**promise 객체를 사용한다.**

아래의 세가지 상태를 가진다.
* 대기
* 이행
* 거부

**비동기 호출 - keyword**

두 가지 패턴이 존재한다.

* async, await 키워드를 활용한

async function

 asyncFunction(){await [Promise객체]}

* [promise객체]

.then(콜백함수)

.catch(콜백함수)

**Fetch API**

* Fetch API는 네트워크 통신을 위해서 제공되는 API이다. - Postman과 똑같다 생각

* Promise 객체를 반환한다.

* Requeset, Response라는 두 개의 객체를 사용한다.
