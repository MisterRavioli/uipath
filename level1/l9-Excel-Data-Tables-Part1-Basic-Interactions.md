# Lesson 9 - Excel & Data Tables Part1 - Excel and Data Tables: Basic Interactions

## Excel Application Scope

이것은 컨테이너로서 다른 모든 Excel 액티비티를 이안에 포함 시켜야 한다.
* Visible 체크박스를 선택하여 UiPath가 마이크로소프트 엑셀을 사용해 파일을 읽고 선택 취소하면 익기 작업이 내부적으로 실행된다.
    + Visible On
        + Visible 옵션을 사용하려면 엑셀을 설치 해야 한다.
        + 모든 액션이 엑셀을 통해 수행 된다.
        + 작업상황을 실시간으로 확인할수 있다.
        + 디버깅에 유용하다.
    + Visible off
        + 엑셀을 설치할 필요가 없다.
        + 전체 프로세스가 백그라운드에서 실행됨.

* Read Range를 통해 엑셀데이터를 입력 받는다.
* Write Range를 통해 엑셀 데이터를 입력 한다.
* Append Range를 통해 데이터를 뒤에 넣는다.
* Build Data Table을 통해 기본적인 테이블을 간단하게 만들 수 있다.
* Sort Data Table을 통해 데이터를 정렬 할 수도 있다. Excel Application Scope 내/외부에서 사용 가능
* AddHeaders 옵션으로 머릿글을 넣고 빼고 할 수 있다.
* Read Cell 하나의 셀을 읽어온다
* Write Value 셀에 데이터를 입력한다
* Select Range 지정된 범위에 있는 개별 셀을 선택하는 액션
