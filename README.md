# VR_Haptic_Drum!
![EntiImage](https://user-images.githubusercontent.com/89020936/158392236-17e3b8ce-04bb-4cec-90da-85dd02a97bb2.png)

### [1.주제](#주제)
   
## ⭐ 주제
  
- **VR 환경에서 사용자에게 실감나는 연주를 제공하는 VR 햅틱 드럼**
- 교내 졸업작품 경진대회 **은상**
- 2021 임베디드 소프트웨어 경진대회 **입선**
- MWU KR Award 2021 **Best Student 부문 Top 3**   

<br/>
   
## ✔️ 주요 기능
     
- HMD를 이용해 드럼이 있는 **가상환경**을 시연
- 가상 드럼 타격 시 **햅틱 신호**로 타격 느낌 제공
- 드럼 연주를 학습할 수 있는 **두더지 게임 형식의 콘텐츠** 제공   

<br/>
   
## 🙋🏻‍♂️ 담당

- **팀원** (팀장1 팀원2 구성)
- 드럼스틱과 Unity 간의 **연동 환경 구현**
- **드럼 타격 판정 알고리즘 구현**
- 드럼스틱 **각속도 및 회전 인식 값 처리**
- IMU와 LeapMotion 위치 **좌표값 보완 및 수정**   

<br/>
   
## ✏️ 개발 동기
![image](https://user-images.githubusercontent.com/89020936/158837317-e122c78d-555d-45d0-ae8f-144096e01b12.png)


- 드럼 연주 ⇒ 충분한 넓이와 방음 처리가 가능한 공간이 필요
- 따라서 공간의 제약으로부터 자유롭고, 소음 피해가 없는 VR 환경을 생각함
- 더불어 햅틱 요소를 접목해 몰입감을 제공할 수 있는 가상현실 기반의 햅틱 드럼 개발을 시작   

<br/>
   
## 🪧 개발 목표
![image](https://user-images.githubusercontent.com/89020936/158837347-e0e06b4a-69a3-4506-bada-e66f92076e7f.png)


- **햅틱요소를 포함한 하드웨어(드럼 스틱)가 추가된 VR 애플리케이션을 개발**
- **드럼 학습 콘텐츠를 추가**하여 드럼 연주에 익숙하지 않은 입문자들도 쉽게 드럼 연주를 배워 나갈 수 있도록 하는 애플리케이션을 개발   

<br/>
   
## 🥁 개발 중 발생한 장애 요인과 해결 방안

- **Gymbal Lock 문제**
    - 오일러(Euler) 좌표계를 사용하는 **IMU의 특성상, Unity 내에서 회전 처리 시 짐벌락이 발생**
    - 특정 각도에서 드럼 스틱 하드웨어의 Y축과 X축이 고착되는 현상을 파악
    - **IMU의 각도 출력 데이터 포맷 형식을 쿼터니온(Quaternion)으로 변경하고 행렬식 계산을 통한 좌표 보정을 통해 짐벌락 발생을 해결**
    
- **가상공간 내 드럼이 두 번 타격 되는 문제**
    - 사용자가 드럼 타격 시, **드럼이 연속적으로 두 번 타격 되는 현상이 발생**
    - 드럼 스틱의 **현재 각도와 충돌 시 시간을 측정하는 알고리즘을 추가**
    - 드럼이 타격 되는 데까지 걸리는 시간을 측정하는 방법으로 타격하는 행위를 판단하여 드럼이 두 번 타격 되는 문제를 해결
    
- **드럼 스틱 하드웨어의 내구성 문제**
    - 조금의 충격에도 3D 프린팅한 드럼 스틱의 하우징이 파손되는 문제가 발생
    - 드럼 스틱이 사용하는 전지와 유사한 크기의 전지가 들어가는 알루미늄제 손전등을 찾고, 손전등의 손잡이 부분을 드럼 스틱과 결합되도록 가공을 진행   

<br/>
   
## 🧐 개발 작품의 필요성

- 권장 안전거리(1*1m)만 확보된다면 **어떠한 환경에서나 실행 가능**
- **저렴한 가격**에 본 시스템을 구비할 수 있을 것으로 기대
- 기본적인 드럼 학습을 위한 콘텐츠를 포함하고 있기에 입문 시에 별도의 레슨을 위한 **경제적 지출 역시 줄일 수 있을 것으로 기대**
- **사용자가 타격한 드럼의 종류(심벌즈, 북)에 적합한 진동 피드백을 발생**시켜 실감 나는 가상환경에서의 드럼 연주 경험 제공

<br/>
   
## 📺 시연 및 소개 영상
[![video1](http://img.youtube.com/vi/mGyuCK_KMoM/0.jpg)](https://youtu.be/mGyuCK_KMoM)
[![video1](http://img.youtube.com/vi/1PxI6T_X53Y/0.jpg)](https://youtu.be/1PxI6T_X53Y)
