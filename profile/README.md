<details>
  <summary>📌 목차</summary>  
  
## [1. 프로젝트 소개](#1-프로젝트-소개)<br/>
  ###### [1.1 프로젝트 개요](#11-프로젝트-개요)<br/>
  ###### [1.2 서비스 목적 및 배경](#12-서비스-목적-및-배경)<br/>
  ###### [1.3 핵심 기능 요약](#13-핵심-기능-요약)<br/>

## [2. 주요 기능](#2-주요-기능)<br/>
  ###### [2.1 기능 목록](#21-기능-목록)<br/>
  ###### [2.2 각 기능 설명](#22-각-기능-설명)<br/>

## [3. 기술 스택 및 아키텍처](#3-기술-스택-및-아키텍처)<br/>
  ###### [3.1 주요 기술 스택](#31-주요-기술-스택)<br/>
  ###### [3.2 ERD](#32-erd)<br/>
  ###### [3.3 시스템 구성도](#33-시스템-구성도)<br/>
  ###### [3.4 프로젝트 폴더 구조](#34-프로젝트-폴더-구조)<br/>

## [4. 프로젝트 결과물](#4-프로젝트-결과물)<br/>
  ###### [4.1 서비스 화면 및 기능 시연](#41-서비스-화면-및-기능-시연)<br/>
  ###### [4.2 성능 최적화--테스트 전략](#42-성능-최적화--테스트-전략)<br/>
  ###### [4.3 사용자 피드백](#43-사용자-피드백)<br/>
  ###### [4.4 트러블 슈팅(문제발생, 해결방안, 결과)](#44-트러블-슈팅문제발생-해결방안-결과)<br/>

## [5. 개발 일정 및 마일스톤](#5-개발-일정-및-마일스톤)<br/>
## [6. 회고 및 향후 개선 방향](#6-회고-및-향후-개선-방향)<br/>
## [7. 팀원 소개 및 역할 분담](#7-팀원-소개-및-역할-분담)<br/>
## [8. 프로젝트 산출물](#8-프로젝트-산출물)<br/>
## [9. 협업 환경 & 툴](#9-협업-환경--툴)<br/>
## [10. 협업 컨벤션 / 절차](#10-협업-컨벤션--절차)<br/>
  ###### [10.1 JIRA 사용 흐름](#101-jira-사용-흐름)<br/>
  ###### [10.2 GIT 컨벤션](#102-git-컨벤션)<br/>
  ###### [10.3 기타 규칙(코드리뷰, PR 템플릿 등)](#103-기타-규칙코드리뷰-pr-템플릿-등)<br/>

<hr/>
</details>

# 👋 Welcome to U-HYU
## 1. 프로젝트 소개
### 1.1 프로젝트 개요
주변 멤버십 혜택을 지도로 찾고, 다른 사람들의 이용 현황과 나만의 매장 리스트를 공유하는 지도 플랫폼
### 1.2 서비스 목적 및 배경
> LG U+ 멤버십 생태계는 구조적으로 많은 혜택을 보유하고 있음에도, 실제 사용자 활용률은 매우 저조한 상태입니다.<br/>
> 조사에 따르면 멤버십 미사용의 가장 큰 이유는 “사용법을 몰라서”(42%), 또는 “어디서 쓸 수 있는지 몰라서”인 경우가 많습니다.<br/>
  복잡한 앱 구조와 정적인 혜택 안내 방식은 사용자 접근성을 떨어뜨리고 있으며, 최근 5년간 233억 원의 포인트가 소멸될 정도로 심각한 활용률 저하 문제가 있습니다. <br/>
> 동시에, 모바일 쿠폰과 위치기반 O2O 시장은 성장 중이며, 디지털 쿠폰 사용률은 33.3%, 종이 쿠폰(24.2%)보다 1.4배 높은 효율성을 보이고 있습니다.<br/>

> [!IMPORTANT]
> 이를 해결하고자 **본 프로젝트는 사용자 중심의 위치 기반 혜택 탐색과 공유 중심의 새로운 멤버십 플랫폼을 제안**합니다.

### 1.3 핵심 기능 요약
| 기능 | 설명 |
|:--|:--|
| **1️⃣ 지도 기반 혜택 탐색** | 사용자의 현재 위치를 기준으로 1km 반경 내 제휴처를 시각화하고, 복잡한 앱 탐색 없이 직관적으로 혜택을 탐색. |
| **2️⃣ 맞춤형 제휴처 추천** | 사용자의 제휴처 이용 이력과 선호 콘텐츠 특성을 분석해 개인화된 제휴 혜택을 추천.|
| **3️⃣ My Map** | 사용자가 직접 만든 제휴처 리스트(데이트 코스, 혼밥 맛집 등)를 저장 및 공유할 수 있는 지도 공유 기능. |
| **4️⃣ U+ FootPrint** | 실시간 활동 마커로, 타인의 이용 이력을 바탕으로 혜택을 발견. |
| **5️⃣ 제휴혜택 리스트** | 제휴처의 혜택을 자세하게 확인. |


## 2. 기능
<table>
  <tr>
    <th>🏠 메인 페이지</th>
    <td>
      • 개인화된 맞춤 제휴처 추천 (행동/검색/위치 기반 알고리즘)<br/>
      • 내 주변 제휴처 실시간 확인<br/>
      • 내 멤버십 등급(VIP/VVIP 등)에 따른 혜택 안내<br/>
      • 내 멤버십 바코드 등록 및 어디서든 혜택 사용 지원 (플로팅 버튼)
    </td>
  </tr>
  <tr>
    <th>🗺️ 지도 페이지</th>
    <td>
      • 현재 위치 중심으로 제휴 매장 마커 시각화 및 혜택 정보 팝업 제공<br/>
      • 카테고리 및 브랜드 2중 필터링<br/>
      • 확대 단계에 따라 클러스터링 UI 제공
    </td>
  </tr>
  <tr>
    <th>🗂️ MyMap</th>
    <td>
      • 테마별 폴더 생성 (예: 데이트코스, 혼밥 맛집 등)<br/>
      • 매장 저장, 수정, 삭제 및 외부 공유 링크(URL) 생성<br/>
      • 공유 링크 클릭 시 해당 매장 지도뷰 진입 및 포커스
    </td>
  </tr>
  <tr>
    <th>📍 U+ FootPrint</th>
    <td>
      • 최근 방문 유저의 마커 자동 표시 (닉네임/방문시간)<br/>
      • 개인정보 동의 기반 마커 공유<br/>
      • 마커 클릭 시 방문 히스토리 및 혜택 안내 팝업
    </td>
  </tr>
  <tr>
    <th>👤 개인화 기능</th>
    <td>
      • 할인 받은 금액, 관심 브랜드/카테고리 관리<br/>
      • 즐겨찾기 추가/조회/삭제<br/>
      • 추천 고도화 (자주 사용하지 않은 유사 매장 제안 등)<br/>
      • 내 정보 수정 및 멤버십 등급 표시
    </td>
  </tr>
  <tr>
    <th>📋 제휴처 목록</th>
    <td>
      • 전체 제휴 브랜드 검색 및 카테고리/브랜드별 필터링<br/>
      • 각 브랜드 클릭 시 상세 혜택 및 사용 방법 확인
    </td>
  </tr>
  <tr>
    <th>🔐 인증 / 인가</th>
    <td>
      • 카카오 소셜 로그인 및 JWT 기반 인증<br/>
      • 회원가입 시 설문조사 진행 (선호 브랜드, 카테고리)<br/>
      • 사용자 / 관리자 권한 분리 및 멤버십 등급 시스템
    </td>
  </tr>
  <tr>
    <th>🎯 추천 알고리즘</th>
    <td>
      • 검색/방문/즐겨찾기 등 행동 기반 개인화 추천<br/>
      • 동일 카테고리 내 미방문 매장 추천 ("여긴 어때요?")<br/>
      • 위치 + 멤버십 등급 조합을 통한 큐레이션 추천
    </td>
  </tr>
  <tr>
    <th>🛠️ 관리자 기능</th>
    <td>
      • 제휴 브랜드 및 매장 정보 추가/수정/삭제<br/>
      • 전체 사용자 행동 기반 통계 (DAU/MAU, 카테고리 인기도 등)<br/>
      • 매장별 즐겨찾기 현황, 브랜드별 성과 분석<br/>
      • 관리자 전용 관심 카테고리/브랜드/혜택 분석 리포트 제공
    </td>
  </tr>
</table>

## 3. 기술 스택 및 아키텍처
### 3.1 주요 기술 스택
<details>
  <summary><strong>⚙️ Backend</strong></summary>
  
  ### 주요 프레임워크
  <img src="https://img.shields.io/badge/Java_17-007396?style=for-the-badge&logo=openjdk&logoColor=white"/>
  <img src="https://img.shields.io/badge/SpringBoot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white"/>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/>
  
  ### 보안 & 인증
  <img src="https://img.shields.io/badge/Spring_Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white"/>
  <img src="https://img.shields.io/badge/OAuth2-EC407A?style=for-the-badge&logo=openid&logoColor=white"/>
  <img src="https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white"/>
  
  ### ORM & 문서화
  <img src="https://img.shields.io/badge/Spring_Data_JPA-6DB33F?style=for-the-badge&logo=spring&logoColor=white"/>
  <img src="https://img.shields.io/badge/QueryDSL-4479A1?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black"/>
  
  ### 테스트 & 버전관리
  <img src="https://img.shields.io/badge/JUnit_5-25A162?style=for-the-badge&logo=junit5&logoColor=white"/>
  <img src="https://img.shields.io/badge/Mockito-78A641?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Liquibase-2962FF?style=for-the-badge&logo=liquibase&logoColor=white"/>
  <img src="https://img.shields.io/badge/LightFM-FF6F00?style=for-the-badge&logo=python&logoColor=white"/>
</details>
<details>
  <summary><strong>🖥️ Frontend</strong></summary>
  
  ### 프레임워크 & 스타일
  <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=white"/>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white"/>
  <img src="https://img.shields.io/badge/TailwindCSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white"/>
  <img src="https://img.shields.io/badge/shadcn/ui-111827?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Radix_UI-161618?style=for-the-badge"/>
  
  ### 상태관리 & 통신
  <img src="https://img.shields.io/badge/Zustand-000000?style=for-the-badge&logo=zotero&logoColor=white"/>
  <img src="https://img.shields.io/badge/TanStack_Query-FF4154?style=for-the-badge&logo=react-query&logoColor=white"/>
  <img src="https://img.shields.io/badge/Axios-5A29E4?style=for-the-badge&logo=axios&logoColor=white"/>
  
  ### 개발 도구
  <img src="https://img.shields.io/badge/Storybook-FF4785?style=for-the-badge&logo=storybook&logoColor=white"/>
  <img src="https://img.shields.io/badge/Recharts-8884D8?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Framer_Motion-0055FF?style=for-the-badge&logo=framer&logoColor=white"/>
  <img src="https://img.shields.io/badge/ESLint-4B32C3?style=for-the-badge&logo=eslint&logoColor=white"/>
  <img src="https://img.shields.io/badge/Prettier-F7B93E?style=for-the-badge&logo=prettier&logoColor=black"/>
</details>
  
<details>
  <summary><strong>🗄️ Database</strong></summary>

  ### RDB & 공간정보
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/PostGIS-008000?style=for-the-badge&logo=postgresql&logoColor=white"/>

</details>

<details>
  <summary><strong>☁️ Infra & Architecture</strong></summary>

  ### 클라우드
  <img src="https://img.shields.io/badge/AWS_EC2-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white"/>
  <img src="https://img.shields.io/badge/AWS_RDS-527FFF?style=for-the-badge&logo=amazonrds&logoColor=white"/>
  <img src="https://img.shields.io/badge/S3-569A31?style=for-the-badge&logo=amazonaws&logoColor=white"/>

  ### 배포 & 자동화
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white"/>

</details>

  ### 3.2 ERD
  ### 3.3 시스템 구성도
### 3.4 프로젝트 폴더 구조
폴더구조..

## 4. 프로젝트 결과물
  ### 4.1 서비스 화면 및 기능 시연
  ### 4.2 성능 최적화 / 테스트 전략
  ### 4.3 사용자 피드백
  ### 4.4 트러블 슈팅(문제발생, 해결방안, 결과)

## 5. 개발 일정 및 마일스톤

## 6. 회고 및 향후 개선 방향

## 7. 팀원 소개 및 역할 분담
  이름, 역할, 맡은 기능
  
## 8. 프로젝트 산출물
  발표자료, 시연 영상, 기획안, 노션, 피그마?

## 9. 협업 환경 & 툴

## 10. 협업 컨벤션 / 절차
  ### 10.1 JIRA 사용 흐름
  ### 10.2 GIT 컨벤션
  ### 10.3 기타 규칙(코드리뷰, PR 템플릿 등)
