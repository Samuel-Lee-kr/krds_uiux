# 디지털 정부서비스 UI/UX 가이드라인 추출

<img src="https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white"/>
<img src="https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white"/>
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black"/>
<img src="https://img.shields.io/badge/jQuery-0769AD?style=flat-square&logo=jQuery&logoColor=white"/>

## 프로젝트 설명

### 프로젝트 생성 이유
※ KRDS 운영팀의 답변 내용도 포함
- UI/UX 가이드라인에 대한 샘플 프로젝트는 제공하지 않음
  - 만들어진 퀄리티에 비해 제공 자료가 한정적이여서 활용도가 낮다고 보여짐
- 대국민 대상으로 제작된 가이드므로 오픈소스로 제공 및 별도 라이선스 정책 없음
  - 단 민간 웹사이트일 경우 **정부공식누리집 배너** 는 사용할 수 없음
  - 해당 프로젝트도 별도 라이선스 정책을 취하지 않음
- HTML, CSS, JS 코드 추출사용 허용
  - components 폴더
    - 디지털 정부서비스 UI/UX 가이드라인의 소스코드를 참고
  - samples 폴더
    - 디지털 정부서비스 UI/UX 임시 웹사이트의 소스코드를 추출 
  - CSS 경로 및 root 변수 참조 문제, JS 버그(UI 관련 버그) 등을 해결하여 업로드

### 추후 목표
- 표준프레임워크 오픈커뮤니티 내 프로젝트에 해당 UI/UX 를 적용하고자 함
  - 기여하고자 하는 프로젝트
    - React Project: [egovframe-template-simple-react](https://github.com/eGovFramework/egovframe-template-simple-react)
    - Spring Project: [egovframe-portal-site-template](https://github.com/eGovFramework/egovframe-portal-site-template) 

### 참조
- [디지털 정부서비스 UI/UX 가이드라인](https://uiux.egovframe.go.kr/guide/index.html)
- [디지털 정부서비스 UI/UX 임시 웹사이트](https://uiux.egovframe.go.kr/pattern/worksheet.html)

## 프로젝트 구성(폴더만)
```bash
ROOT
│ 
├─samples           // 임시 웹사이트 샘플 html
│ 
├─components        // 각 UI 요소 별 html
│ 
└─resources         // JS, CSS, IMAGES 등 리소스 영역
   │ 
   ├─js
   │  │ 
   │  ├─component
   │  │
   │  └─pattern
   │
   └─css            // CSS 폴더 내 fonts, images를 포함
      │
      ├─output
      │
      ├─fonts
      │
      └─images
         │  
         ├─guide
         │  
         ├─component
         │  │
         │  └─common
         │
         └─pattern
             ├─common
             ├─content
             ├─layout
             └─sample
```

## 프로젝트 구성(파일 포함)

<details>
<summary>접기/펼치기</summary>

```bash
ROOT
│
│  .gitignore
│  README.md
│
├─components
│      00. 탬플릿.html
│      01. 공식배너.html
│      02. 운영기관 식별자(기본형태).html
│      02. 운영기관 식별자(적용예시).html
│      03. 푸터.html
│      04. 헤더(타입1).html
│      04. 헤더(타입2).html
│      05. 건너뛰기 링크.html
│      06. 메인 메뉴(타입1).html
│      06. 메인 메뉴(타입2).html
│      07. 브레드크럼.html
│      08. 사이드 메뉴.html
│      09. 콘텐츠 내 탐색(일반형).html
│      10. 페이지네이션.html
│      11. 구조화 목록.html
│      12. 긴급공지.html
│      12. 긴급공지.html~
│      13. 달력.html
│      14. 디스클로저.html
│      15. 모달(alert형).html
│      15. 모달(class_data-target 호출형).html
│      15. 모달(기본형).html
│      16. 배지.html
│      17. 아코디언.html
│      18. 캐러셀(요소배너).html
│      18. 캐러셀(풀배너).html
│      19. 탭.html
│      20. 표.html
│      21. 링크.html
│      22. 버튼(계층).html
│      22. 버튼(기본).html
│      22. 버튼(사이즈).html
│      22. 버튼(아이콘버튼).html
│      22. 버튼(텍스트).html
│      23. 라디오버튼(기본).html
│      23. 라디오버튼(박스).html
│      23. 라디오버튼(사이즈별).html
│      23. 라디오버튼(칩).html
│      23. 라디오버튼(칩-사이즈별).html
│      24. 체크박스(기본).html
│      24. 체크박스(박스).html
│      24. 체크박스(사이즈별).html
│      24. 체크박스(스위치).html
│      24. 체크박스(스위치-사이즈별).html
│      24. 체크박스(칩).html
│      24. 체크박스(칩-사이즈별).html
│      25. 셀렉트(기본).html
│      25. 셀렉트(사이즈별).html
│      26. 태그.html
│      27. 단계 표시기(일반).html
│      27. 단계 표시기(제목혼합).html
│      28. 스피너.html
│      29. 도움 패널(타입1).html
│      29. 도움 패널(타입2).html
│
├─resources
│  ├─css
│  │  │  pattern_css.css
│  │  │  swiper-bundle.min.css
│  │  │
│  │  ├─fonts
│  │  │      PretendardGOV-Bold.subset.woff
│  │  │      PretendardGOV-Medium.subset.woff
│  │  │      PretendardGOV-Regular.subset.woff
│  │  │
│  │  ├─images
│  │  │  ├─component
│  │  │  │  └─common
│  │  │  │          ico-prev_24.svg
│  │  │  │          ico_arr1_20_right.svg
│  │  │  │          ico_arr_16_down.svg
│  │  │  │          ico_arr_16_right_gray70.svg
│  │  │  │          ico_arr_20_down_blue.svg
│  │  │  │          ico_arr_20_down_white.svg
│  │  │  │          ico_arr_20_right.svg
│  │  │  │          ico_arr_20_right_disabled.svg
│  │  │  │          ico_arr_accordion.svg
│  │  │  │          ico_arr_func_20.svg
│  │  │  │          ico_bread_dot.svg
│  │  │  │          ico_calendar.svg
│  │  │  │          ico_call.svg
│  │  │  │          ico_cal_dropdown.svg
│  │  │  │          ico_cal_move.svg
│  │  │  │          ico_check_8.svg
│  │  │  │          ico_check_chip.svg
│  │  │  │          ico_check_chip_checked.svg
│  │  │  │          ico_check_chip_disabled.svg
│  │  │  │          ico_check_primary_checked.svg
│  │  │  │          ico_check_primary_disabled.svg
│  │  │  │          ico_check_secondary.svg
│  │  │  │          ico_check_secondary_checked.svg
│  │  │  │          ico_check_secondary_disabled.svg
│  │  │  │          ico_chip_del.svg
│  │  │  │          ico_close_24.svg
│  │  │  │          ico_close_modal.svg
│  │  │  │          ico_comment_16.svg
│  │  │  │          ico_del1_20.svg
│  │  │  │          ico_del_20.svg
│  │  │  │          ico_email_20.svg
│  │  │  │          ico_faq.svg
│  │  │  │          ico_file_20.svg
│  │  │  │          ico_filter_20.svg
│  │  │  │          ico_foldable.svg
│  │  │  │          ico_go_20.svg
│  │  │  │          ico_help_24.svg
│  │  │  │          ico_hint_20.svg
│  │  │  │          ico_hint_error.svg
│  │  │  │          ico_info.svg
│  │  │  │          ico_invalid_error_20.svg
│  │  │  │          ico_invalid_ok_20.svg
│  │  │  │          ico_like_20.svg
│  │  │  │          ico_link_16.svg
│  │  │  │          ico_login_20.svg
│  │  │  │          ico_logout_16.svg
│  │  │  │          ico_page_arr_left.svg
│  │  │  │          ico_page_arr_right.svg
│  │  │  │          ico_page_dot.svg
│  │  │  │          ico_plus_24.svg
│  │  │  │          ico_print_20.svg
│  │  │  │          ico_pw_visible.svg
│  │  │  │          ico_refresh_16.svg
│  │  │  │          ico_sch1_20.svg
│  │  │  │          ico_sch_20_wh.svg
│  │  │  │          ico_sch_40.svg
│  │  │  │          ico_scrap_20.svg
│  │  │  │          ico_select_20.svg
│  │  │  │          ico_select_lg.svg
│  │  │  │          ico_setting_20.svg
│  │  │  │          ico_share_20.svg
│  │  │  │          ico_step_active.svg
│  │  │  │          ico_swiper_more.svg
│  │  │  │          ico_swiper_next.svg
│  │  │  │          ico_swiper_next_gray.svg
│  │  │  │          ico_swiper_next_wh.svg
│  │  │  │          ico_swiper_play.svg
│  │  │  │          ico_swiper_prev.svg
│  │  │  │          ico_swiper_prev_gray.svg
│  │  │  │          ico_swiper_prev_wh.svg
│  │  │  │          ico_swiper_stop.svg
│  │  │  │          ico_tooltip_20.svg
│  │  │  │          ico_tool_arr.svg
│  │  │  │          ico_upload_20_wh.svg
│  │  │  │          ico_urgent_badge_danger.svg
│  │  │  │          ico_urgent_badge_info.svg
│  │  │  │          ico_urgent_badge_ok.svg
│  │  │  │
│  │  │  ├─guide
│  │  │  │      favicon_180.png
│  │  │  │      favicon_192.png
│  │  │  │      favicon_32.png
│  │  │  │      favicon_512.png
│  │  │  │
│  │  │  └─pattern
│  │  │      ├─common
│  │  │      │      ico_bread_arr.svg
│  │  │      │      ico_bread_home.svg
│  │  │      │      ico_close_48.svg
│  │  │      │      ico_drop_arr.svg
│  │  │      │      ico_h_tit_drop_arr.svg
│  │  │      │      ico_info.svg
│  │  │      │      ico_sch1_20.svg
│  │  │      │      ico_time_16.svg
│  │  │      │
│  │  │      ├─content
│  │  │      │      balloon-bottom.png
│  │  │      │      btm_ban_ico_flag.svg
│  │  │      │      ico_arr_expand.svg
│  │  │      │      ico_check_rd_20.svg
│  │  │      │      ico_conts_expand.svg
│  │  │      │      ico_helper_info.svg
│  │  │      │      ico_helper_info_trans.svg
│  │  │      │      ico_login_certify_go.svg
│  │  │      │      ico_login_certify_type_01.svg
│  │  │      │      ico_login_certify_type_02.svg
│  │  │      │      ico_login_certify_type_03.svg
│  │  │      │      ico_login_certify_type_04.svg
│  │  │      │      ico_login_certify_type_05.svg
│  │  │      │      ico_login_certify_type_06.svg
│  │  │      │      ico_outline.svg
│  │  │      │      ico_outline_chk.svg
│  │  │      │      ico_smile_20.svg
│  │  │      │      main_ico_bag_S.svg
│  │  │      │      main_ico_bankbook_L.svg
│  │  │      │      main_ico_bankbook_S.svg
│  │  │      │      main_ico_battery_M.svg
│  │  │      │      main_ico_book_M.svg
│  │  │      │      main_ico_building_L.svg
│  │  │      │      main_ico_building_M.svg
│  │  │      │      main_ico_bulb_S.svg
│  │  │      │      main_ico_card_S.svg
│  │  │      │      main_ico_energy_S.svg
│  │  │      │      main_ico_store_S.svg
│  │  │      │      main_ico_truck_S.svg
│  │  │      │      main_menu_blue_ico1.svg
│  │  │      │      main_menu_blue_ico2.svg
│  │  │      │      main_menu_blue_ico3.svg
│  │  │      │      main_menu_blue_ico4.svg
│  │  │      │      main_menu_ico1.svg
│  │  │      │      main_menu_ico2.svg
│  │  │      │      main_menu_ico3.svg
│  │  │      │      main_menu_ico4.svg
│  │  │      │      main_menu_ico5.svg
│  │  │      │      main_menu_ico6.svg
│  │  │      │      main_menu_ico7.svg
│  │  │      │      main_menu_ico8.svg
│  │  │      │      top_ban_ico_flag.svg
│  │  │      │
│  │  │      ├─layout
│  │  │      │      foot_ico_plus.svg
│  │  │      │      foot_ico_sns_blog.svg
│  │  │      │      foot_ico_sns_facebook.svg
│  │  │      │      foot_ico_sns_Instagram.svg
│  │  │      │      foot_ico_sns_twitter.svg
│  │  │      │      foot_ico_sns_youtube.svg
│  │  │      │      head_gnb_ico_arr.svg
│  │  │      │      head_gnb_ico_arr_on.svg
│  │  │      │      head_ico_navi_all.svg
│  │  │      │      head_ico_navi_join.svg
│  │  │      │      head_ico_navi_login.svg
│  │  │      │      head_ico_navi_my.svg
│  │  │      │      head_ico_navi_sch.svg
│  │  │      │      head_ico_nuri.svg
│  │  │      │      head_logo.svg
│  │  │      │      head_logo_slogan.svg
│  │  │      │      lnb_ico_prev.svg
│  │  │      │
│  │  │      └─sample
│  │  │              sample_img_total_thum1.jpg
│  │  │              sample_img_total_thum2.jpg
│  │  │              sample_img_total_thum3.jpg
│  │  │              sample_main_news_thum1.jpg
│  │  │              sample_main_news_thum2.jpg
│  │  │              sample_main_person_thum1.jpg
│  │  │              sample_main_person_thum2.jpg
│  │  │
│  │  └─output
│  │          c_components.css
│  │          c_forms.css
│  │          c_initialize.css
│  │          c_kds.css
│  │          p_common.css
│  │          p_content.css
│  │          p_layout.css
│  │
│  └─js
│      ├─component
│      │      ui-script.js
│      │
│      └─pattern
│              jquery.min.js
│              swiper-bundle.min.js
│              ui-pattern-script.js
│
└─samples
        00. 화면목록.html
        01. 레이아웃(레이아웃1).html
        02. 레이아웃(레이아웃2).html
        03. 탐색(검색어버튼,필터 즉각적용1).html
        04. 탐색(검색어버튼,필터 즉각적용2).html
        05. 탐색(검색어버튼,필터 즉각적용3).html
        06. 탐색(검색어+필터).html
        07. 로그인(로그인 방식 선택).html
        08. 로그인(로그인 선택(싱글타입)).html
        09. 로그인(로그인 입력).html
        10. 로그인(로그인 입력(탭타입)).html
        11. 로그인(약관동의).html
        12. 통합검색(검색결과).html
        13. 통합검색(검색필터(선택 전)).html
        14. 통합검색(검색필터(선택 후)).html
        15. 서비스 신청(신청목록-카드형).html
        16. 서비스 신청(신청목록-카드 선택형).html
        17. 서비스 신청(신청목록-리스트형).html
        18. 서비스 신청(신청목록-리스트 선택형).html
        19. 서비스 신청(신청상세-일반형).html
        20. 서비스 신청(신청상세-탭형).html
        21. 서비스 신청(신청안내 step1).html
        22. 서비스 신청(신청안내 step2-조회 전).html
        23. 서비스 신청(신청안내 step2-조회 후).html
        24. 서비스 신청(신청안내 step2-복잡도에 따른 유형).html
        25. 서비스 신청(신청안내(주민등록등본발급)).html
        26. 서비스 신청(신청안내(건물대장등본발급)-도움패널 타입1).html
        27. 서비스 신청(신청안내(건물대장등본발급)-도움패널 타입2).html
        28. 서비스 신청(신청안내(자료신청)).html
        29. 서비스 신청(신청안내(신청완료)).html
        31. 방문(방문유형1-1).html
        32. 방문(방문유형1-2).html
        33. 방문(방문유형2-1).html
        34. 방문(방문유형2-2).html
        35. 방문(방문유형3-1).html
        36. 방문(방문유형3-2).html
        37. 긴급공지.html
        38. 정책정보(정책목록).html
        39. 평가.html
        40. 코치마크(단계적 실습패널-선택 단계).html
        41. 코치마크(단계적 실습패널-1단계).html
        42. 코치마크(단계적 실습패널-2단계).html
        43. 코치마크(단계적 실습패널-3단계).html
        44. 코치마크(단계적 실습패널-4단계).html
        45. 전입신고(기관 적용안-1).html
        46. 전입신고(기관 적용안-2).html
        47. 전입신고(기관 적용안-3).html
        48. 전입신고(기관 적용안-4).html
        49. 전입신고(기관 적용안-5).html
        50. 전입신고(기관 적용안-6).html
        51. 전입신고(기관 적용안-7).html
```
</details>
