# 📚 3월도서관 및 도서 통합관리 웹서비스
본 프로젝트는 국비지원 훈련과정 중 진행한 두번째 프로젝트입니다.


* * *

## 📑 목차


[1. 프로젝트 개요](#-프로젝트-개요)
   - [개발기간](#-개발기간)
   - [주제 및 목표](#-주제-및-목표)
   - [개발환경 및 기술스택](#-개발환경-및-기술스택)


[2. 프로그램 구조](#-프로그램-구조)
   - [ER Diagram](#-ER-Diagram)
   - [View](#-View)
   - [Procedure](#-Procedure)
   - [Usecase Diagram](#-Usecase-Diagram)
   - [FLow Chart](#-Flow-Chart)
   - [테이블 명세서](#-테이블-명세서)


[3. 개별 페이지 기능 안내](#-개별-페이지-기능-안내)
   - [팀원별 구현 기능](#-팀원별-구현-기능)
   - [관리자 화면](#-관리자-화면)
   - [사용자 화면](#-사용자-화면)


[4. 프로젝트 후기](#-프로젝트-후기)
   - [개선사항 및 후기](#-개선사항-및-후기)
   - [참고 url](#-참고-url)


🔗 [프로젠테이션 자료](https://docs.google.com/presentation/d/19Hi8HgZE-Zn88lhW7pmRSJ1mOBWTmTxJ34NunvYbvU4/edit#slide=id.g2696ce6de55_1_555)


* * *


## 📌 프로젝트 개요


#### 📅 개발기간
   2024.02.08 ~ 2024.03.11 (약 5주)

- 1주차 : 프로젝트 기획 및 DB 구축회의 / 화면설계(파트별 레이아웃 및 핵심 기능 설계)
- 2주차 : 파트별 DB 설계 및 구축 / 개인별 화면 및 모델 개발 작업 진행
- 3주차 : 1차 기능테스트 및 작업현황 공유 / 오류수정
- 4주차 : 2차 기능테스트 / 사이트 오픈 및 최종시연 / 프레젠테이션 준비


#### 🖍 주제 및 목표


**[주제]**


도서관 및 도서 통합관리 웹

**[목표]**
1. 1차 프로젝트 후 피드백 반영 및 훈련기간 동안 학습한 내뇬=용 적용
2. 데이터베이스 구축 및 SQL문 연습
3. 뷰, 조인, 프로시저 등의 적극 활용
4. Front-end & Back-end의 다양한 기술스택을 활용한 웹 애플리케이션 구현


#### 🛠️ 개발환경 및 기술스택


- OS : Windows11


- Tools : Eclipse, SQL Developer, SVN


- Front-end : HTML/CSS, Javascript


- Back-end : JDK21, OracleDB 23.1.1, Java


- Library : Lombok 1.18.30, MyBatis 3.5.15, Json, Jquery 3.7.1, JSTL, Ajax, Bootstrap 5.3, Sweetalert2, Chart.js 4.4.0, Apache Tomcat 10.1.19


* * *


## ⚙️ 프로그램 구조


### [ER Diagram]
![erDiagram](https://github.com/Miihyunee/LibraryinMarch/assets/151993240/4ce6cca0-29a9-4622-9053-7c1650431234)


### [View]
![view](https://github.com/Miihyunee/LibraryinMarch/assets/151993240/a5d8b2cf-63eb-4e81-b617-1d63277b5ef6)


### [Usecase Diagram]
![usecase](https://github.com/jh91019/android/assets/156145497/62260a38-3dd1-499a-9b2d-7af892ea42b0)


### [FLow Chart]


**[관리자]**
![flow_admin](https://github.com/jh91019/android/assets/156145497/900737ac-d290-492a-8253-f987fb55572c)


**[회원/비회원]**
![flow](https://github.com/jh91019/android/assets/156145497/e212ed6f-034d-44e5-9a92-001f785a5692)


## 📋 개별 페이지 기능 안내


### 👥 팀원별 구현 기능
< 팀원 소개 >
- [도경민](https://github.com/mindyhere)
- [박미현](https://github.com/Miihyunee)
- [양미영](https://github.com/didaldud)
- [조연우](https://github.com/yunuyununu)🙌
- [홍재희](https://github.com/jh91019)


![team](https://github.com/jh91019/android/assets/156145497/e90d15c6-c666-4275-9262-df549e33b49c)


### 📌 관리자 화면 (통합관리시스템)


#### ◻️ 메인화면


![admain1](https://github.com/jh91019/android/assets/156145497/9796cc57-cb39-4959-8fef-6dfcd1659ef2)

[관리자 로그인]
- 관리자 아이디/비밀번호 틀리면 alert창. 맞으면 메인화면으로 화면전환


![admain2](https://github.com/jh91019/android/assets/156145497/22108082-2d6d-44cf-9605-b07e49dcaffa)

[관리자 메인화면]
- 로그인 상태 : 세션에 저장된 관리자 로그인 상태 띄워짐
- 헤더아이콘 : 클릭 시 메인페이지로 이동
- 헤더, 풋터, 메뉴바 : 고정된 컴포넌트. 메뉴 클릭 시 해당 페이지 콘텐트 안에 띄워짐
- 오른쪽 상단 버튼 : 이용자 페이지로 이동. 로그아웃 시 alert창으로 확인 후 로그인페이지로 이동(세션 삭제됨)

![admain3](https://github.com/jh91019/android/assets/156145497/1533f2f1-c36e-4e87-abf4-7c134af82650)

[관리자 메인화면 상세]
- 달력 : 현재날짜 동그라미 표시됨. 옵션창으로 날짜 조회 가능
- 메모리스트 : 현재 등록된 메모 리스트로 보여짐
- 메모등록 : 메모작성칸에 입력 후 등록버튼 누르면 리스트에 바로 메모 등록됨. 현재 세션에 저장된 작성자 자동 등록
- 메모 수정/삭제 : 모달창을 이용해 메모 상세확인 및 수정 가능. 삭제 시 한번더 alert창으로 확인 후 삭제됨

#### ◻️ 도서 관리


![도서 수정 삭제](https://github.com/jh91019/android/assets/156145497/537df695-60bd-4b06-a8c4-14601855ecfa)


[도서 목록/수정/삭제]
- 도서번호, 도서명, 저자, 출판사, 분류별로 검색 가능
- 분류나 검색어가 없을 경우 alert 창으로 알림
- 번호 클릭 시 도서 수정 화면으로 이동
- 삭제 시 한 번 더 묻는 알림창 표시


![도서 등록](https://github.com/jh91019/android/assets/156145497/8f83de76-748b-4de4-abc5-41b5fe7a0f87)


[도서 등록]
- 전부 입력하지 않으면 각각에 맞춰 알림창이 뜸
- 도서 등록 후 확인을 누르면 목록으로 이동, 취소를 누르면 추가 등록 가능
- 데이터베이스의 SL_BOOK.B_CATEGORY를 불러와서 select 대신 datalist로 처리함 (기존의 분류 선택과 직접 작성 전부 가능) 


#### ◻️ 대출 반납


![도서 대출 반납 목록](https://github.com/jh91019/android/assets/156145497/194cc700-48bb-4dcb-9271-e64e8aa9a688)


[도서 대출/반납 목록]
- 최초 리스트는 가장 최근 대출건부터, 연체일을 누르면 미반납 중에서 연체일이 큰 순서로 정렬
- 연체자에게 반납 요구 연락 가능
- 해당 대출자의 이메일을 기본으로 가져옴 
- 보내는 사람은 도서관 메일로 지정
- 모달의 바깥 부분을 누르거나 X 표시 클릭 시 꺼짐


#### ◻️ 대출도서 관리


![대출 도서 관리](https://github.com/jh91019/android/assets/156145497/619c428e-4b5e-48a7-9716-1d538b7459d1)


![reserv](https://github.com/jh91019/android/assets/156145497/ff98eef7-d56b-4ca0-b821-280eccc025b1)


#### ◻️ 도서 통계 및 회원 관리

     
![도서 통계](https://github.com/Miihyunee/LibraryinMarch/assets/151993240/3b72d358-5239-4355-ae84-62ff7dba883b)

[도서 이용 통계]
- 현재 날짜 기준 대출 수량 통계그래프(막대/원형)
- chart.js 사용
- 차트 데이터 추출을 위해 가각의 뷰 생성
- DAO에서 List map으로 받은 데이터를 JSONObject로 변환하여 차트로 보냄
- 화면 로딩과 동시에 차트/테이블 생성 함수를 호출함

![member](https://github.com/jh91019/android/assets/156145497/ccad5cc9-5079-4fc9-9bfd-cbd8f9e885cb)

[회원 정보]
- 회원정보 리스트 출력
- 분류 선택 시 해당 내용 검색 가능
- 상세 클릭 시 회원 상세 정보 페이지로 넘어감

[회원 상세정보]
- 회원 상세 정보와 대출/예약 가능 권수 확인 가능
- 대출 현황이 리스트로 띄워짐

### 📌 사용자 화면 (도서관 홈페이지)


#### ◻️ 메인화면


![홈 화면](https://github.com/jh91019/syLibrary/assets/156145497/46c49514-f891-4d8c-a503-cd47cae6ce32)


![회원권한 확인](https://github.com/jh91019/syLibrary/assets/156145497/63f49e93-047a-44d1-954b-1a44035bbc05)


![추천도서](https://github.com/jh91019/syLibrary/assets/156145497/696bad0c-45b0-4595-8471-21b3e5dda34a)


![도서검색](https://github.com/jh91019/syLibrary/assets/156145497/f9d20ef5-a4d5-44ca-bb70-e6a8cbcfcb87)


![도서 상세 정보](https://github.com/jh91019/syLibrary/assets/156145497/1a46c8e9-c7a4-4caf-9199-ebeb79a1fd2a)


![페이지인쇄](https://github.com/jh91019/syLibrary/assets/156145497/05271abf-7c23-4ac2-9772-476493f94260)


![리뷰](https://github.com/jh91019/syLibrary/assets/156145497/d5cd1703-6182-4cc5-be9b-8e6bdca0a8f1)


#### ◻️ 회원


![회원가입](https://github.com/jh91019/syLibrary/assets/156145497/ec8a8767-4f7b-4af5-98f2-67b860acfb10)


![로그인](https://github.com/jh91019/syLibrary/assets/156145497/aaf0cec9-6271-4a51-83b0-3b2d0a2c856e)


![아이디 찾기](https://github.com/jh91019/syLibrary/assets/156145497/d086a9a4-303b-4c44-995a-f078fe13faad)


![비밀번호 찾기](https://github.com/jh91019/syLibrary/assets/156145497/c68c1d72-1ad1-4680-ba56-392c1721be30)


![나의 서재](https://github.com/jh91019/syLibrary/assets/156145497/581b27eb-bc3c-4184-838c-340f9c548404)


![회원정보 수정](https://github.com/jh91019/syLibrary/assets/156145497/3e25ba34-10e9-48ba-94a7-76717fd0fafd)


#### ◻️ 도서 관리


![대출 중인 도서](https://github.com/jh91019/syLibrary/assets/156145497/825d4746-d87a-449a-ab57-e7bc440ab5bc)


![도서대출내역](https://github.com/jh91019/syLibrary/assets/156145497/752c0723-4d42-42a7-9f22-b3f134fc6c35)


![도서 대출 신청](https://github.com/jh91019/syLibrary/assets/156145497/0428e864-399e-4a97-9a98-0b731850c752)


![도서대출신청](https://github.com/jh91019/syLibrary/assets/156145497/4d294bec-22bc-408b-b5eb-40974629b6b8)


![도서 예약 신청](https://github.com/jh91019/syLibrary/assets/156145497/05cd07ac-36bc-4c9d-a8a0-94c284d6069d)


![예약신청내역](https://github.com/jh91019/syLibrary/assets/156145497/d0c14c1c-3305-418d-81ad-f08f7c83e8b2)


![예약 신청 내역](https://github.com/jh91019/syLibrary/assets/156145497/31095f5a-de20-4c49-b8dc-8a270d89417c)


* * *


## 🎓 프로젝트 후기


- DB구축 과정에서 기획부터 다양한 테이블 관계 형성과 프로시저, 뷰를 적극 활용할 수 있도록 노력했고 그 결과 많은 공부가 되었다.
- 협업툴로써 SVN을 활용하여 1차 프로젝트보다 의사소통 및 버전 관리를 더 효율적으로 진행할 수 있었다.
- 팀 프로젝트를 통해 서로 부족한 부분을 채울 수 있는 계기가 되었다.


#### 💡 개선사항 및 후기


- 데이터가 바뀔 때마다 화면 깜빡이는 현상 개선
- 검색어 자동 완성 기능 업그레이드
- 온라인 중고 서적 사이트나 도서관 이용 모바일 앱 등으로의 발전
- 도서 정보 오픈 API 활용해보기
- 현업에서 많이 사용하는 Git을 활용해 볼 것을 고려


#### 📎 참고 url


- **[노원구립 도서관]**: https://www.nowonlib.kr/
- **[인창 도서관]**: https://www.gurilib.go.kr/inlib/index.do
- **[국립 중앙 도서관]**: https://www.nl.go.kr/
- **[알라딘]**: https://www.aladin.co.kr/home/welcome.aspx
- **[교보문고]**: https://www.kyobobook.co.kr/

