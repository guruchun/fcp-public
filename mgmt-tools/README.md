## 관리자 도구 

시스템 모니터링 및 제어용으로 엔지니어가 사용하기 위해 만들어진 도구이다. 일반 사용자 및 고객에게는 공개되지 않는다.



### 범용 도구

범용으로 사용할 수 있는 도구이다.

#### Modbus Tool

* Modbus RTU/TCP 통신을 제공한다.
  * Function Code는 Simple List만 제공한다. (단일 읽기/쓰기, 영역 읽기/쓰기)
* Client/Server 모드로 동작할 수 있다.
* Coil, Disc, Holding, Input 레지스터는 별도의 메모리 공간으로 분리되어 있다.

#### CAN Manager

* DBC 파일로부터 CAN 버스의 Node 목록, 메시지 목록, Signal 목록을 읽는다.
* DBC에 정의된 메시지 규격과 Signal 규격을 사용해서 CAN 메시지와 메시지의 Data Field를 구성한다.
* PC에 연결된 CAN 컨버터를 사용해 메시지를 송신한다.
* PC에 연결된 CAN 컨버터를 사용해 메시지를 수신한다.
* 수신된 메시지를 DBC에 정의된 메시지 규격에 따라  파싱해 Signal의 값을 읽는다.
* Signal의 값을 Tag에 매핑해 Data View에 보여준다.
* Data View의 Tag 값을 소스로 사용해서 CAN Signal의 값을 업데이트할 수 있다.



### 시스템 도구

시스템용으로만 사용할 수 있는 도구이다.

* Main-Controller Client on Modbus/TCP
* Sub-Controller Client on CAN
* Device Simulator
   - Inverter Simulator
   - TC Module Simulator
   - HSS Simulator
   - Sub-Controller Simualtor
* 실시간 데이터 보기
* 로그 데이터 차트 분석



### 공통 기본 기능
* 송수신 메시지 로깅
* 송수신 데이터의 상태값 저장 및 데이터 조회화면 제공
* 데이터의 초기값 지정
* 데이터의 상태값을 파일로 저장



