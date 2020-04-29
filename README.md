# MovieFlex
영화예매(만) 하는 사이트입니다. 종류는 영화예매, 영화목록이 있습니다.

# 프로젝트 기간
> v.0.0.3 (2020.04.29)
- 2020-02-28 ~ 2020-05-02 (약 2개월)
- 이후 상시 업데이트중...

# 사용 기술
- spring(security, AOP, tx)
- HTML5, CSS3, JAVSCRIPT
- JQUERY, AJAX
- JSON

# 사용한 핵심 기능
- properties 암호화
- 이메일 인증 (google)
- 영화 openapi 이용
- jsoup 이용하여 영화정보를 추출하여 DB저장
- spring security 인가/인증/권한 커스텀마이징
- spring transaction 이용
- 영화 하루 스케쥴 알고리즘 제작
- 영화 좌석 알고리즘 제작
- 하루마다 (하루 스케쥴 알고리즘) 자동 시작하기 위해 Job Scheduled 이용
- 쿠키를 이용하여 인증번호 부여 및 아이디 저장
- error 페이지 제작
- 영화 예매 restful기술 이용 및 AJAX 기술 사용
- hikaricp를 이용하여 사용자에게 더욱 빠른 서비스를 제공

# 프로젝트 안내
1. 이 프로젝트는 개인 프로젝트입니다.
2. css (영화 C사)를 벤치마킹 하였으며 다른것들은 모두 직접 제작함.
3. 실력향상을 위해 라이브러리를 이용하지 않음 ex(페이징, 슬라이드 등등...)

# 프로젝트 메뉴 소개
1. 영화
- 상영중인 영화 목록, 상영 종료 영화 목록
2. 예매
- 상영중인 영화 예매목록
- 선택한 영화의 좌석목록
3. 조회(검색)
- 네이버 api를 이용하여 모든 영화 검색 (이미지 클릭시 네이버 영화로 이동)

# 프로젝트 상세도
```
  MOVIEFLEX
  │
  ├─src/main/java
  │  │
  │  ├─com.reserved.Auth
  │  │  │
  │  │  ├CustomAccessDeniedHandler
  │  │  ├CustomAuthenticationEntryPoint
  │  │  ├CustomAuthenticationFailHandler
  │  │  ├CustomAuthenticationProvider
  │  │  └CustomAuthenticationSuccessHandler
  │  ├─com.reserved.Controller
  │  │  │
  │  │  ├ AuthEmailController
  │  │  ├ ErrorController
  │  │  ├ LoginController
  │  │  ├ MainController
  │  │  ├ MoviesController
  │  │  ├ ReservedAjaxController
  │  │  ├ ReservedController
  │  │  └ UserController
  │  ├─com.reserved.DAO
  │  │  │
  │  │  ├ MovieDAO
  │  │  ├ MovieDAOImpl
  │  │  ├ ReservedDAO
  │  │  ├ ReservedDAOImpl
  │  │  ├ TheaterDAO
  │  │  ├ TheaterDAOImpl
  │  │  ├ UserAuthDAO
  │  │  ├ UserDAO
  │  │  └ UserDAOImpl
  │  ├─com.reserved.DTO
  │  │  │
  │  │  ├ ApiInfo
  │  │  ├ Criteria
  │  │  ├ EntryptInfo
  │  │  ├ MemberInfo
  │  │  ├ MovieInfo
  │  │  ├ PagingInfo
  │  │  ├ TheaterInfo
  │  │  └ TicketInfo
  │  ├─com.reserved.interceptor
  │  │  │
  │  │  └ CustomInterceptor
  │  ├─com.reserved.service
  │  │  │
  │  │  ├ CustomUserDetailService
  │  │  ├ EmailService
  │  │  ├ MainService
  │  │  ├ MoviesService
  │  │  ├ ReservedService
  │  │  └ UserService
  │  └─com.reserved.utils
  │     │
  │     ├ EncryptAES
  │     └ MessageUtils
  └─src/main/Resource
     │
     ├ config
     │  │
     │  ├ encrypt-secret.properties
     │  ├ encrypt.xml
     │  ├ openapi.secret.propeties
     │  └ openapi.xml
     └─ mybatis
        │
        ├ MovieDAO.xml
        ├ ReservedDAO.xml
        ├ TheaterDAO.xml
        ├ TicketDAO.xml
        └ UserDAO.xml
```

# DB 모델링 자료
![DATAMODEL](/DATAMODEL/MOVIEFLEX_MODEL.png)
# 페이지 실행 화면
> 메인

> 회원가입

> 로그인

> 아이디 찾기

> 비밀번호 찾기

> 영화목록

> 영화정보

> 예매(step1)

> 예매(step2)


