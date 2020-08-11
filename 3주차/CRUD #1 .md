# CRUD #1

**GET/POST**

클라이언트에서 서버로 요청을 보내는 방법

**GET**

1. Data를 "URL"에 포함시켜 전송
2. 전송하는 길이에 제약 있음
3. Caching 가능

(REST에서 데이터 조회에 활용) == READ에서 활용

**POST**

1. Data를 "Body"에 넣어 전송(URL에서 노출 X)

2. 전송하는 길이에 제약 X

3. Caching 불가능

(REST에서 데이터 생성에 활용)
== CREATE / UPDATE에서 활용

**CREATE**

새로운 객체를 생성해 Data를 저장

- 객체 생성 

> if request.method == 'POST':   
post = Designer()

* 입력 Data 수신

> post.name = request.POST['name']   
post address = request.POST['address']....

* 입력 Data 저장

> post.save()

**UPDATE**

정보 수정이 필요한 객체를 찾아 Data를 새롭게 저장

* 객체 탐색

> post = get_object_or_404(Designer,pk=designer_id)     
if request.method =='POST'

* 입력 Data 수신

> post.name = request.POST['name']
post.address=request.POST['address']

* 입력 Data 저장 

> post.save()

**DELETE**

제거가 필요한 객체를 찾아 삭제

* 객체 탐색 

> post = get_object_or_404

* 객체 삭제

> post.delete()

* Home으로 이동

> return redirect('home')