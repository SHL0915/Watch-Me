# **프로젝트 개요**

![Watch_Me_시연영상](https://github.com/user-attachments/assets/fca3c408-bf75-42ff-9344-08c5e292894f)

## 프로젝트명
**Watch Me**

## 슬로건
**모든 OTT 콘텐츠를 한 손에!**

## 프로젝트 주제
깔끔하고 편리한 UI와 완전한 OTT 플랫폼의 통합으로 인한 편리성.  
그리고 플랫폼을 뛰어넘어 유저의 시청 기록 및 평가를 통한 학습된 강력한 개인 추천 시스템을 지원하는 어플리케이션.

<br>

## 프로토타입 및 결과물 미리보기
(좌) 프로토타입 / (우) 결과물 메인페이지  
<img width="623" alt="프로토타입" src="https://github.com/user-attachments/assets/eb46c6cf-07e1-4d68-9eab-17893ee0703f" />

<br>

# **팀 소개**

## 팀명
**Watch Me**

## 팀원
| 학번 | 이름 | 역할 |
|------|------|------|
| 201915** | **김*수** | 팀장, Recommender System |
| 202015** | **강*규** | Front-End, Back-End |
| 202115** | **김*건** | Front-End |
| 201917** | **이*형** | Back-End |

## 지도교수 및 멘토
| 역할 | 이름 | 소속 |
|------|------|------|
| 지도교수 | **정영민 교수님** | 서강대학교 |
| 멘토 | **임*환** | NAVER |

<br>

## 협업 방법
- **Github** : 프로젝트 버전 관리  
- **Discord, 카카오톡** : 비대면 커뮤니케이션  
- **Notion** : 프로젝트 일정 및 회의, 멘토링 기록  
- **Flutter Flow** : 어플리케이션 프로토타입 설계  

<br>

- **Github를 통한 프로젝트 버전 관리**  
  <img width="886" alt="깃허브화면" src="https://github.com/user-attachments/assets/4f2ddaf1-6746-4319-b7ff-ee815608138a" />


- **Notion을 통한 작업 현황 및 일정 관리**  
  <img width="980" alt="노션화면" src="https://github.com/user-attachments/assets/7f199b1b-20fe-428a-afc4-17365ff187c8" />

<br>

# **프로젝트 소개**

## 프로젝트 목적
1. **편리하고 쉬운 UI**: 좋은 UI란, 앱에 익숙치 않은 사용자도 빠르고 쉽게 접근할 수 있어야 한다.
2. **플랫폼의 통합화**: 다양한 OTT 플랫폼을 통합하여, 한 번에 콘텐츠를 검색하고 즐길 수 있다.
3. **강력한 추천 시스템**: 하나의 OTT 플랫폼에 국한되지 않고, 각 플랫폼에서의 시청 기록을 기반으로 유저에게 알맞은 콘텐츠를 추천 받을 수 있다.

## 문제 인식
- 시중에 다양한 OTT 플랫폼이 등장하고 있다.
- 그에 따라 콘텐츠의 양이 방대해지고, 사람들의 콘텐츠 추천에 대한 수요가 증가하였다.

## 해결 방안
시청 기록 DB와 추천 시스템을 활용한 플랫폼 통합 어플리케이션 개발.

## 기대 효과
완전한 플랫폼의 통합으로 인한 편리성 증대.

<br>

# **프로젝트 구조**

## 프로젝트 전체 구조
<img width="452" alt="프로젝트구조" src="https://github.com/user-attachments/assets/f88d280f-902a-4cb4-87d6-dc8fdf97ee49" />


## 추천 시스템 구조
<img width="719" alt="추천시스템구조" src="https://github.com/user-attachments/assets/d602bea0-a32c-4a2f-9e9a-cbb640779052" />


<br>

# **프로젝트 내용**

## SW 구조 및 구성요소

Watch me 앱의 목표는 OTT 플랫폼을 통합하고, 이에 따른 개인화된 추천 시스템을 운영하는 것이다.  앱의 개발과정에서의 구성 요소는 크게 실제적인 사용자들에게 화면을 보여주고, 앱의 기능을 제공하는 프론트엔드 부분과, 요청에 따라 DB를 관리하고 통신하며, 추천 시스템과의 연결까지 고려하며 구현되는 백엔드, 그리고 백엔드에서 사용자들 각각에 대한 정보와 검색 쿼리에 따라 개인화된 추천을 제공하는 추천 시스템 부분 총 3가지로 나눌 수 있다.

앱의 개발을 시작하기에 앞서, 각각 SW 개발에 대한 구조를 어느 정도 파악하고 들어갔다. 백엔드는 추천 시스템과 DB 그리고 프론트엔드와의 연결에 대해서 어떤 식으로 통신할 것이고, 각각에 대해서 어떤 프레임워크로 작성할 지에 대해 구조를 신경 썼다. 프론트엔드는 flutter /android studio로 이용한 개발로 먼저 확정이 지어진 상태로 시작하였고, 어떤 기능들이 필요하고, 어떤 화면들이 실제 앱에서 구동되어야 하는지를 화면 전환도를 그려 미리 계획하였다. 앱의 프로토 타입은 flutter flow를 이용하여 만들기로 하였다. 추천 시스템은 하이브리드 추천을 적용시키기로 정했고, 관련 논문과 baseline 코드를 통해, 우리 앱에 알맞게 수정하여 구현기로 하였다.

아래는 개발 계획 단계에서의 백엔드와 프론트엔드의 전체적인 구상도이다.

![앱_구조도2](https://github.com/user-attachments/assets/b371fa4e-3181-486b-b311-56bd17a06458)

<img width="452" alt="프로젝트구조" src="https://github.com/user-attachments/assets/538c4ff3-203b-4819-bd53-87462f10dcb5" />


## 설계 주요 고려사항 및 개발항목

Watch me 앱의 주요 기능은 크게 2가지로 나눌 수 있다. OTT 플랫폼들의 통합과 함께 통합된 콘텐츠 데이터를 이용한 개인 맞춤 추천이 주요한 기능이다. 이러한 기능들을 구현하기 위해서는 우선적으로 영화와 OTT 플랫폼들에 대한 정보를 수집해야 했다. 개발 전에 각 OTT 플랫폼들은 관련된 API를 따로 제공하지 않는 것으로  확인했었기 때문에, 전체적인 데이터를 수집할 수 있는 방법을 고민하게 되었다. 우리가 필요한 주요한 정보는 다음과 같은 것들이 있었다. OTT 플랫폼들을 통합하기 위해서 우선적으로 어떠한 영화에 대해서, 그 영화를 시청할 수 있는 OTT들을 찾아야 했다. 또한 영화를 모바일 애플리케이션 화면에 표시하기 위해서는, 그 영화에 대한 여러 정보가 필요하다. 예를 들면, 영화의 제목, 포스터 이미지, 감독과 배우등이 필요하였다. 처음에 개발에 들어가기에 앞서서는 데이터 스크래핑을 통하여 정보를 얻은 후 DB에 순차적으로 저장하고, 백엔드 서버에서 특정 주기마다 데이터 스크래핑을 통해 데이터를 갱신하는 방식을 취하려 했었다. 개발을 이어나가게 되면서 tmdb와 키노라이츠등의 api를 활용하여 데이터를 수집하는 방식으로 전환하였다. 아래는 API 호출하여 데이터를 확보하는 실제 화면이다.

![줄거리_토큰1](https://github.com/user-attachments/assets/e3331c71-6f09-4bf4-b1c0-41ae327a8b1f)


이렇게 얻게 된 영화에 관련된 데이터는 크게 두가지 부분에서 사용된다. 우선 백엔드에서 db에 관련된 데이터를 json 형식으로 저장하고 있다. 프로트엔드에서는 영화의 포스터 이미지와 함께 실제로 화면에 표시해야 한다. 이를 위하여 fastapi를 사용하여 http api로 백엔드와 소통하여 정보를 주고받고, 실제 화면에 표시한다. 추천 시스템에서도 이러한 데이터들을 활용한다. 각 영화의 줄거리를 자연어 처리를 통해 정제한 후, 유사도를 파악함으로써 하이브리드 된 추천 시스템에서 콘텐츠 기반 추천 부분의 기반이 된다. 또한 이러한 자연어 처리를 통해 유사도를 분석함으로써, 각 영화와 비슷한 영화에 대한 학습이 진행될 수 있었다.  tmdb api에서는 각 영화를 별점을 매긴 사람 수와 함께 평균 별점이 제공된다. 우리 앱에서는 개인별 추천 시스템과 동시에 일반적인 추천도 적용하는데 이에 활용되었다.  아래는 관련 화면이다.

<img width="451" alt="줄거리_토큰2" src="https://github.com/user-attachments/assets/c4b46fee-4ddd-47ba-a5fc-016c8d0067ff" />


이러한 줄거리에 대한 것들은 검색 시스템에도 포함되어 키워드를 포함한 검색 또한 가능하게 하였다. 아래는 배우와 장르를 검색시스템에 활용하여 올바른 결과가 검색된 화면이다.

<img width="728" alt="키워드검색" src="https://github.com/user-attachments/assets/f17d552f-0f4d-4f14-8bca-632acb19a458" />


OTT를 토글링하는 방식으로 OTT들에 대한 필터링을 진행하였다. 이에 총 6가지 플랫폼들에 대해서 원하는 플랫폼만에 대한 추천과 메인화면이 구성되게 된다. 이러한 각 OTT들에 대한 선택 정보는 프론트엔드와 백엔드간의 정보를 주고받으면서, 사용자의 토글링 상태를 프론트엔드가 백엔드에 관련 요청을 보냄으로써 백엔드에서는 각 OTT들에 대한 선택 상태를 고려해 메인 화면에 구성될 영화들을 넘기게 된다.  

이러한 각 OTT들에 대한 선택 상태를 메인 화면에서 관리하고자 결정했다. 앱은 프론트엔드 상에서 크게 5가지 화면으로 구성된다. 로그인 페이지, 메인 페이지, 상세 페이지, 마이 페이지, 검색 페이지로 구성된다. 첫 설계에서는 추천 페이지도 포함되었으나, 후에 메인 화면에 추천 영화를 함께 포함하는 방식으로 화면 구현을 변경했다. 나머지 전체적인 화면 전환의 구성 흐름은 설계했던 것과 동일하게 적용하였다. 상세 페이지에서는 그 영화를 시청할 수 있는 OTT 플랫폼들을 나열하여 보여주었고, 각 OTT를 누르면 내 모바일 환경에서 그 OTT 플랫폼의 링크로 직접 이동되도록 구현하였다.

![보러가기-2](https://github.com/user-attachments/assets/06b6fca0-cfea-4e8c-aa83-284fe969bb62)


상세 페이지에서는 평가 버튼을 누르면 영화에 대한 별점과 코멘트를 남길 수 있는데, 이는 백엔드 서버에 연결되어 추천 시스템과 적용된다. 각 유저가 어떠한 영화에 대해 남긴 별점을 분석하여 개인화된 추천 시스템이 업데이트 된다.

![평가남기기-2](https://github.com/user-attachments/assets/0d53e663-45b6-4f5e-a170-90687224d322)

아래는 특정 유저의 별점과 평가에 따라서 각 유저의 추천되는 콘텐츠들이 실제로 어떻게 달라졌는지를 보여주는 화면이다. 위 화면은, 배우 박보영의 로맨스/드라마 영화에 대해서 높은 별점을 준 유저의 추천 영화 항목이고 아래는 배우 마동석의 액션 영화에 대해 높은 별점을 준 유저의 추천 영화 항목이다.

<img width="334" alt="박보영추천-2" src="https://github.com/user-attachments/assets/3db4bc5b-12ad-4a97-aba5-63f6424f3b57" />

<img width="343" alt="마동석추천-2" src="https://github.com/user-attachments/assets/9c20b31e-4ecc-471d-ada0-f491ec6f5e2d" />


이러한 내용들을 통합하여 watch-me 앱을 설계 및 구현 완료하였다.

# 프로젝트 결과물

## 목차
- 최종 결과
- 메인 페이지 OTT 필터링
- 검색 페이지 OTT 필터링
- 키워드 검색 기능
- 개인별 추천 시스템
- OTT 서비스와의 연동

<br>

## 최종 결과

<img width="950" alt="결과물" src="https://github.com/user-attachments/assets/4ded8320-fb82-48f4-87d1-d124bea14013" />


<br><br>

## 메인 페이지 OTT 필터링

<img width="730" alt="메인필터링" src="https://github.com/user-attachments/assets/d040d3fb-a945-4f4f-b189-8142a857a4dd" />


**(좌) Netflix On, (우) Netflix Off**  
서울의 봄, 오펜하이머의 경우 Netflix에만 있는 작품이다.  
따라서 상단의 Netflix 버튼을 토글하여 Off하면 오른쪽 사진과 같이 Netflix에만 있는 작품들은 Display되지 않는다.  

<br><br>

## 검색 페이지 OTT 필터링
<img width="730" alt="검색필터링" src="https://github.com/user-attachments/assets/f0f63000-14fa-4db2-82c5-8b3efd30c407" />


**(좌) ALL On, (우) 티빙 & 디즈니+ Off**  
마동석 배우 검색 결과이다.  
범죄도시의 경우 티빙 혹은 디즈니+에만 존재하여서, 검색 후 Tving 또는 Disney+ 버튼을 토글링하여 Off한 경우, 범죄도시는 검색결과에서 사라지게 된다.  

<br><br>

## 키워드 검색 기능

<img width="728" alt="키워드검색" src="https://github.com/user-attachments/assets/42fc0770-5d4c-497c-826e-7dd0382cb489" />

**(좌) '황정민 모험' 검색 결과, (우) '이하늬 코미디' 검색 결과**  

위 키워드 검색 기능의 경우 검색 쿼리가 들어왔을 때, CountVectorizer를 이용하여 문자를 유사도 행렬으로 변경하였다.  
이때, 감독과 배우진의 중요도를 올리기 위해 Naive하게 감독 이름과 배우 이름을 여러 번 반복하여 CountVectorizer에서의 점수를 높이는 방식을 이용하였다.  
해당 유사도 행렬을 이용하여 코사인 유사도를 적용시켜 검색 쿼리가 들어왔을 때, 가장 유사한 상위 몇 개의 작품을 골라내고 그 중에서 인기도 있는 작품 순으로 정렬하였다.  

<br><br>

## 개인별 추천 시스템
<img width="730" alt="카카오로그인" src="https://github.com/user-attachments/assets/cb7619ae-a7f1-4b54-a2d0-d92e40840205" />


개인화 추천 기능을 제공하기 위해, 카카오계정을 이용한 로그인 기능이 제공된다.  
또, 우측 화면과 같이 각 영화별로 리뷰를 남길 수 있는 기능을 제공한다.  
아래는 그 후의 메인 페이지 결과이다.  

<br><br>
<img width="733" alt="추천시스템" src="https://github.com/user-attachments/assets/195b2c54-aefb-4d5e-b52a-543c2da94203" />



왼쪽 화면의 경우 아무런 추천이 적용되지 않은 상태로, 인기 순위와 유사하게 컨텐츠들이 추천되고 있다.  
우측 화면의 경우 범죄도시 1, 2, 3에 대한 평점 5점을 제출한 후의 결과로, 범죄도시의 주연 배우인 마동석 배우가 출연하는 영화들이 추천되고 있는 모습을 볼 수 있다.  

추천 시스템의 경우, 기본적으로 콘텐츠 기반 필터링과 협업 필터링을 결합한 하이브리드 추천 시스템을 사용하였다.  
- **콘텐츠 기반 필터링**: 콘텐츠의 메타데이터(제목, 줄거리, 감독, 배우진 등)를 이용하여 유사한 작품을 추천하는 방식  
- **협업 필터링**: 나와 유사한 취향을 가진 사람들이 좋은 평점을 남긴 작품을 추천하는 방식  

추천 시스템은 위 2가지 방식을 결합하여 유저의 시청 기록 및 남긴 평점을 기반으로 유저 개개인마다의 추천 목록을 제공하는 방식으로 구현하였다.  

<br><br>

## OTT 서비스와의 연동
<img width="292" alt="연동" src="https://github.com/user-attachments/assets/3bfdf2d7-7c19-4b12-be69-b07311c458c4" />


각 컨텐츠의 디테일 페이지에서 시청 가능한 OTT의 리스트들을 확인할 수 있다.  
클릭 시에는 바로 해당 OTT 어플리케이션으로 넘어가게 된다.  


## 향후 개선 방안 및 보완 사항

### 서버 스펙 이슈로 인한 보완사항
현재 가용 가능한 서버 스펙 상 너무 많은 작품과 많은 데이터를 감당할 수 없어서 현재 영화에 대해서만 작품리스트 및 추천 기능을 제한한 상태이다.  
추후에 서버 스펙을 업그레이드할 수 있다면 드라마, 예능 및 스포츠 더 나아가 웹 소설, 웹툰, 책 과 같은 콘텐츠들까지 범위를 확장하여 앱의 사용성을 증가시킬 수 있을 것이다.  

### DB 변경을 통한 쿼리 속도 개선
현재 영화 정보와 사용자 평가 정보를 보관하는 DB로 검색 엔진인 Elasticsearch를 선택하여 사용하고 있다. 그러나, 상세 구현을 진행한 결과 Elasticsearch로 query하기 전 추천 시스템 모델의 도움을 받아 줄거리나 키워드 검색을 Elasticsearch의 색인, 역색인 기능을 이용하여 진행하고 있지 않고, 작품의 ID만을 이용하여 쿼리하고 있는 상태이다.  
즉, DB로써 Elasticsearch를 고집해야 하는 필요성이 옅어졌고, 이에 따라 읽기/쓰기 연산에 더욱 최적화된 key-value 기반의 NoSQL 저장소(ex. Amazon DynamoDB)와 같은 데이터베이스의 도입을 고려해볼 법하다. 

### 향후 계획
현재는 단순히 평가 및 평점을 남기는 기능을 제공하고 있는데, 유저 본인이 본 시청 목록과 남긴 리뷰 및 평점에 대한 데이터를 유저가 쉽게 탐색 및 관리할 수 있도록 마이페이지 및 평점 부분의 기능을 개선시킬 계획이 있다.  
또한 이를 SNS처럼 사람들이 남긴 평점 및 한줄평을 볼 수 있게 만들고 퀄리티가 높은 리뷰를 달아주는 유저들에게는 보상 및 Celebrity와 같이 만들어 평점을 유저들이 잘 남길 수 있는 재미와 동기를 부여하도록 할 계획이 있다.  

# **프로젝트 기록**

## 회의록 및 멘토링
[회의록 및 멘토링 정리본](https://quill-bulb-27c.notion.site/38c60ef591524f6fa592374f2ba8ac09)

## 발표자료
- 제안발표: [Watch-Me_제안_발표.pptx](https://github.com/user-attachments/files/18871591/Watch-Me_._.pptx)  
- 중간발표: [Watch-Me_중간_발표.pptx](https://github.com/user-attachments/files/18871593/Watch-Me_._.pptx)  
- 최종발표: [Watch-Me_최종_발표.pptx](https://github.com/user-attachments/files/18871590/Watch-Me_._.pptx) / [Watch-Me 최종 발표(구글 슬라이드)](https://docs.google.com/presentation/d/1NhUGDlvh8zAaRte0kignFLydAL6fmD3GBPKEaSO7A60/edit?usp=sharing)

## 최종 보고서
- [Watch_Me_최종보고서.docx](https://github.com/user-attachments/files/18871592/Watch_Me_.docx)  
- [Watch_Me_최종보고서.pdf](https://github.com/user-attachments/files/18871594/Watch_Me_.-3.pdf)
