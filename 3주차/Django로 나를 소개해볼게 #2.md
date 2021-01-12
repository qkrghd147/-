# Django로 나를 소개해볼게(2)

**QuerySet이란?**

전달받은 모델의 객체 목록

붕어빵과 붕어빵 틀을 생각하자!


**객체가많으면**

views.py에

* **#Model의 존재 알려주기**
> from .models import Designer -> 

**#Queryset을 Templates로 보내기**
def home(request):
>designers = Designer,objects.all()
return render(request, home.html, {'designers': designers})

**Detail page 구현**

**각각의 글을 분류 - PK (Primary Key) - Model을 통해 생성된 객체들을 구분할 수 있는 "고유한" Key**

Ex) 우리가 Designer등록하면 각각의 PK(id)가 있음.

**여러 객체의 url을 "계층적으로" 다룰 수 있도록 도와주는 도구 - Path Convertor**

>**urls.py** path('profile/<int:designer_id>/', views.detail, *name = "detail")

>**Tempalte** {% url 'detail' designer.id %}

ex) www.dreamary.com/profile/1 ~ 3   /profile/객체번호

**Objecct를 가져오려 했는데 없을 경우 나타나는 에러 - get_object_or_404**

**views.py** from django.shortcuts import render,get_object_or_404

>def detai(request, designer_id): 
designer=get_object_or_404(Designer, pk = designer_id)
return render(request, 'detail.html',{'designer':designer}
