# 정구민

## 기본 정보

- email : jgm0710@gmail.com
- github : https://github.com/jgm0710

## 학력

- 명지전문대학교 2015/03 ~ 2021/02 컴퓨터 전자과 졸업

## 경력 사항

- 신입

## 자격 사항

- 정보처리산업기사 자격증

## 기술 스택

- 백엔드
  - Spring(java) : 
    - Spring Boot 활용
    - Spring Data Jpa 를 활용한 ORM 방식의 프로그램 개발
    - QueryDsl 을 활용한 동적쿼리
    - Spring Rest Docs 를 활용한 문서화
    - Spring Security 를 이용한 JWT토큰 인증 방식 API
    - Junit5 / Junit4 를 활용한 단위/통합 테스트
  - Mysql
  - REST API 성숙도 모델에 대한 이해 有

- 배포
  - AWS EC2 사용 
  - Docker 
    - Dockerfile, docker-compose 를 사용한 이미지 빌드 사용
    - 컨테이너에 대한 이해 有

- 소스코드 관리
  - GitHub, GitLab 사용 경험 有

- 협업 경험
  - 경험 중
  - GitLab 를 사용한 협업 진행
    - milestone, issue 를 등록하여 일정 관리
  - Git-Flow 를 사용한 Git 협업 



# 진행 프로젝트

## 개인 프로젝트

- [Custom Vocabulary](https://github.com/jgm0710/custom-vocabulary)
  - 기술 스택 : Spring Boot, Spring Data JPA, QueryDsl, Spring Rest Docs, jquery + ajax, MariaDB, AWS RDS, GCP
  - [API 문서 열람 링크](http://3.35.0.222:8080/docs/index.html)
  - 기간 : 2021 / 01 ~ 2021 / 03
  - 개인 프로젝트
  - 설명
    - 자신만의 단어장을 만들어서 학습할 수 있도록 서비스를 제공
    - REST API 기반의 프로젝트
    - Rest Docs 를 통한 문서화 진행
    - Junit5 를 통한 단위 테스트 및 통합 테스트 진행
    - AWS 를 통한 배포
    - certbot 을 사용한 https 적용
    - AWS RDS
    - Spring MVC 를 통해 만들어진 REST API 를 활용 -> jquery ajax 를 통해 클라이언트 
    - flyway 를 통한 DB 형상 관리

## 팀 프로젝트 

- [Bbangduck](https://github.com/jgm0710/Bbangduck/tree/develop)
  - 기술 스택 : Spring Boot, Spring Data JPA, QueryDsl, Spring Rest Docs, Mockito 
  - [API 문서 열람 링크](http://13.125.48.96:8080/docs/index.html)
  - 설명 
    - 방탈출 리뷰 사이트를 구현하기 위한 API
      - 국내의 여러 방탈출 카페의 테마를 대상으로 리뷰를 공유하고 자신의 경험을 남길 수 있다.

  - 프로젝트 진행 상황 
    - 참여 인원 : 6
      - 기획 - 1
      - 디자인 - 1 
      - 프론트 - 1 
      - 백엔드 - 3
    - 개발 완료 일정 - ~ 7/18 

  - 담당 파트 (정구민 담당 파트) 
    - 프로젝트 초기 세팅 및 백엔드 리딩
      - Spring Boot 초기 설정 담당
      - Entity 초기 설계 담당
    - 회원 인증 기능 담당
      - JWT 토큰을 사용하여 Access Token 발급
      - AuthenticationEntryPoint 를 Custom 구현하여 인증되지 않은 사용자는 401 응답이 내려지도록 설정
      - AccessDeniedHandler 를 Custom 구현하여 리소스 접근 권한이 없는 사용자는 403 응답이 내려지도록 설정
      - 소셜 로그인 기능 구현
        - 카카오 로그인 API 를 통한 사용자 인증 구현
        - 네이버 로그인 API 를 통한 사용자 인증 구현
    - 회원 프로필 관리 기능 담당
      - 프로필 조회
      - 프로필 수정
    - 테마 관련 기능 담당
      - 필터링 조건을 통한 테마 목록 조회
      - 테마 상세 조회
    - 리뷰 관련 기능 담당
      - 리뷰 생성
        - 이미지, 코멘트 등을 기입하지 않는 리뷰 생성
      - 리뷰 상세 정보 추가
        - 이미지, 코멘트 등을 리뷰에 추가
      - 리뷰 설문 추가
        - 리뷰에 테마에 대한 설문을 추가할 수 있는 기능
      - 리뷰 수정
      - 리뷰 상세, 목록 조회
      - 리뷰 삭제 
        - 실제 데이터를 삭제하지 않고 상태 값을 변경하도록 구현
    - 파일 업로드 관련 기능 담당 
      - 파일 업로드 기능 구현
      - 파일 다운로드 기능 구현 
    - 프로젝트 배포 담당 
      - AWS EC2 를 사용하여 프로젝트 배포
      - 로컬, Develop 환경에서의 application.yml 파일 구분
      - Dspring.profiles.active 옵션을 사용하여 배포 환경에 따라 다른 설정 적용
      - 로컬, Devlop DB 를 각각 사용