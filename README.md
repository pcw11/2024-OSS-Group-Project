# 오픈소스소프트웨어 팀 과제
## 팀 - 오소소
### 구성원
|<a href="https://github.com/kbs-kbs/2024-OSS-Group-Project/graphs/contributors"><img src="https://contrib.rocks/image?repo=kbs-kbs/kbs-kbs"/></a>||||| 
|:---:|:---:|:---:|:---:|:---:|
|[@kbs-kbs](https://github.com/kbs-kbs)|||||
## 프로젝트 소개
### 제목
- 오픈소스소프트웨어 개발을 위한 효과적인 원격 저장소 구축 방법
### 설명
- 이 프로젝트는 오픈소스소프트웨어 개발을 위한 효과적인 원격 저장소 구축 방법을 제시합니다.
### 프로젝트 기간
- 2024-11-11 ~ 2024-12-06

## 목차
- [배경](#배경)
- [목적](#목적)
- [사례](#사례)
- [결론](#결론)


### 리포지토리 구조

```bash
├── README.md
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



## 설치

프로젝트를 로컬 환경에 설치하려면 깃을 실행한 뒤 다음 명령어를 입력합니다:

```bash
git clone https://github.com/kbs-kbs/2024-OSS-Group-Project.git
```

## 기여 방법

프로젝트에 기여하려면 GitHub wiki의 [기여 가이드라인](https://github.com/kbs-kbs/2024-OSS-Group-Project/wiki/How-To-Contribute)을 참고해 주시기 바랍니다.

## 라이선스
- MIT License
