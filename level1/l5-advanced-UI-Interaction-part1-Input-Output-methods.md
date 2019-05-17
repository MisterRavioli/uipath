# Advanced UI Interaction Par1 - Input/Output methods

* 데이터 스크래핑 - 테이블 및 구조적 데이터를 웹페이지와 애플리케이션 그리고 문서에서 추출하는 기술

## 범주

* Input actions
    + 사용자(봇)이 직접적인 액션을 수행하는 것
    + 자동화하는 애플리케이션이나 웹 페이지에 대해서도.
    + 클릭, 입력, 숏컷, 
* Output Actions
    + 앱에서 정보를 얻어 추가 처리를 위해 uipath에 제공하는 것.
    + 레코딩 할 수 없다. 모든 애플리케이션은 사람을 위해 만들어 지며 주요 출력 방법이 결과를 디스플레이에 표시하는 것.
    + 텍스트 가져 오기 등등
    
## Type Info의 3가지 방법
* Default - 기본적인 옵션
    + 느리다
    + 백그라운드에서 작동되지 않는다.
* Send Window Messages
    + 가장 느리다
    + 백그라운드에서 작동 된다.
* Simulate Type/Click
    + 빠르다
    + EmptyField를 선택하지 않아도 텍스트가 대체 된다.
    + 백그라운드에서 작동 된다.