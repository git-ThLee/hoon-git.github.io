---
title:  "[스크래치] 픽셀 그림판 만들기"
excerpt: "픽셀 그림판 만들기"

categories:
  - Scratch_dev
tags:
  - [Scratch]

toc: true
toc_sticky: true
 
date: 2021-12-20
last_modified_at: 2021-12-20
---

# #만들 프로젝트 설명

![Animation](https://user-images.githubusercontent.com/55564114/146697841-31f2993a-04a0-46ff-a1d8-2f440a7696ee.gif)  

- 만들어야 할것.  
1. 그림판 만들기  
2. 그림판의 어두운 타일을 클릭하면 노란색으로 변경  
3. 그림판의 밝은 타일을 클릭하면 변경 X  
4. 그림판의 노란색 타일을 클릭하면 어두운 타일로 변경  
5. 초기화 버튼을 클릭하면 그림판을 초기상태로 변경  
6. 불러오기 버튼을 클릭하면 노란색 타일 불러오기  

- 스크래치 공유  
  
  [스크래치](https://scratch.mit.edu/projects/616687706/)  
    
  공유했으니 궁금하면 들어보시면 좋을거 같아요.  

---

# 1. 디자인

## 1.1 스프라이트

![스크린샷(99)](https://user-images.githubusercontent.com/55564114/146698093-0453060a-938f-43b9-91de-17cd8ede6cd1.png)  

- 맵(타일)  

![스크린샷(100)](https://user-images.githubusercontent.com/55564114/146698159-d74b03f4-c9ba-4665-aabc-c109cd4931fd.png)  

|속성|내용|예시|
| :---: | :---: | :---: |
|생성 방법| 스프라이트 그리기 |  |
|스프라이트 이름 | 맵 |  |
|모양 개수 | 3 개  |  |
| x | 상관 X | |
| y | 상관 X | | 
| 보이기 | on |  |
|크기 | 100 | |
|방향 | 90 |  |  
  

  
  
- 불러오기  

![스크린샷(101)](https://user-images.githubusercontent.com/55564114/146698326-35d06efa-564d-4065-8f69-fd33f2684f00.png)  

|속성|내용|예시|
| :---: | :---: | :---: |
|생성 방법| 스프라이트 그리기 |  |
|스프라이트 이름 | 불러오기  |  |
|모양 개수 | 1 개  |  |
| x | 160 | |
| y | -140 | | 
| 보이기 | on |  |
|크기 | 100 | |
|방향 | 90 |  |  
  

- 초기화  

![스크린샷(102)](https://user-images.githubusercontent.com/55564114/146698432-0df3bf34-40a0-4693-8f4c-0359730381bd.png)  

|속성|내용|예시|
| :---: | :---: | :---: |
|생성 방법| 스프라이트 그리기 |  |
|스프라이트 이름 | 초기화  |  |
|모양 개수 | 1 개  |  |
| x | 40 | |
| y | -140 | | 
| 보이기 | on |  |
|크기 | 100 | |
|방향 | 90 |  |  
  
---

## 1.2 배경

- 배경  

![스크린샷(79)](https://user-images.githubusercontent.com/55564114/144007172-37103c8d-d6f5-4b69-8e24-69e5878cf1ea.png)  
  
  직사각형으로 채워주면 되요. 


---

# 2. 변수, 리스트, 내 블록

## 2.1 변수  

1. 블록 번호  
1.1 이 스프라이트에서만 사용(타일에서 변수 생성해주세요)  
2. 반복문 카운트  
2.1 모든 스프라이트에서만 사용  
3. 플레이어 위치  
3.1 모든 스프라이트에서만 사용
  
## 2.2 내 블록 

- 없음. 

## 2.3 리스트

1. 그림저장_리스트

---

# 3. 블록코딩

 - 맵(타일)  
![스크린샷(99) (1)](https://user-images.githubusercontent.com/55564114/146698577-b5ec67aa-610f-46ca-9f3a-2dc89d438c9e.png)  

 - 불러오기  
![스크린샷(103)](https://user-images.githubusercontent.com/55564114/146698629-98da348c-be76-4041-a0bd-02f76cc2c629.png)  

 - 초기화  
 ![스크린샷(104)](https://user-images.githubusercontent.com/55564114/146698695-699a4053-7b85-4ead-9f4a-3296acc49ae1.png)  

---

수고하셨습니다.  

---

