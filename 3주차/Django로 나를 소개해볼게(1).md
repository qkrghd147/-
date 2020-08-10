# Django로 나를 소개해볼게(1)

* Model의 이해
* Model과 Database의 연동 이해 & 실습
* Admin 파악

Model이란?

데이터에 접속하고 관리하도록 도와주는 객체
==
장고와 데이터베이스가 서로 소통하도록 도와주는 객체

Model 생성 & 적용

models.py # 모델명의 첫글자는 무조건 대문자!

class Designer(models.Model):

image = models.lmageField(upload_to = 'images/')

name = models.CharField(max_length = 50)
address = models.CharField(max_length = 255)

description = models.TextField()

Terminal

DB가 알아듣도록 번역하기
python manage.py makemigrations + App이름

번역한 내용을 DB에 적용
python manage.py migrate + App이름
