# npm start 후 ctrl+c 누르면 종료도 가능
# react 구성요소

App.js -> index.js -> index.html로 넣어준다
![image](https://user-images.githubusercontent.com/85022962/128715099-9e85e2cc-5304-4ff5-9cf3-df33faac87c8.png)

# 자동완성 기능 안될 시 아래와 같이 수정

 "emmet.triggerExpansionOnTab": true, // <-- emmet 활성화
    "emmet.includeLanguages": {
      "javascript": "javascriptreact" // <-- react에서도 emmet 사용가능하도록
    }
![image](https://user-images.githubusercontent.com/85022962/128716946-9193e33d-6efa-4630-8b9d-f2654346b9ce.png)

# 변수 지정 시 2가지 방법 있따

## 1번 {} 중괄호 사용 하면 거의 다 넣는거 가능 
![image](https://user-images.githubusercontent.com/85022962/128787995-828a44f7-8f0e-425e-a2a1-b311e079c569.png)

## 2번 useState(with destructuring) 
### 왜 쓰냐? 새로고침 없이 바로 변경이 가능하기 때문!!

const [a,b] = useState(1)2 > 함수는 1번 내용과 2번 함수를 갖고온다  즉 a=1, b=2

![image](https://user-images.githubusercontent.com/85022962/128788371-13c6547d-9a78-4062-900a-ce9861073b25.png)

