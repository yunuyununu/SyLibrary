# 📚 3월도서관 및 도서 통합관리 웹서비스
본 프로젝트는 국비지원 훈련과정 중 진행한 두번째 프로젝트입니다.
<br/>
* * *
## 📑 목차
[1. 프로젝트 개요](#-프로젝트-개요)
   - [개발기간](#-개발기간)
   - [주제 및 목표](#-주제-및-목표)
   - [개발환경 및 기술스택](#-개발환경-및-기술스택)
<br/>
[2. 프로그램 구조](#-프로그램-구조)
  - [ER Diagram](#-ER-Diagram)
  - [View](#-View)
  - [Procedure](#-Procedure)
  - [Usecase Diagram](#-Usecase-Diagram)
  - [FLow Chart](#-Flow-Chart)
  - [테이블 명세서](#-테이블-명세서)
<br/>
[3. 3월 도서관 개별 페이지 기능 안내](#-3월-도서관-개별-페이지-기능-안내)
  - [팀원별 구현 기능](#-팀원별-구현-기능)
  - [관리자 화면(통합관리시스템)](#-관리자-화면(통합관리시스템))
  - [사용자 화면(도서관 홈페이지)](#-사용자-화면(도서관-홈페이지))
<br/>
[4. 프로젝트 후기](#-프로젝트-후기)
  - [개선사항 및 후기](#-개선사항-및-후기)
  - [참고 url](#-참고-url)
<br/>
🔗 [프로젠테이션 자료](https://docs.google.com/presentation/d/19Hi8HgZE-Zn88lhW7pmRSJ1mOBWTmTxJ34NunvYbvU4/edit#slide=id.g2696ce6de55_1_555)
<br/>
<br/>
<br/>
<br/>

* * *

## 📌 프로젝트 개요
#### 📅 개발기간
2024.02.08 ~ 2024.03.11 (약 5주)

- 1주차 : 프로젝트 기획 및 DB 구축회의 / 화면설계(파트별 레이아웃 및 핵심 기능 설계)
- 2주차 : 파트별 DB 설계 및 구축 / 개인별 화면 및 모델 개발 작업 진행
- 3주차 : 1차 기능테스트 및 작업현황 공유 / 오류수정
- 4주차 : 2차 기능테스트 / 사이트 오픈 및 최종시연 / 프레젠테이션 준비

<br/>

#### 🖍 주제 및 목표
[주제] : 도서관 및 도서 통합관리 웹

[목표]
1. 1차 프로젝트 후 피드백 반영 및 훈련기간 동안 학습한 내뇬=용 적용
2. 데이터베이스 구축 및 SQL문 연습
3. 뷰, 조인, 프로시저 등의 적극 활용
4. Front-end & Back-end의 다양한 기술스택을 활용한 웹 애플리케이션 구현
<br/>

#### 🛠️ 개발환경 및 기술스택
- OS  :  Windows11
- Tools  :  Eclipse, SQL Developer, SVN
- Front-end  :  HTML/CSS, Javascript
- Back-end  :  JDK21, OracleDB 23.1.1, Java
- Library  :  Lombok 1.18.30, MyBatis 3.5.15, Json, Jquery 3.7.1, JSTL, Ajax, Bootstrap 5.3, Sweetalert2, Chart.js 4.4.0, Apache Tomcat 10.1.19

<br/>
<br/>
<br/>

* * *

## ⚙️ 프로그램 구조
  - [ER Diagram]
![erd](https://github.com/jh91019/android/assets/156145497/fd2e695f-51e4-4f3c-b91a-1421b781315a)
<br/>
  - [View]
![view](https://github.com/jh91019/android/assets/156145497/2425f37d-5358-47a2-be5a-ca54975f7fa3)
<br/>
  - [Usecase Diagram]
![usecase](https://github.com/jh91019/android/assets/156145497/62260a38-3dd1-499a-9b2d-7af892ea42b0)
<br/>
  - [FLow Chart]

**[관리자]**
![flow_admin](https://github.com/jh91019/android/assets/156145497/900737ac-d290-492a-8253-f987fb55572c)

**[회원/비회원]**
![flow](https://github.com/jh91019/android/assets/156145497/e212ed6f-034d-44e5-9a92-001f785a5692)
<br/>

## 📋 개별 페이지 기능 안내
<br/>

### 👥 팀원별 구현 기능
< 팀원 소개 >
- [도경민](https://github.com/mindyhere)
- [박미현](https://github.com/Miihyunee)
- [양미영](https://github.com/didaldud)
- [조연우](https://github.com/yunuyununu)🙌
- [홍재희](https://github.com/jh91019)
![team](https://github.com/jh91019/android/assets/156145497/e90d15c6-c666-4275-9262-df549e33b49c)
<br/>

### 📌 관리자 화면(통합관리시스템)
<br/>

#### ◻️ 메인화면
![admain1](https://github.com/jh91019/android/assets/156145497/9796cc57-cb39-4959-8fef-6dfcd1659ef2)
![admain2](https://github.com/jh91019/android/assets/156145497/22108082-2d6d-44cf-9605-b07e49dcaffa)
![admain3](https://github.com/jh91019/android/assets/156145497/1533f2f1-c36e-4e87-abf4-7c134af82650)
<br/>

#### ◻️ 도서 관리
<br/>

![도서 수정 삭제](https://github.com/jh91019/android/assets/156145497/537df695-60bd-4b06-a8c4-14601855ecfa)
<br/>

[도서 목록/수정/삭제]
- 도서번호, 도서명, 저자, 출판사, 분류별로 검색 가능
- 분류나 검색어가 없을 경우 alert 창으로 알림
- 번호 클릭 시 도서 수정 화면으로 이동
- 삭제 시 한 번 더 묻는 알림창 표시
<br/>

![도서 등록](https://github.com/jh91019/android/assets/156145497/8f83de76-748b-4de4-abc5-41b5fe7a0f87)
<br/>

[도서 등록]
- 전부 입력하지 않으면 각각에 맞춰 알림창이 뜸
- 도서 등록 후 확인을 누르면 목록으로 이동, 취소를 누르면 추가 등록 가능
- 데이터베이스의 SL_BOOK.B_CATEGORY를 불러와서 select 대신 datalist로 처리함 (기존의 분류 선택과 직접 작성 전부 가능) 
<br/>

#### ◻️ 대출 반납
<br/>

![도서 대출 반납 목록](https://github.com/jh91019/android/assets/156145497/194cc700-48bb-4dcb-9271-e64e8aa9a688)
<br/>

[도서 대출/반납 목록]
- 최초 리스트는 가장 최근 대출건부터, 연체일을 누르면 미반납 중에서 연체일이 큰 순서로 정렬
- 연체자에게 반납 요구 연락 가능
- 해당 대출자의 이메일을 기본으로 가져옴 
- 보내는 사람은 도서관 메일로 지정
- 모달의 바깥 부분을 누르거나 X 표시 클릭 시 꺼짐
<br/>

#### ◻️ 대출도서 관리
![대출 도서 관리](https://github.com/jh91019/android/assets/156145497/619c428e-4b5e-48a7-9716-1d538b7459d1)
![reserv](https://github.com/jh91019/android/assets/156145497/ff98eef7-d56b-4ca0-b821-280eccc025b1)
<br/>

#### ◻️ 도서 통계 및 회원 관리
<br/>

### 📌 사용자 화면(도서관 홈페이지)
<br/>

#### ◻️ 메인화면
<br/>
![홈 화면](https://github.com/jh91019/syLibrary/assets/156145497/46c49514-f891-4d8c-a503-cd47cae6ce32)
![회원권한 확인](https://github.com/jh91019/syLibrary/assets/156145497/63f49e93-047a-44d1-954b-1a44035bbc05)
![추천도서](https://github.com/jh91019/syLibrary/assets/156145497/696bad0c-45b0-4595-8471-21b3e5dda34a)
![도서검색](https://github.com/jh91019/syLibrary/assets/156145497/f9d20ef5-a4d5-44ca-bb70-e6a8cbcfcb87)
![도서 상세 정보](https://github.com/jh91019/syLibrary/assets/156145497/1a46c8e9-c7a4-4caf-9199-ebeb79a1fd2a)
![페이지인쇄](https://github.com/jh91019/syLibrary/assets/156145497/05271abf-7c23-4ac2-9772-476493f94260)
![리뷰](https://github.com/jh91019/syLibrary/assets/156145497/d5cd1703-6182-4cc5-be9b-8e6bdca0a8f1)
<br/>

#### ◻️ 회원

![회원가입](https://github.com/jh91019/syLibrary/assets/156145497/ec8a8767-4f7b-4af5-98f2-67b860acfb10)
![로그인](https://github.com/jh91019/syLibrary/assets/156145497/aaf0cec9-6271-4a51-83b0-3b2d0a2c856e)
![아이디 찾기](https://github.com/jh91019/syLibrary/assets/156145497/d086a9a4-303b-4c44-995a-f078fe13faad)
![비밀번호 찾기](https://github.com/jh91019/syLibrary/assets/156145497/c68c1d72-1ad1-4680-ba56-392c1721be30)
![나의 서재](https://github.com/jh91019/syLibrary/assets/156145497/581b27eb-bc3c-4184-838c-340f9c548404)
![회원정보 수정](https://github.com/jh91019/syLibrary/assets/156145497/3e25ba34-10e9-48ba-94a7-76717fd0fafd)

<br/>

#### ◻️ 도서 관리
![대출 중인 도서](https://github.com/jh91019/syLibrary/assets/156145497/825d4746-d87a-449a-ab57-e7bc440ab5bc)
![도서대출내역](https://github.com/jh91019/syLibrary/assets/156145497/752c0723-4d42-42a7-9f22-b3f134fc6c35)
![도서 대출 신청](https://github.com/jh91019/syLibrary/assets/156145497/0428e864-399e-4a97-9a98-0b731850c752)
![도서대출신청](https://github.com/jh91019/syLibrary/assets/156145497/4d294bec-22bc-408b-b5eb-40974629b6b8)
![도서 예약 신청](https://github.com/jh91019/syLibrary/assets/156145497/05cd07ac-36bc-4c9d-a8a0-94c284d6069d)
![예약신청내역](https://github.com/jh91019/syLibrary/assets/156145497/d0c14c1c-3305-418d-81ad-f08f7c83e8b2)
![예약 신청 내역](https://github.com/jh91019/syLibrary/assets/156145497/31095f5a-de20-4c49-b8dc-8a270d89417c)

<br/>

* * *

## 🎓 프로젝트 후기

- DB구축 과정에서 기획부터 다양한 테이블 관계 형성과 프로시저, 뷰를 적극 활용할 수 있도록 노력했고 그 결과 많은 공부가 되었다.
- 협업툴로써  SVN을 활용하여 1차 프로젝트보다 의사소통 및 버전 관리를 더 효율적으로 진행할 수 있었다.
- 팀 프로젝트를 통해 서로 부족한 부분을 채울 수 있는 계기가 되었다.

<br/>

#### 💡 개선사항 및 후기

- 데이터가 바뀔 때마다 화면 깜빡이는 현상 개선
- 검색어 자동 완성 기능 업그레이드
- 온라인 중고 서적 사이트나 도서관 이용 모바일 앱 등으로의 발전
- 도서 정보 오픈 API 활용해보기
- 현업에서 많이 사용하는 Git을 활용해 볼 것을 고려

<br/>
#### 📎 참고 url

- **[노원구립 도서관]**: https://www.nowonlib.kr/
- **[인창 도서관]**: https://www.gurilib.go.kr/inlib/index.do
- **[국립 중앙 도서관]**: https://www.nl.go.kr/
- **[알라딘]**: https://www.aladin.co.kr/home/welcome.aspx
- **[교보문고]**: https://www.kyobobook.co.kr/










## 🕹️ 주요 구현기능 설명
#### __📜 호스트 회원가입 및 승인__
![approve](https://github.com/mindyhere/final-project/assets/147589193/153b76b9-3528-43aa-8bff-5e3f159fcc33 "flow1")
- 호스트 회원가입
  -  각 항목마다 필수 입력 Alert 표시
  -  이메일 유효성 확인 → 중복확인 버튼 활성화 → 사용가능한 이메일에 한해 회원가입 가능
![호스트 회원가입 영상](https://github.com/mindyhere/final-project/assets/147589193/570ed74d-b23d-4676-8d89-33188b9eb6e8)
- 호스트 승인요청
  -    최초 가입 시 “가입 완료” 상태 → 호스트 승인요청 시, 첨부파일 등록 필수(프로필/사업자 등록증/ 통장사본) → 승인요청 버튼 활성화
  - [승인요청] 클릭 시 완료 Alert
- 관리자 - 호스트 가입 승인
  - 신규 회원 승인 대기 상태일 때 [가입승인] 버튼 클릭 후, 사업자등록증, 통장사본 일치 확인 가입정보 일치 → 승인 완료 Alert
![approve1](https://github.com/mindyhere/final-project/assets/147589193/05c332cc-e66b-4257-9113-a34c66fcac6b)

<br/>

#### __🏨 호텔등록 및 영업관리__
![hotel](https://github.com/mindyhere/final-project/assets/147589193/77fc6c98-8df6-4189-a236-e93a445f5236 "flow2")
- 호텔 신규등록
  - 기본정보 입력 후 ‘다음’ 클릭 시 편의시설, 객실정보 입력하는 페이지로 이동
  - 객실 정보 등록 시, 싱글룸은 필수 입력, 객실 사진은 최대 3장까지 첨부 가능
![숙소 등록하기](https://github.com/mindyhere/final-project/assets/147589193/6aa97fe5-4d82-4543-8845-b4f34218ac4c)
- 호텔 등록 : 이어서 작성하기 기능 적
  -  작성 중인 내용이 있을 경우 이어서 작성할 것인지 묻는 Alert
  -  "네” 선택 : 입력했던 데이터 불러온 후 이어서 작성 가능 / “아니오” 선택 : 저장되었던 데이터 삭제, 신규 데이터 입력
![신규호텔_이어서](https://github.com/mindyhere/final-project/assets/147589193/50d8226d-7e40-471e-80c1-4e9a51787a0c)
- 숙소영업관리 및 숙소승인
  - 신규등록호텔이 “승인대기” 상태일 때 → [승인] 버튼 클릭 → “영업중” 상태로 변경
![호텔 등록 승인](https://github.com/mindyhere/final-project/assets/147589193/9af3c403-4cb6-4474-b5ac-41d0bd6ec5dc)

<br/>

#### __📇 숙박예약 및 예약관리__
![reservation](https://github.com/mindyhere/final-project/assets/147589193/5b56dafe-191c-49da-a502-8b3c7d65761d "flow3")
🔗 [숙박예약/결제 시연영상 보기](https://github.com/mindyhere/final-project/assets/147589193/cbf80039-e428-42be-ae34-cf464309f211)
- 포트원API 및 카카오페이 결제API 적용

![ex2](https://github.com/mindyhere/final-project/assets/147589193/4c2f9745-e179-4940-8ad4-893273566ea0)
![ex5](https://github.com/mindyhere/final-project/assets/147589193/8c010fce-1a43-4707-88cd-41238e620c53)
- 호스트 예약관리 : 예약확정/체크인완료 처리 또는 예약변경 승인/거부 처리 → 예약확정 시 바우처 이메일발송

<br/>

#### __📝 후기 및 평점관리__
![reputation](https://github.com/mindyhere/final-project/assets/147589193/f4615140-0746-493b-b973-c18ecb8b512d "flow4")
![reputation1](https://github.com/mindyhere/final-project/assets/147589193/e752f61c-0bed-4d99-b36d-eae9c604c754)

- 게스트
  - 리뷰가 등록되어 있지 않은 지난 여행만 작성 가능 
  - 프로필에서 본인 작성 리뷰 조회 및 수정, 삭제 가능 
  - 호스트가 남긴 답글 조회 가능
- 호스트
  - 해당 호텔의 별점 및 리뷰 상세 조회 가능
  - 답글 등록, 수정, 삭제
- 호텔 상세페이지, 평점 및 후기란에서 조회 가능
  
<br/>

* * *
 
## 🎓 후기
#### __🛠️ 개선사항__
- 깜박임 현상이 잦아 아쉬움. 후 axios(비동기처리)로 개선 필요
- 관리자 자동로그인 기능 추가
- 후기 작성 후 일정기간이 지나면 수정/삭제가 불가능하도록 개선 필요
- 호스트 가입승인 시 가입정보가 일치하지 않으면 ‘승인요청거부’ 메시지가 전달되도록 개선 필요

#### __💡 후기__
- Github를 활용하여 원활한 팀 프로젝트를 진행할 수 있었다.
- 안드로이드를 활용한 숙박예약어플, 관리자-호스트 매출/정산 기능 등 기획단계에서 더 많은 아이디어가 나왔었는데 여건 상 시도하거나 최종 구현하지 못한 부분들이 아쉬움으로 남는다.
- 프로젝트 기획과정에서 다양한 테이블 관계형성과 프로시저, 새로운 프론트엔드(React)를 활용할 수 있도록 노력했고 그 결과 많은 공부가 되었다. 
- 팀 프로젝트를 통해 많이 배우고 부족한 부분을 채워 성장할 수 있는 계기가 되었다. 
<br/>
