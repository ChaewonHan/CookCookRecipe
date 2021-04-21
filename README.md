# 🍳CookCook Recipe

![Untitled](https://user-images.githubusercontent.com/75398832/115556780-fbc5f180-a2eb-11eb-9285-1a5ada8f5af6.png)


## 목차


## 소개

 kh교육원에서 진행한 JSP/Servlet 기반 팀 프로젝트 입니다.  MVC1 패턴 구현을 통해 동작원리를 이해하고 기본적인 게시판 CRUD를 구현하는 것에 중점을 맞춘 프로젝트 입니다. 

### 프로젝트 주제

레시피 공유 사이트

### 기획의도

코로나 19로 인하여 가정에서의 식사시간에 늘어남에 따라 2020년 식문화 트렌드 또한 변화되었습니다. 인터넷상에서 달고나 커피가 유행하는 등 가정에서 요리에 소요하는 시간이 늘어나게 되었고이러한 트렌드에 발 맞추어 다양한 집밥 레시피를 공유하기 위한 홈페이지를 기획하고 제작하게 되었습니다.

### **구현 기능**

- 회원 관리
    - 회원가입(이메일 인증)
    - 아이디 찾기, 비밀번호 찾기(이메일 인증)
    - 개인 정보 수정
    - 회원 탈퇴
- 게시판
    - 게시판 CURD
    - 게시글 답글 기능
    - 게시판 페이징
    - 검색기능(분류별)
    - 카테고리 기능

## ERD
<br/>

![그림1](https://user-images.githubusercontent.com/75398832/115559610-ccfd4a80-a2ee-11eb-9ce7-ad21eb55ae3e.png)
<br/>
회원 테이블을 중심으로 유니크 속성을 가진 닉네임을 참조하여 비식별 관계로 각각의 게시판 테이블을 구성하였습니다. 
레시피 게시판의 경우, 파일 업로드 기능을 구현하기 위해 파일과 관련된 컬럼들을 추가하였고 
1:1관계로 설정하여 카테고리 테이블도 만들어 카테고리별로 게시글이 나타날 수 있도록 하였습니다. 
비회원 게시판의 경우에는 답글 기능을 구현하여 답글과 관련된 컬럼들이 담긴 테이블로 구성하였습니다.


## 담당한 기능


**회원가입 기능**
<br/>

![ezgif-3-12cde8da2b2b](https://user-images.githubusercontent.com/75398832/115556912-26b04580-a2ec-11eb-8bbb-71e83bb80e77.gif)
<br/>
[회원가입 jsp](0_semiProject/WebContent/views/memberJoin.jsp)<br/>
[회원가입 java]()
정규식과 ajax, onkeyup을 사용하여 입력하는 도중에 유효한 값인지 바로 검사할 수 있도록 구현 하였습니다. 유효한 값이 아니라면 경고 메세지가 입력창 아래 span 태그에 경고문장을 넣어서 실시간으로 경고메세지를 볼 수 있도록 했습니다.

**이메일 인증번호 전송**
<br/>

![ezgif-3-16500890328c](https://user-images.githubusercontent.com/75398832/115557402-a3dbba80-a2ec-11eb-8d0a-4f2c55b5e720.gif)


**게시판 페이징 처리**
<br/>

![ezgif-3-306c4d3aa6c3](https://user-images.githubusercontent.com/75398832/115557455-af2ee600-a2ec-11eb-8bad-8da93d2a3463.gif)


**게시판 글 작성**
<br/>

![ezgif-3-a8c19394c9f5](https://user-images.githubusercontent.com/75398832/115557520-bbb33e80-a2ec-11eb-8f70-4164514cd7e0.gif)


**게시글 답글 작성**
<br/>

![ezgif-3-e49efa842237](https://user-images.githubusercontent.com/75398832/115557566-c8379700-a2ec-11eb-8fc2-712600f4e30a.gif)



**게시글 수정**
<br/>

![ezgif-3-dfb9db1a26a0](https://user-images.githubusercontent.com/75398832/115557644-dd142a80-a2ec-11eb-9228-70bd91fee1fa.gif)


**게시글 삭제**
<br/>

![ezgif-3-0caccaee5e10](https://user-images.githubusercontent.com/75398832/115557665-e604fc00-a2ec-11eb-8802-87f35f791b64.gif)


**게시판 키워드 검색**
<br/>

![ezgif-3-5e3d060a6caa](https://user-images.githubusercontent.com/75398832/115557697-edc4a080-a2ec-11eb-80f4-b0df00680b53.gif)


