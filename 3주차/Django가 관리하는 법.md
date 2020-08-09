# Django가 관리하는 법

**Bootstrap**

Front-End개발을 빠르고 쉽게 할 수 있는 오픈소스 Framework

**URL 관리**

urls.py의 urlpatterns에서 담당

**path 의 구조**

**path('URL', views.xxxxx, name="URL")**

* **URL** 페이지 주소(ex introduce/, new/)

* **함수** url이 불렸을 때 실행할 함수(ex views.home)

* **name** 해당 path를 대표하는 이름(ex. name="home")

**Template 언어**

python변수 & 문법을 HTML에서 쓸 수 있도록 Django에서 제공하는 언어

*  **{{}}** 템플릿 변수(명사)

* **{%%}** 템플릿 태그(동사)

**Static File**

이미지나 CSS, JS파일처럼 내용이 고정되어 있어, 응답을 할 떄 파일 그대로를 보내주면 되는 파일

**Static** -  웹 서비스를 위해 개발자가 준비해두는 파일

**Media** - 웹 서비스 이용자들이 업로드하는 파일

**HTML에서 static file 사용 할 때 맨 위에 {%load static%} 꼭 써주기!**