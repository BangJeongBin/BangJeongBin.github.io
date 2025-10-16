---
layout: post
---

## 1. 프로젝트 소개 (Introduction)
---
 - **프로젝트 개요**
	- 학원에서 학생들을 관리할 수 있는 학적 관리 서비스를 개발, 강사는 수업을 게시하고 학생은 수강신청을 하여 직원의 컴펌하에 개강 후 정해진 커리큘럼대로 출석과 테스트 점수등을 입력 받고 수료를 받는 전 과정을 관리시스템에서 진행.

<br>

- **개발 기간, 투입 인원**
	- 2025.03.21 ~ 2025.04.17 / 3 주
	- 3 인

<br>

- **담당 역할 [본인]**
	- NEXT.js를 이용한 강사 페이지 UI 구성 및 개발
	- REST API를 이용한 마이크로 서비스 아키텍쳐 개발
	- 학사관리 시스템의 강사기능을 주요 개발하여 관련 기능 구현
	- Spring Security와 JWT를 이용해 토큰 기반 인증 및 권한 관리를 통해 보안 강화
	- 페이지네이션, 검색, 정렬, 한 페이지에서 다중 기능 구현 및 레이아웃을 구현하여 강사 Role의 친화적인 UX를 구현

<br>

## 2. 개발 환경 (Tech Stack)
---
- **Language**
	- `Java 17 (JDK 17.0.13)`
	- `JavaScript (ES6+)`

- **Framework & Library**

	- **Backend**
	    - `Spring Boot 2.7.18`    
	    - `Gradle`
	    - `Spring Security`
	    - `JPA (Java Persistence API)`
	    - `Tomcat 9.0.89`
	    - `JUnit`
	    - `MyBatis`
	    - `REST API`
        
	- **Frontend**
	    - `Next.js 15.2.4`
	    - `React 19.1.0`
	    - `Node.js v20.19.0`
	    - `Bootstrap`, `HTML5`, `CSS3`, `JavaScript`

- **Database**
	- `MariaDB 10.11`
	- `Amazon RDS`

- **Server & Deployment**
	- `Amazon EC2 (Ubuntu 22.04 LTS)`
	- `Apache Tomcat 9.0.89`
	- `GitHub Actions (CI/CD)`

- **Tools**
	- `IntelliJ IDEA 2024.3.3`
	- `Git`
	- `GitHub`
	- `Postman`

- **API & External Services**
	- `Google API`
	- `Kakao API`
	- `reCAPTCHA`

<br>

## 3. 주요 기능 (Features)
---
- 유저의 로그인 및 계정 관리에 다양한 JWT, Spring Security, Token 기반으로 보안을 중점적으로 개발
- Google API, Kakao API, reCAPTCHA 등 외부 API를 이용한 로그인 기능 구현
- MSA로 개발하여 서비스의 유연성과 독립성을 높히고 협업 함에 있어 이슈발생을 최소한으로 유지
- RESTful API 기반 설계 및 개발
- Spring Boot 기반의 백엔드 구조 설계 및 구현
- RSC를 이용해 Next.js스럽게 개발
- AWS EC2와 Github Action을 이용하여 배포 진행

<br>

- **관리자(교직원)**
	- 전반적인 운영(학생, 강사, 강의 학적, 공지 등)
	- UI를 이용하여 DB에 관련 값을 수정 및 입력, 삭제
	- 학생의 관리 및 강사 정보 관리, 전체적인 수업 진행 관리 등
	- 사전에 설정된 커리큘럼대로 진행되도록 수강 및 학적 개입 권한
	
- **강사**
	- 수업 계획, 수업 진행에 따른 성적, 과제 관리 등
	- 수강생 관리, 성적입력, 평가 등 본인 수업에 대한 모든 권한
	
- **학생**
	- 수강 신청 및 수업 진행에 따른 이벤트 처리
	- 출석, 평가, 설문조사 등 수료 가능 조건을 달성한 뒤 지정된 날찌에 수료

<br>

## 4. 시스템 아키텍처 (System Architecture)
---

![아키텍처 다이어그램](./assets/images/project_img/company-project/architecture_diagram.png)

- **아키텍처 다이어그램**

[ERD Diagram 링크](https://drive.google.com/file/d/1uPjuI-It98BK5cblLxbgAtwFObtsHJ5M/view?usp=sharing)

- **ERD**

<br>

## 5. 작성 문서 (Deliverables)
---

- [요구사항 명세서 링크](https://drive.google.com/file/d/1edgNto8dlFNehbWMFDiCsAvP0xYwrplO/view?usp=sharing)
	
- [UseCase Diagram 링크](https://drive.google.com/file/d/1_cOrtPCfBNhilgO3-mbrE83TDCeZvxHU/view?usp=sharing)
	
- [Process Modeling 링크](https://drive.google.com/file/d/1Pfa43bfY1Y_Zu1Qke1dTgKLZ_pRTdBNW/view?usp=sharing)
	
- [기능 정의서 링크](https://drive.google.com/file/d/1k9flrh6s6oK20oB2rqNn29xF2wm0XwEo/view?usp=sharing)

- [WBS 링크](https://drive.google.com/file/d/18t_rIrol3yg0CVLbj3kTic2tV-9dtfZV/view?usp=sharing)

<br>

## 6. 핵심 구현 (Core Implementation)
---

![로그인 페이지](./assets/images/project_img/company-project/login_page.png)

- **로그인 페이지**

<br>

![강사 대시보드](./assets/images/project_img/company-project/inst1.png)

- **강사 대시보드**

<br>

![과정정보 페이지](./assets/images/project_img/company-project/inst2.png)

- **과정정보 페이지**

<br>

![과제관리 페이지](./assets/images/project_img/company-project/inst3.png)

- **과제관리 페이지**

<br>

## 7. 트러블 슈팅 (Troubleshooting)
---
1. **reCAPTCHA 토큰이 다시 작성 버튼 클릭 시 제거되지 않음**
	- **문제 상황** : 사용자가 "다시 작성" 버튼 클릭 시 reCAPTCHA 토큰이 제거되지 않아, 새로 인증을 시도할 수 없음
	- **원인** : reCAPTCHA 토큰은 수동으로 제거되지 않으며 일정 시간이 지나야 자동 만료됨
	- **해결 과정** : `grecaptcha.reset()` 메서드를 사용하여 토큰을 수동으로 초기화, 버튼 클릭 시 명시적으로 토큰 초기화 코드 실행
	
2. **이메일 인증하기 버튼 클릭 시 404 에러**
	- **문제 상황** : 이메일 인증하기 버튼 클릭 시 `404 Not Found` 에러 발생
	- **원인** : 백엔드 API URL 오타 또는 라우팅 설정 누락
	- **해결 과정** : 이메일 인증 요청 URL을 정확히 확인하고 프론트에서 호출 경로 수정, 백엔드 컨트롤러의 엔드포인트 확인 및 CORS 허용 설정
	
3. **카카오/구글 로그인 시 DB 중복 등록**
	- **문제 상황** : SNS 로그인 사용자가 재로그인할 때마다 회원 정보가 DB에 중복 저장됨
	- **원인** : 로그인 시 기존 사용자 확인 로직 없이 매번 신규 회원으로 등록
	- **해결 과정** : SNS 로그인 시 이메일 또는 고유 ID 기준으로 기존 사용자 조회, 존재할 경우 새로 등록하지 않고 로그인 처리만 진행
	
4. **JWT 관련 Git 충돌**
	- **문제 상황** : JWT 인증 기능을 구현하는 과정에서 팀원 각자가 `JwtTokenProvider`, `JwtAuthenticationFilter`, `SecurityConfig` 등을 각각 작성하여 Git merge 시 충돌 발생
	- **원인** : 동일한 기능을 각자 다른방식으로 구현, 공통 클래스들을 따로 작성하여 git 충돌이 발생 
	- **해결 과정** : JWT 관련 코드를 공통 클래스로 통합하고, Bean 등록 방식을 통해 다중 `UserDetailsService`를 분리 주입하여 구조를 정리함
	
5. **`Refresh Token` 없이 `Access Token`만 초기화한 구조로 인한 보안 문제**
	- **문제 상황** : 갱신 버튼을 누르면 토큰을 재발급받기는 했지만, 이는 `Refresh Token`을 통한 재발급이 아니라 단순히 `Access Token`을 새로 발급하는 요청
	- **원인** : “Refresh Token"이라는 명칭만 사용했을 뿐, 실제로는 서버에 저장하거나 관리하지 않아 보안에 취약한 구조였음
	- **해결 과정** : 잘못 구현된 점을 인지하고, `Refresh Token`의 개념과 역할을 명확히 정리함. 이후 `Refresh Token`을 별도로 생성하고 서버에서 관리하는 구조로 개선할 필요성을 확인하여, 로직 수정이 필요한 상황임

<br>

## 8. 회고 (Outcomes & Learnings)
---
- **개선할 점**
	- ERD 작성 시 굉장히 수정이 많이 들어갔다. 도메인 지식이 많이 필요한 프로젝트 주제이기 때문에 초반에 시행착오가 많이 발생했다. 다음번엔 초반에 더 치밀하게 설계해야겠다
	
	- 프론트를 먼저 개발하고 그 이후에 백엔드와 연결하는 방식으로 개발은 진행했는데 이 과정에서 오류가 많이 발생했다. 프론트엔드 개발 시 백엔드를 염두에 두고 파라메터를 작성했어야 했는데 둘 사이에 싱크가 맞지 않아 중간중간 수정하느라 시간이 많이 걸렸다

<br>

- **느낀 점**
	- 팀원들과 협업 소통을 하는 과정에서 크고 작은 트러블 등을 해결해가며 의사소통 능력과 문제해결 능력이 상승한 것을 크게 느꼈다. 내 의견을 상대에서 의도대로 설명하는 것도 어렵지만 상대 입장에서 생각하며 조율해 나갈 수 있는 것이 개발자에게 필요한 역량인 것 같다.
	
	- 이번 프로젝트에서 계획, 개발, 배포까지 모든 과정을 직접 경험하며 많은 것을 배웠다. 굉장히 많은 새로운 기술들을 사용하였는데 이를 실제 프로젝트에 적용하는 과정에서 많은 시행착오를 겪었다. 많은 시간이 들었지만 돌아보니 그와 비례해서 실력이 크게 늘었고 그 순간들이 큰 보람으로 다가옴을 느꼈다.

<br>

## 9. 프로젝트 자료 (Links)
---
- [GitHub Repository](https://github.com/BangJeongBin/wizian_mentorship_project.git)
