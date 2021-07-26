# window.close로 팝업창을 닫을 수 있다.

```
 자기자신을 닫을 때는

 window.open("about:blank","_self").close();

 자기 자신에 윈도우를 하나열어서 자기 자식윈도우로 만든다음에 바로 닫아버린다.
```
 

 그렇다면 반대로 팝업이나 Open된 창에서 부모창을 닫을 때는 어떻게 할까..

  간단하다..

  opener.open('about:blank','_self').close();
  부모창에다 열고 닫아버리면 된다...
  
  
[출처] JavaScript에서 close()함수를 사용하자! 총정리!|작성자 일리
