# useState 변경시 [1,2] 2번에 있는 함수 활용

![image](https://user-images.githubusercontent.com/85022962/128806230-cb733988-5892-47c6-9e87-27af11291cf2.png)
![image](https://user-images.githubusercontent.com/85022962/128806274-50ca0af8-af4e-4999-a1fa-e944bad42fb3.png)
![image](https://user-images.githubusercontent.com/85022962/128806286-b835d1f0-f446-4f8c-82e5-3c25c7f2acfe.png)

## 1번 변수를 가져와서 2번에 넣는다

![image](https://user-images.githubusercontent.com/85022962/128806394-26e418bf-3bc8-4b5f-b599-f51d45c37b82.png)

## useState 배열값을 바꾸고 싶으면 통쨰로 바꿔라

![image](https://user-images.githubusercontent.com/85022962/128810947-3e6ddcdc-dfa6-40f7-b457-dd7032656081.png)

## deep copy로 배열 복사 참조값만 갖고옴 (값공유x)

![image](https://user-images.githubusercontent.com/85022962/128811527-820c8998-4a4c-4712-ad7c-5b9c77f8661d.png)


## state 건들지 말자
![image](https://user-images.githubusercontent.com/85022962/128815115-4c90474f-5842-4e09-9c29-af8588a79858.png)

# 핵심은 복사다 원리는 아래와 같고 참조형(배열 객채 함수)이기에 [...state명]으로 쓰자
![image](https://user-images.githubusercontent.com/85022962/128815229-5c29a30d-583a-4257-ae43-2d6f9b7e6fb2.png)
![image](https://user-images.githubusercontent.com/85022962/128815372-c76d3b02-6b88-4aa3-bab7-30fd0e2349f5.png)


