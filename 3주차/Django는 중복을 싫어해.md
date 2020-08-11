# Django는 중복을 싫어해

**URL Include**

App별로 URL을 관리할 수 있도록 구조화

**Template 상속**

* 맨 위에 {% extends 'base.html' %}

똑같은걸 반복해서 만들기 싫기 때문에 기본 틀은 그대로 만들어두고 거기에 main 콘텐트만 추가하는 형식

**{%block}, {%endblock%}**
: 블록 단위로 떼어온다고 생각하기