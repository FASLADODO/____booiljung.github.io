# Tips of Software architecture

##### 로그, 캐시 파일을 위한 별도의 디스크

- 데이터, 로그, 캐시 등이 있는 데이터 서버가 HDD에 저장하는 경우 할 수 있다면 하나의 HDD를 사용하는 것보다, 데이터용 HDD와 로그/캐시용 HDD로 나누는 것이 속도에 유리 합니다. 데이터를 커밋하는 경우 별개의 파일을 사용하면 HDD 헤드를 움직이고, 헤드를 움직이면 연속으로 읽는 것보다 10만배 이상의 시간을 낭비합니다.