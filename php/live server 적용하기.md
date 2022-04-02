첫번째는 xampp설치

https://teserre.tistory.com/12

2번째는
htdocs안에 workspace 만든 후 setting.json 파일 만든 후 vs코드에 live server setting.json을 맞춰준다
아래처럼 경로 맞춰주기

{
    "liveServer.settings.CustomBrowser": "chrome",
    "liveServer.settings.proxy": {
        "enable": false,
        "baseUri": "/",
        "proxyUri": "http://localhost:8080/workspace/test.php"
    }
}
