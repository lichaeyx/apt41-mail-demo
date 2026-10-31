# APT41 TOUGHPROGRESS - Phishing Mail

## 1. 개요
APT41 TOUGHPROGRESS 기반 CHEIRON BAS 프로젝트의 초기 침투(Initial Access) 단계를 재현하기 위한 피싱 메일 형태의 웹페이지 제작

- **MITRE ATT&CK:** T1566.002 (Spearphishing Link)
- **사용 기술:** HTML, CSS
- **실행 환경:** Windows 브라우저

## 2. 구현 내용
- 발신자, 수신자, 제목, 본문으로 구성된 메일 화면 구현
- CSS를 이용한 이메일 형태의 UI 제작
- 임시 ZIP 파일 다운로드 버튼 구현
- 실제 이메일 발송 없이 로컬 HTML로 실행 가능

## 3. 파일 구성
```text
apt41-mail-demo/
├── README.md
├── apt-41-demo.zip
    └── index.html
    └── style.css
    └── files/
        └── sample.zip
```

## 4. 실행 방법
1. `index.html`을 브라우저로 실행
2. 피싱 메일 형태의 화면 확인
3. 다운로드 버튼 클릭 후 임시 ZIP 다운로드 확인

## 5. 향후 작업
- 팀원이 제작한 최종 테스트 ZIP 연결
- CHEIRON Procedure와 연동
- 공통 작업 경로 `%TEMP%\toughprogress_bas\` 적용
- ZIP 다운로드 및 SHA-256 검증 테스트

## 6. 참고
본 모듈은 보안 실습용으로 실제 메일 발송 및 악성코드 실행 기능은 포함하지 않음.
