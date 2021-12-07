# study-fast-api


## 2021.12.02
바운드와 블로킹(=바운드에 의해 코드실행이 멈추게 되는 현상)
* CPU 바운드
* I/O 바운드
* 사용자 I/O
* 네트워크 I/O


## 2021.12.03
* 동기/비동기
* 코루틴, 서브루틴: 코루틴은 서브루틴의 일반화 형태이다. 
* 서브루틴: 하나의 진입점, 하나의 탈출점이 있는 루틴(함수) --> 우리가 알고있는 일반적 함수 
* 코루틴: 다양한 진입점, 다양한 탈출점이 있는 루틴(함수)

병렬성과 동시성은 구분해야한다.

* 멀티 스레딩/ 멀티 프로세싱


## 2021.12.05

* 프로그램: 저장장치에 저장된 정적인 상태(HDD, SSD에 저장 및 보조 메모리)
* 프로세스: 실행을 위해 주메모리에 프로그램(일련의 코드)이 올라온 동적인 상태

프로세스가 생성되면 CPU는 프로세스가 해야할 작업을 수행한다.
이때 CPU가 처리하는 작업의 단위가 스레드이다.

* 사용자 수준 스레드
* 커널 수준 스레드


## 2021.12.06

병렬성을 포기하고 한번에 1개의 스레드만 유지하는 락인 GIL --> 멀티스레딩시 메모리 자원을 공유하는데서 오는 위험성을 차단

멀티스레딩은 동시성을 사용하여 IO bound 에서는 이점을 가질 수 있지만
CPU bound에서는 GIL에 의해 원하는 결과를 얻을 수 없다.
