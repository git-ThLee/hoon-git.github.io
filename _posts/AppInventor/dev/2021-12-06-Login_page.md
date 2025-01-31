---
title:  "[앱인벤터] 로그인 페이지 만들기 "
excerpt: "로그인 페이지 만들기 "

categories:
  - AppInventor_dev
tags:
  - [Login, Sign In, Sign Up]

toc: true
toc_sticky: true
 
date: 2021-12-06
last_modified_at: 2021-12-06
---

# 로그인 페이지 만들기

---  

![KakaoTalk_20211213_134532226_02](https://user-images.githubusercontent.com/55564114/145754223-f77b5366-0fee-43b6-a6fd-6f8bc258627f.png)  

![KakaoTalk_20211213_134532226_01](https://user-images.githubusercontent.com/55564114/145754101-588a04aa-35a6-48aa-9fb6-539d4743ecff.png)  



오늘 만들어볼 것은 **로그인 페이지**입니다.  
- 사용방법  
  1. 회원가입을 한다.  
  2. 로그인을 한다.  
  3. 로그인에 성공하면 "훈깃님 반갑습니다." 알람 띄우기  
  4. 로그인에 실패하면 실패이유 알람 띄우기  

---
## 1. 디자인

### # Screen 1
![스크린샷(90)](https://user-images.githubusercontent.com/55564114/145754442-3b581bbd-9d93-4539-88cc-536ea932ae26.png)  

### # Screen 2
![스크린샷(91)](https://user-images.githubusercontent.com/55564114/145754459-4067faa5-4875-4e11-ad98-b13ad826535c.png)  

---

### #디자인 구조

#### # Screen 1

| 1 | 2 | 3 | 4 | 
| :---: | :---: | :---: | :---: | 
| Screen1 |  |  |
|└|수직배치|
||└|레이블_로그인|
||└|수평배치|
|||└|텍스트박스_아이디|
||└|수평배치|
|||└|암호텍스트박스_비밀번호|
||└|버튼_로그인|
||└|버튼_회원가입|
|보이지않는||
||알림1|
||타이니DB1|  

#### # Screen 2

| 1 | 2 | 3 | 4 | 
| :---: | :---: | :---: | :---: | 
| Screen2 |  |  |
|└|수직배치|
||└|레이블_회원가입|
|└|수평배치|
||└|레이블_아이디|
||└|텍스트박스_아이디|
|└|수평배치||
||└|레이블_비밀번호|
||└|텍스트박스_비밀번호|
|└|수평배치||
||└|레이블_비밀번호확인|
||└|텍스트박스_비밀번호확인|
|└|수평배치|
||└|레이블_이름|
||└|텍스트박스_이름|
|└|수평배치|
||└|버튼_취소|
||└|버튼_회원가입|
|보이지않는|
||알림1|
||타이니DB1|
  

**구체적인 속성이 궁금하시면 댓글 적어주세요**

---

## 2. 만들어야할 기능 

### # Screen 1

1. 회원가입 버튼을 클릭하면 Screen 2로 이동하기  

2. 로그인 버튼을 클릭하면 타이니 DB로 로그인 시도하기  
> ex)  
> 1 : 로그인 버튼 클릭  
>> 2 : 만약 아이디가 비어있다면, "UserName을 입력해주세요" 알림 띄우기  
>> 3 : 만약 비밀번호가 비어있다면, "Password를 입력해주세요" 알림 띄우기  
>>> 4 : 타이니 DB에 아이디 조회하기  
>>> 5 : 만약 조회된 아이디가 없다면, "가입된 회원이 아닙니다" 알림 띄우기  
>>>> 6 : 타이니 DB에 비밀번호 비교하기  
>>>> 7 : 만약 비밀번호가 틀리면, "틀렸습니다" 알림 띄우기  
>>>> 8 : 만약 비밀번호가 맞으면, "○○님 반갑습니다:)" 알림 띄우기  

### # Screen 2

1. 취소하기 버튼을 클릭하면 Screen 1로 이동하기  

2. 회원가입 버튼을 클릭하면 타이니 DB로 회원강비 시도하기
> ex)  
> 1 : 회원가입 버튼 클릭  
>> 2 : 만약 아이디가 비어있다면, "UserName을 입력해주세요" 알림 띄우기  
>> 3 : 만약 비밀번호가 비어있다면, "Password를 입력해주세요" 알림 띄우기  
>> 4 : 만약 이름이 비어있다면, "이름을 입력해주세요" 알림 띄우기  
>> 5 : 만약 비밀번호와 비밀번호_확인이 다르면, "다릅니다" 알림 띄우기  
>>> 6 : 타이니 DB에 아이디 조회하기  
>>> 7 : 만약 조회된 아이디가 없다면, 타이니 DB에 값 저장하기  
>>> 8 : 만약 조회된 아이디가 없다면, "회원가입에 성공" 알림 띄우기  
>>> 9 : 만약 조회된 아이디가 없다면, Screen 1으로 이동하기  
>>> 10 : 만약 조회된 아이디가 있다면, "이미 존재하는 유저입니다" 알림 띄우기  

---

## 3. 블록코딩

### #한글버전  

#### # Screen 1  
![스크린샷(92)](https://user-images.githubusercontent.com/55564114/145756001-8ad0f25f-e5df-4d29-909b-a47d83478873.png)  

#### # Screen 2  
![스크린샷(95)](https://user-images.githubusercontent.com/55564114/145756224-d9aa613b-8e5c-4914-8a2c-03292e7bc375.png)  




### #영어버전  

#### # Screen 1  
![스크린샷(93)](https://user-images.githubusercontent.com/55564114/145756048-1b6df145-5c1c-4aa1-abfd-c2722f9ab634.png)  

#### # Screen 2  
![스크린샷(94)](https://user-images.githubusercontent.com/55564114/145756154-3597452e-7b57-4da5-955b-478971d62945.png)  



---

## 4. 추가정보

1. 타이니 DB에 저장된 값은 어플을 종료했다 다시 실행해도 데이터가 남아있다.  
2. DB 는 DateBase의 약자로 데이터 저장하고 조회 및 삭제 등이 가능하다.  
3. MySQL, Firebase 등을 이용하면 온라인으로 아이디 조회 및 삭제 등이 가능하다.  
4. 타이니 DB는 리스트를 저장이 가능하다.  

로그인 페이지 끝입니다.  
궁금하신 부분은 댓글주시거나 메일 주시면 됩니다.🥰🥰  

---

