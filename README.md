# HTML

## 표기법
1. dash-case(kabab-case)  
-html ,css
-기호를 써서 캐밥 혹 대쉬  
 ex)   the-quick-brown-fox-jumps-over-the-lazy-dog  
 ( - 기호를 써서 띄어쓰기를 인지 )


2. snake_case  
-htme ,css  
ex ) the_quick_brown_fox_jumps_over_the_lazy_dog ( _ 기호를 써서 띄어쓰기를 인지 )

3. camelCase  
-js (대부분사용)  
ex ) theQuickBrownFoxJumpsOverTheLazyDog  ( 대문자를 써서 인지)

4. PascalCase  
-js  
ex ) theQuickBrownFoxJumpsOverTheLazyDog ( 첫문장부터 대문자 )

***
## 특수문자정리
grave= `  
tilde=~  
at sign=@  
caret=^  
ampersand=&  
hyphen,dash=-  
underscore,low dash = _  
equals sign ==  
quotation mark="  
apostropha='  
colon=:  
semicolon=;  
period,dot=.  
comma=,  
slash=/  
vertical bar =|  
back slash =\  
parenthesis=()  
brace={}  
bracket=[]   
angle bracket =<>

***
## 부모와 자식관계
<태그><태그>내용</태그></태그>  
  조상 부모    자식  부모    조상
***
## 인라인(inline)
인라인요소(글자요소)
-대표적으로 span이 있다  
-수평으로 쌓임  
-본질적으로 아무것도 나타내지 않는 콘텐츠 영역을 설정하는 용도이다  
-요소가 수평으로 쌓인다  
-포함한 콘텐츠 크기만큼 자동으로 줄어듬  
-글자요소는 가로세로 사이즈를 지정할 수 없다
그래서 css속성(width,height)로 지정 불가능  
-글자여백(margin=외부여백 , padding=내부여백)은 가로세로는 가능하지만 위,아래는 불가능하다  
-인라인 요소 안에는 블럭요소를 넣을 수 없다  

## 블록(block)
블록요소(상자요소)(레이아웃)  
-대표적으로div가 있다  
-요소가 수직으로 쌓임  
-부모요소의 크기만큼 자동으로 늘어남  
-글자요소는 가로세로 사이즈를 지정할 수 있다
그래서 css속성(width,height)로 지정 가능  
-글자여백(margin=외부여백 , padding=내부여백) 가능  
-블록요소 안에는 다 넣을 수 있다
***
## 전역속성
title
-요소의 정보나 설명을 지정

style
-요소에 적용할 스타일을 지정

class
-요소를 지칭하는 중복 가능한 이름
-그룹을 짓는것이다
-css에 적용할때 .을 붙힌다

id
-요소를 지칭하는 고유한 이름
-css에 적용할때 # 을 붙힌다
-핵심적인 요소는 id를 붙히자

data
-요소에 데이터를 지정   
-사용법-
-data-이름="데이터"
-코드팬에서 테스트를 하고 vs코드에서 테스트를 할때 오류가 날 수 있기 때문에
script에서 defer를 추가해야한다(defer은 html 코드를 다 읽고 js로 이동할 수 있도록 한다) 
***

## 태그(tag)
doctpe html -문서의 html버전을 지정
DTD은 마크업 언어에서 문서 형식을 정의 웹 브라우저가 어떤 html버전의 해석 방식으로 페이지 알려줌

Html -시작 테그  
Html-종료 테그

-->문서의 전체 범위

head
--> 문서의 정보(눈에 보이지 않음)를 나타내는 범위 

body
--> 문서의 구조(눈에 보이는)를 나타내는 범위 

title
--> 문서의 제목을 정의
     웹 브라우저 탭에 표시 됌.

link
--> 외부 문서를 가져와 연결할 때 사용 (대부분 css파일)
rel -가져올 문서와 관계
href- 가져올 문서의 경로


style
--> 스타일을 html문서 안에서 작성하는 경우에 사용

script
--> 자바스크립트파일 가져오는 경우

meta
--> 나머지 모든정보를 제공

***

## HTML 요소
div
-특별한 의미가 없는 구분을 위한 요소(division)

h
-제목을 의미하는 요소 (Heading)
-h1~h6이 있는데 대체로 목차인 느낌
-숫자가 작을수록 더 중요한 제목을 정의

p
-문장을 의미하는 요소(paragraph)

img(인)
-이미지를 삽입하는 요소
-필수속성-
-src : 삽입할 이미지의 경로
-alt : 삽입할 이미지의 이름

ul
-순서가 필요없는 목록의 집합의 의미(undered list)
-ul태그에는 li가 있어야 한다 (세트의 느낌)

li
-목록 내 각 항목 (list item)

ol
-순서가 있는 목록의 집합의 의미(ordered list)

a(인)
-다른/같은 페이지로 이동하는 하이퍼링크를 지정하는 요소(Anchor닻)
-링크를 걸때 사용
-필수요소-
-href : 사이트
-target : 링크 url의 표시 위치 "_blank" 은 새탭에 연다라는 뜻 ex)href="google.com" target="_blank"

span(인)
-특별한 의미가 없는 구분을 위한 요소
-보통 글자 중 특별한 범위를 잡고 싶을 때

br(인)
-줄바꿈(break)

input(인라인이면서 블록)
-입력받을 데이터가 있을때
-인라인요소지만 사이즈 설정 가능
-요소-
-type : 입력받을 데이터의 "타입"
-value : 미리 입력된 값(데이터)
-placeholder : 사용자가 입력할 값의 힌트 
-disabled : 입력 요소 비활성화 

label(인)
-라벨 가능 요소의 제목
-요소-
type="checkbox" : 사용자에게 체크 여부를 받음 checked 체크박스 입력 요소 미리 체크됨
type="radio"  :  사용자에게 체크 여부를 그룹에서 1개만 입력 받음  name=" " 그룹

table(테이블요소,표)
-표 요소 행과 열의 집합
-행이 먼저이고 다음이 열이다
-요소-
-tr : 행
-td : 열 

***

## HTML 특수기호
&copy
-동그란 c   

```
&lt; abcd &gt;  
<abcd>
```

html entities
-html에서 쓸 수 있는 특수기호들
