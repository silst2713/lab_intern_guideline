# 자연대 랩인턴 백서 웹페이지

## 파일 구조
- index.html: 홈
- labs.html: 연구실 찾기
- interviews.html: 인터뷰 모아보기
- contact-mail.html: 컨택메일 가이드라인
- admin.html: 데이터 변환용 관리자 페이지
- site-data.js: 연구실/인터뷰 데이터 파일
- site-config.js: 외부 URL 설정
- sigape.css: 공통 스타일
- logo.png: 파람 로고

## 데이터 업데이트
연구실/인터뷰 페이지는 구글 스프레드시트에 연결하지 않고 site-data.js만 읽습니다.
site-data.js가 비어 있으면 "관리자 페이지에서 파일을 업로드해주세요." 안내가 표시됩니다.

1. admin.html에 접속합니다.
2. 비밀번호를 입력합니다.
3. 연구실 DB와 인터뷰 DB 파일을 업로드합니다.
4. site-data.js를 다운로드합니다.
5. GitHub 저장소의 기존 site-data.js를 다운로드한 파일로 교체합니다.
6. GitHub Pages 반영 후 기존 주소에서 새 데이터를 볼 수 있습니다.

CSV/TSV 파일은 외부 도구 없이 읽을 수 있습니다. XLSX 파일은 브라우저가 SheetJS 도구를 불러올 수 있어야 합니다.

## 외부 URL 설정
site-config.js에서 다음 값을 수정합니다.
- ERROR_FORM_URL: 오류 제보 구글폼 URL
- NOTION_URL: 자연대 학생회 노션 URL
