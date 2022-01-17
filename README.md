# mvt-downloader
mvt downloader &amp; directory distributor 
사내에서 사용하기 위해 만들었으며, 다양한 방면으로 응용이 가능할 것으로 생각되어 백업해둔다...

개발사양: Java 11 + Maven + Mac OS(영향X)

#### mvt-downloader-static - [MVT파일 다운로드 모듈]
사전작업: 크롬 브라우저 설정에서 다운로드 폴더 지정 & '다운로드 전에 각 파일의 저장 위치 확인' 체크 해제
사용법: 화면 내 input box들에 z, x, y 입력 후 다운로드 시작 버튼 클릭. 자동으로 크롬 다운로드 지정 폴더로 파일이 저장된다.

#### mvt-distributor - [MVT파일 폴더 구조(Z/X/Y.mvt 구조) 생성 모듈]
config 폴더 내에 config.properties 파일 수정
path=크롬 다운로드 폴더 경로
extension=타겟 확장자
separator=파일명 내 Z,X,Y구분자

## 유의사항 + 메모
1. 크롬 브라우저 사용권장
2. 종종 CORS 오류가 떨어짐 (다만 정상적인 tile파일이 아닌 경우에 해당 에러가 발생하는 것으로 보인다. 자세한 원인은 파악X)
3. config.properties 안에 extension이나 separator를 조정하여 응용이 가능하나, 첨부된 원본 소스를 약간 수정해야할 수도 있다. (현재는 Z/X/Y 구조를 타겟으로 개발)
