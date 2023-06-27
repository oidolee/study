https://bill1224.tistory.com/268

Laravel .env파일 설정
MAIL_MAILER=smtp
MAIL_HOST=smtp.gmail.com
MAIL_PORT=587
MAIL_USERNAME=아이디
MAIL_PASSWORD=비번
MAIL_ENCRYPTION=tls
MAIL_FROM_ADDRESS=null
MAIL_FROM_NAME="${APP_NAME}"
.env 파일 설정까지 해주면, Gmail을 이용할 준비는 끝났다.


https://sung-jun.tistory.com/157

 

그리고 .env 파일을 열어줍니다.

MAIL_MAILER=smtp
MAIL_HOST=smtp.gmail.com
MAIL_PORT=587
MAIL_USERNAME=user_name@gmail.com
MAIL_PASSWORD=user_password
MAIL_ENCRYPTION=tls
MAIL_FROM_ADDRESS=hello@example.com
MAIL_FROM_NAME="${APP_NAME}"
 

위와 같이 입력해주는데

이메일과 비밀번호는 자신의 구글 이메일과, 비밀번호입니다.

그리고 MAIL_FROM_ADDRESS, MAIL_ENCRYPTION 부분을 null로 해두면 에러가 발생하기 때문에 꼭 입력해줍시다.

 

php artisan config:cache
 

위 명령어로 캐시를 초기화 해주고, 다음으로 서버를 재시작해줍니다.

그렇지 않으면 에러가 발생합니다. 꼭 해주세요.
