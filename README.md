[[ front - svelte ]]

frontend/.env

에서 백엔드 주소 명시가능.

현재 백엔드 주소는 192.168.254.10:8000 으로 되어있음

쿠버네티스에서는 서비스이름, 도커에서는 --link 옵션으로

백엔드를 내부에서 지정하는게 좋습니다.

node:20에서 빌드후 생성된 dist폴더의 정적파일을

nginx 컨테이너로 옮기도록 구성됨.

[[ 백엔드 - fastapi ]]

DB사용자=user

DB암호=1234

DB이름=db

DB주소=192.168.254.10

DB포트=3306

database.py 에서 주소 수정가능

DB는 mysql:8 사용. 직접 만들어야함!