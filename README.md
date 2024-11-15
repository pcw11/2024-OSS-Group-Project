# 오픈소스소프트웨어 개발을 위한 원격 저장소 구축 방법 보고서
## 개요
## 팀 구성과 역할
## 프로젝트 기간
## 목차
- [배경](#배경)
- [목적](#목적)
- [사례](#사례)
- [결론](#결론)

## 소개

프로젝트에 대한 자세한 설명을 여기에 작성합니다. 프로젝트의 목적, 기능, 주요 특징 등을 포함할 수 있습니다.

### 팀 구성

|프로젝트 매니저|개발|개발|문서화|문서화|                                            
|:---:|:---:|:---:|:---:|:---:|
|<a href="https://github.com/kbs-kbs/2024-OSS-Group-Project/graphs/contributors"><img src="https://contrib.rocks/image?repo=kbs-kbs/kbs-kbs"/></a>|||||
|[@kbs-kbs](https://github.com/kbs-kbs)|||||


### 프로젝트 기간

2024.11.11 ~ 2024.12.06

### 주요 기능 📦

#### ⭐️강좌 선택 및 강의 영상 시청 기능
- Scratch, Python 2개 강좌 및 각 강좌마다 10개 가량의 강의 영상 제공
- 추후 지속적으로 강좌 추가 및 업로드 예정

#### ⭐️ 강의 관련 및 단체에 대한 자유로운 댓글 작성 가능
- Disqus를 이용하여 강의 관련 질문이나 단체에 대한 질문 작성 가능

#### ⭐️ 이어 학습하기 기능
- Cookie 기능을 이용하여 이전에 학습했던 내용 이후부터 바로 학습 가능


### 화면 구성 📺
| 메인 페이지  |  소개 페이지   |
| :-------------------------------------------: | :------------: |
|  <img width="329" src="https://user-images.githubusercontent.com/50205887/208036155-a57900f7-c68a-470d-923c-ff3c296ea635.png"/> |  <img width="329" src="https://user-images.githubusercontent.com/50205887/208036645-a76cf400-85bc-4fa2-af72-86d2abf61366.png"/>|  
| 강좌 소개 페이지   |  강의 영상 페이지   |  
| <img width="329" src="https://user-images.githubusercontent.com/50205887/208038737-2b32b7d2-25f4-4949-baf5-83b5c02915a3.png"/>   |  <img width="329" src="https://user-images.githubusercontent.com/50205887/208038965-43a6318a-7b05-44bb-97c8-b08b0495fba7.png"/>     |



## 설치

프로젝트를 설치하는 방법을 설명합니다. 예를 들어, 필요한 의존성 설치와 관련된 명령어를 포함할 수 있습니다.

```bash
# 예시 명령어
git clone https://github.com/사용자명/프로젝트명.git
cd 프로젝트명
npm install
```

## 사용법

프로젝트를 사용하는 방법을 설명합니다. 예제 코드나 스크린샷을 포함하여 사용법을 명확히 설명합니다.

```python
import example

example.run()
```

## 아키텍쳐

- 시스템 구성도: 프로젝트의 주요 구성 요소와 그들 간의 관계를 시각적으로 나타낸 다이어그램.
- 모듈 설명: 각 모듈이나 컴포넌트의 역할과 기능에 대한 설명.
- 데이터 흐름: 데이터가 시스템 내에서 어떻게 이동하고 처리되는지에 대한 설명.
- 기술 스택: 프로젝트에서 사용된 주요 기술과 도구.

### Stacks 🐈
#### Environment
![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-007ACC?style=for-the-badge&logo=Visual%20Studio%20Code&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=Git&logoColor=white)
![Github](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=GitHub&logoColor=white)             

#### Config
![npm](https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white)        

#### Development
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=Javascript&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Strapi](https://img.shields.io/badge/Strapi-2F2E8B?style=for-the-badge&logo=Strapi&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=Next.js&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=Bootstrap&logoColor=white)
![Material UI](https://img.shields.io/badge/Material%20UI-007FFF?style=for-the-badge&logo=MUI&logoColor=white)

#### Communication
![Slack](https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=Slack&logoColor=white)
![Notion](https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=Notion&logoColor=white)
![GoogleMeet](https://img.shields.io/badge/GoogleMeet-00897B?style=for-the-badge&logo=Google%20Meet&logoColor=white)


### 디렉토리 구조

```bash
├── README.md
├── package-lock.json
├── package.json
├── strapi-backend : 
│   ├── README.md
│   ├── api : db model, api 관련 정보 폴더
│   │   ├── about
│   │   ├── course
│   │   └── lecture
│   ├── config : 서버, 데이터베이스 관련 정보 폴더
│   │   ├── database.js
│   │   ├── env : 배포 환경(NODE_ENV = production) 일 때 설정 정보 폴더
│   │   ├── functions : 프로젝트에서 실행되는 함수 관련 정보 폴더
│   │   └── server.js
│   ├── extensions
│   │   └── users-permissions : 권한 정보
│   ├── favicon.ico
│   ├── package-lock.json
│   ├── package.json
│   └── public
│       ├── robots.txt
│       └── uploads : 강의 별 사진
└── voluntain-app : 프론트엔드
    ├── README.md
    ├── components
    │   ├── CourseCard.js
    │   ├── Footer.js
    │   ├── LectureCards.js
    │   ├── MainBanner.js : 메인 페이지에 있는 남색 배너 컴포넌트, 커뮤니티 이름과 슬로건을 포함.
    │   ├── MainCard.js
    │   ├── MainCookieCard.js
    │   ├── NavigationBar.js : 네비게이션 바 컴포넌트, _app.js에서 공통으로 전체 페이지에 포함됨.
    │   ├── RecentLecture.js
    │   └── useWindowSize.js
    ├── config
    │   └── next.config.js
    ├── lib
    │   ├── context.js
    │   └── ga
    ├── next.config.js
    ├── package-lock.json
    ├── package.json
    ├── pages
    │   ├── _app.js
    │   ├── _document.js
    │   ├── about.js
    │   ├── course
    │   ├── index.js
    │   ├── lecture
    │   ├── newcourse
    │   ├── question.js
    │   └── setting.js
    ├── public
    │   ├── favicon.ico
    │   └── logo_about.png
    └── styles
        └── Home.module.css

```

## 기여

프로젝트에 기여하는 방법을 설명합니다. 기여 가이드라인, 코드 스타일, 풀 리퀘스트(PR) 절차 등을 포함할 수 있습니다.

### 가이드라인

- [깃허브 위키](https://github.com/kbs-kbs/2024-OSS-Group-Project/wiki/How-To-Contribute)

## 라이선스

MIT License

## 연락처

- 이메일: example@example.com
- 깃허브 이슈: [GitHub Issues](https://github.com/kbs-kbs/2024-OSS-Group-Project/issues) 
