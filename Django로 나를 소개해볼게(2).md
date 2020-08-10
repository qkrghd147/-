# Django로 나를 소개해볼게(2)

QuerySet이란?

전달받은 모델의 객체 목록

붕어빵과 붕어빵 틀을 생각하자!


객체가많으면

views.py 

#Model의 존재 알려주기

from .models import Designer -> 

#Queryset을 Templates로 보내기

def home(request):
designers = Designer,objects.all()

return render(request, home.html, {'designers': designers})