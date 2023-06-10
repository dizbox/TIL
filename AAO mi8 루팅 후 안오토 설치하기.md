* mi 및 구글 계정 로그아웃
* 개발자모드 활성화
* usb 디버깅 활성화
* fastboot 모드로 부팅
    * power + volume down
* fastboot 확인
    * fastboot devices
    * fastboot oem device-info
* 초기화
    * fastboot format system
    * fastboot format userdata
* twrp로 3.3으로 부팅
    * fastboot flash recovery twrp-3.3.1-1-dipper.img
    * fastboot boot twrp-3.3.1-1-dipper.img
* twrp로 부팅
    * 기본 세팅 - 언어 + 시간
    * mount에서 enable MTP를 설정
        * 맥일 경우 android file transfer 설치해야함
    * 설치할 이미지 파일 복사
* install에서 설치
* miui 설정
    * 시스템앱 업데이트 (업데이트 하고 시스템 설정 마무리 해아함)
    * 구글 계정 로그인
    * 플레이 프로텍트 비활성화
    * 개발자 모드 및 usb 디버그 활성화
* trwp 3.7로 부팅 (파일암호화)
* magisk 23설치
    * zip파일로 이름 바꿔서 download 경로에 두기
    * 개인정보 보호 > 특수 앱 엑세스 > 알 수 없는 앱 설치에서 파일, magisk 등을 지정
    * 모듈
        - liboemcrypto disabler 설치
        - magiskhide props config 설치
* 스마트폰 화면용 안드로이드 오토 설치
    * 개발자 모드 설정
    * 어플리케이션 모드 개발자로
    * 알수없는 소스 체크
* screen2auto 2.4.6 설치



fastboot oem off-mode-charge 0


