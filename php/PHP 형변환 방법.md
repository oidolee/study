PHP에서 cint() 혹은 parseint() 같은
문자를 숫자로 형변환 하는걸 찾고 계셨군요

PHP는 다른 언어들 보다 더 쉽고
직관성 있게 형변환을 사용할 수 있습니다.


출처: https://gocoder.tistory.com/611 [고코더 IT Express]2

<?php
    // PHP는 (int)를 원하는
    // 변수에 붙이면 형변환이 된다.
 
    echo (int)1.1;    // 1
    echo (int)"2";    // 2
    echo (int)-3.1;    // -3
    echo (int)"고코더";    // 0
 
?>

그밖에 변환 가능한 형변환 종류는 아래와 같습니다.

(string) 문자열
(int) 정수
(double) 실수
(bool) 부울
(array) 배열
(object) 객체


출처: https://gocoder.tistory.com/611 [고코더 IT Express]
