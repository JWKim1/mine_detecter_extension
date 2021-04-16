# mine_detecter_extension
smartcar mine detector, using remote control, color


smart_mine_detector 확장.

Adoxx와 smartcar 이용.
  (Adoxx : University of Vienna의 OMiLAB 에서 개발한 Meta Modeling Platform, 
    Meta model을 기반으로 modeling 도구를 생성할 수 있는 도구)

주어진 지도를 smartcar로 주행하며 위험요소 탐지.

빨강, 노랑, 초록색을 탐지할 경우 각각 다른 위험 요소로 인식.

지뢰를 탐지한 위치를 저장하여 Adoxx프로그램으로 송신.

백지 지도를 가지고 있던 사용자는 탐색 후 위험요소를 아이콘으로 표시된 지도를 얻게 됨.




Smart car를 이용하여 지도의 경로 상에 있는 색상을 파악하여
지정된 색에 따라 어떤 위험요소인지 사용자에게 지도로 표시해 알려주는 프로그램이다.

주행 및 지뢰탐색을 위해 
Smart car에 있는 센서 중 빛의 반사값을 저장하는 적외선 센서를 이용하였다.
적외선 센서를 이용하여 Smart car 하단 부분의 색을 파악하고,
이를 이용하여 초기값을 설정하여 빨강, 노랑, 초록, 흰색을 구분하도록 설정한다.

먼저 제작된 지도를 주행하도록 블루투스 통신 리모콘을 사용하여 조작하도록 하였다.
이를 바탕으로 주행 중 색을 인지한 경우 스마트카는 속도를 줄이고,
통신을 통해 adoxx에 인지한 해당 값을 넘겨주게 된다.

사용자는 지도의 길만 표시된 백지 지도를 가지고 있는 상태에서,
Smart car가 탐색을 끝낸 후 위험 요소가 표식된 지도를 얻게 된다.
