# Lesson Orchestrator Presentation and Agenda

UIPath Orchestrator는 UiPath Robots의 자동화 작업을 배포, 모니터링 및 관리 할 수 있는 웹 기반 응용 프로그램.
Attended 및 UnAttended Robot 리소스를 통합하고 중앙 집중식 로봇 로그, 원격 실행, 모니터링, 스케쥴링 및 작업 대기열을 제공.

UIPath Orchestrator는 일종의 명령 센터로서 로봇과 자동화 프로젝트를 제어하며, 대규모로 배치된 로봇을 관리하는 기능과
여러 시스템과 검토자가 관련된 복잡한 프로세스를 관리하는 기능을 제공한다.

Studio에서 프로젝트를 퍼블리싱하면 프로젝트가 패키지로 Orchestrator에 전송 된다.
이를 위해 Studio의 SETUP 탭으로 이동해 Publish를 클릭 성공하면 메시지창이 나타나고 패키지 이름과 버전이 표시된다.

프로세스가 작동하려면 먼저 로봇 인스턴스를 Orchestrator에 연결 해야 한다.

여러 로봇을 동시에 작동하게 하기위해 그룹핑을 해야 한다. 
Orchestrator에서 ROBOTS의 Environment를 만들어야 한다.

그리고 사용가능한 모든 로봇이 해당 환경에서 패키지를 실행할 수 있게 패키지를 환경에 설정해야 한다.
Orchestrator에서 프로세스를 만들어 연결을 설정 할 수 있다.

이렇게 만들어진 프로세스는 3개의 로봇 모두에서 동시에 실행 가능하다.

이후 새로운 Job을 만들어야 진행할 수 있다. Start를 한후 새로 만든 프로세서를 선택한다. 실행될 로봇을 선택후 시작!


## Trigger

UiPath Orchestrator에서 작업을 트리거 하는 방법에는 두 가지가 있다.

* 수동으로 작업 시작
* 스케쥴링으로 시작
    * 이름을 적고 실행될 프로세스를 추가
    * 표준 시간대를 설정
    * Actions에서는 지정한 시간이 경과한 후에 작업을 중지 할 수 있다. 이떄 종료/취소 를 선택 할 수 있다.
    * Executing Target은 기본적으로 모든 로봇이 작업을 실행하도록 설정 돼 있다.
        +  특정 로봇을 선택하거나 원하는 만큼 로봇을 선택 할 수 있다.
        
* 동일한 로봇이 이미 자동화를 실행중이면 뒤에 실행될 자동화는 pending상태가 되고 앞의 자동화가 끝이나면 실행된다.
* 또한 should Stop 액티비티를 사용하여 Orchestrator의 Job에 Stop기능을 사용할수 있다.
    + Stop을 하면 should Stop이 True을 반환 한다.
    
    
## Log

SendLog를 통해 Orchestrator로 로그를 전송할 수 있다.

## Asset

* Asset을 사용하면 한 곳에서 변수 값을 관리할 수 있다.
* Asset은 전역 변수처럼 사용할 수 있다. 다양한 시스템과 환경 전체에서 동기화 할수 있는 변수 처럼.
* Aseet은 4가지 타입이 존재 함.
    + Text
    + Bool
    + Integer
    + Credential
* Orchestrator의 Asset에서 만들 수 있다.
* Get Asset으로 가져 와 변수에 할당 할 수 있다.

## Queue