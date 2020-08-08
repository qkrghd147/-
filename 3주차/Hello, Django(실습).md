# Hello, Django(실습)

**가상환경**

자신이 원하는 python 환경 구축을 위해 필요한 모듈만 담아 놓는 바구니(필요한 패키지만 그 가상환경안에서 활용함!)

**PIP**

python으로 작성된 패키지 소프트웨어를 관리하는 패키지 관리 시스템

**VS code 단축키**

* 터미널 생성

> ctrl + shift + `

* 현재 커서 위치의 코드 복사

> ctrl + D

**가상환경 관련 코드**

* 가상환경 생성

> python -m venv <가상환경  이름>

* 가상환경 활성화

> source <가상환경 이름>/Script/activate

* 가상환경 끄기

> deactivate

**Django 명령어**

* Django 패키지 설치
> pip install django

* Django 프로젝트 생성
> django-admin startproject<프로젝트명> . (온점을 붙이면 폴더를 생성하지 않음)

* Django App 생성
> python manage.py startapp <App이름>

* Django 로컬 서버 시작
> python manage.py runserver

**.git ignore**

캐시 파일 담당

**Django의 Project와 App**

하나의 project = 하나의 web site

Project 안의 기능을 각각의 App으로 관리
Ex) Project = 대학교
App = 대학 안의 각 부서

**Project**

* **settings.py** 전체 프로젝트를 관리하는 설정 파일

* **urls.py** 프로젝트의 URL 관리 파일

* **wsgi.py, asgi.py** 프로젝트를 서비스하기 위한 파일

* **__init__.py** 해당 디렉토리가 python package의 일부임을 python에게 알려주는 파일

**App**

* **views.py** 웹 요청을 받고, 전달받은 데이터를 처리해서 가공하는 파일

* **models.py** Database와 관련된 다양한 역할 수행

* **admin.py** 관리자 관련 파일

* **apps.py** Project에게 App의 존재를 알려줄 때 활용되는 파일

**Home 페이지 출력과정**


1. **settings.py** Project에게 App의 존재 알리기

2. **Templates** User에게 보여줄 HTML 파일 만들기

3. **views.py** 요청이 들어오면 HTML 파일을 열어주는 함수 정의

4. **urls.py** url 요청을 views와 연결하기