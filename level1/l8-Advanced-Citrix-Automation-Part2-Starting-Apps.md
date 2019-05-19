# Lesson 8 - Advanced Citrix Automation Part2- Advanced Citrix Automation: Starting Apps

## 애플리케이션 시작

* 바탕화면 아이콘 더블 클릭
    + Click Image를 사용하여 특정 아이콘에 대한 두번 클릭 액션을 수행 가능
    + 정확한 대상을 선택하지 않은 경우에는 문제가 발생한다.

* 애플리케이션에 윈도우 단축키를 적용 하는 것.
    + 복잡한 키 조합을 쓰는것이 안정적임. 기존의 숏컷과 충돌 가능성이 적어짐.
    * 해당 숏컷을 Send HotKey액션을 워크 플로우에 추가하여 키 조합을 할당.
    + 빠르고 안정적이기 때문에 이 방법을 먼저 쓰는것이 좋다.
    
* 매개변수나 인수를 사용하여 애플리케이션을 실행하는 경우.
    + Win+R 숏컷을 이용하여 실행
    + Win+R을 숏컷으로하는 Send Hotkey 액션을 등록
    + 이후 응용프로그램 경로를 TypeInfo로 적어 실행시킴.
    