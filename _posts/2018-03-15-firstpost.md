STS에서 생성한 프로젝트에 Mybatis를 설정하도록 하겠습니다. (이전작업 http://huskdoll.tistory.com/184 을 하시고 따라하시면 좋습니다.)

아래의 프로젝트 구성을 확인하시면 빨간박스안에 있는 파일들은 새로 생성한 파일이며 파란색 박스는 기존 소스에 Mybaits 설정을 추가해준 파일입니다.

아래 예제를 따라 하실때 아래와 동일한 구조로 해보시기 바랍니다.



작업 순서는 아래와 같습니다.



1. pom.xml 에 라이브러리를 추가 시켜 줍니다. (Mybatis 및 jdbc등 DB에 접근하기 위한 라이브러리 추가)



2. root-context.xml에 Mybatis 설정을 적어 줍니다. (DB설정 정보 및 Mybatis 정보를 가지고 있는 파일 위치 셋팅)



3. jdbc-config.xml 을 생성하고 설정을 적어 줍니다. (DB설정 정보 및 Mybatis 정보 설정)



4. jdbc.properties 을 생성하고 설정을 적어 줍니다. (DB설정 정보파일 생성, url, id, pw 같은 정보를 따로 저장관리)



5. package와 class을 생성하고 내용을 적어 줍니다. (controller, service, dao...등 작성)



6. 테이블 및 데이터 생성 (DB에서 가져올 데이터 생성)



7. 쿼리 xml (쿼리문 작성)



8. jsp 페이지 생성



9. 실행