# User

## User #1

**회원관리구현**

migrate를 통해서 user model 연동됨

------------------------
<br>

## User #2

**로그인과 로그아웃 구현**

* url 두번째 인자 **.as_view** : class를 url인자에서 직접적으로 실행시키기 위해 필요!

* import 하는것 잊지않기

* {% csrf_token %} : 토큰을 넣어서 보안에 신경쓰기

**overriding**

1. 위치를 간소화 하기 위해서 사용
ex) A파일을 B/C에 넣을 때 C만 기입하여 넣고싶을 때

2. 상속을 통해서 이루어짐

3. 바꾸고 싶은 항목에 대해서 새롭게 정의를 통해서 진행!