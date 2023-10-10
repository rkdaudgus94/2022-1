<div align="center">
    <h1>⏰VHDL Clock System⏰</h1>
</div>

<div align="left">
    
## ✍️ : [프로젝트 설계목표]

디지털 직접 회로의 설계를 위한 하드웨어 기술 언어인 HDL을 학습하고 이를 바탕으로 시계를 설계한다. 
기존의 시계에 개인 기능을 추가하여 작동이 잘 되는지 훈련 키트를 이용하여 설계 결과를 확인하며, 회로 설계 능력 향상이 프로젝트의 궁극적 목표이다.


## ↖️ : [방향성 및 역할 분담]

1) 이번 프로젝트의 목표는 디지털시계에 개인 기능을 추가하여 키트로 작동 여부 확인 

2) DIP SWITCH를 통해 모드를 변경
- DIP SWITCH가 모두 0일 때 모드 0 (RESET(SW 0번)일 때 LCD에 2022년 6월 09일 11시 30분 30초로 표시되고 이 기능일 때 날짜, 요일, 시간을 확인할 수 있습니다) - 공통과제
- DIP SWITCH 1번만 1일 때 모드 1 (시계의 날짜 요일, 시간을 설정할 수 있는 기능) - 개인 기능: 황태언
- DIP SWITCH 2번만 1일 때 모드 2 (알람이 울리면 UART를 통한 송수신 기능) - 개인 기능: 이혜선 
- DIP SWITCH 3번만 1일 때 모드 3 (UART를 통한 송수신 기능으로 모드 변경) - 개인 기능: 강명현 
## 🔲 : [블록선도]
</div>

<div align="center">

<img width="806" alt="image" src="https://github.com/rkdaudgus94/VHDL-clock-system/assets/76949032/df3cd3c2-1a0f-4432-9f02-81b595cad00e">

</div>

<div align="left">
    
## 🛠️ : [동작여부]
<br>
</div>

## ⏰MODE_WATCH(시계 기본 기능)

<div align ="center">
<img width="807" alt="image" src="https://github.com/rkdaudgus94/VHDL-clock-system/assets/76949032/3127d5c1-931c-45fe-9670-70b18e4863db">
</div>

## ⏰MODE_WATCH_SET(시계의 연도, 날짜, 시간 설정이 가능)

<div align = "center">
<img width="807" alt="image" src="https://github.com/rkdaudgus94/VHDL-clock-system/assets/76949032/d48ef5c7-addb-4768-869d-ccbb39acc4aa">
</div>

## ⏰MODE_UART_TX_ALARM(UART 알람 모드)

<div align = "center">
<img width="807" alt="image" src="https://github.com/rkdaudgus94/VHDL-clock-system/assets/76949032/0f4e2ec7-cd4b-4356-ab7e-9561a5a46490">
</div>

## ⏰MODE_UART(UART TX/RX를 통한 모드 변경)

### 🔹MODE_WATCH = "!"
<div align = "center">
<img width="700" alt="image" src="https://github.com/rkdaudgus94/VHDL-clock-system/assets/76949032/98a93039-5566-4041-b0d5-9155f0c1d891">
</div>

### 🔹MODE_WATCH_SET = "@"
<div align = "center">
<img width="700" alt="image" src="https://github.com/rkdaudgus94/VHDL-clock-system/assets/76949032/4733729e-3c29-49c3-9635-a1149923bedc">
</div>

### 🔹MODE_WATCH_SET = "#"
<div align = "center">
<img width="700" alt="image" src="https://github.com/rkdaudgus94/VHDL-clock-system/assets/76949032/70298d11-a1b5-4880-b53c-066883f26f41">
</div>

### 🔹MODE_UART = "$"
<div align = "center">
<img width="700" alt="image" src="https://github.com/rkdaudgus94/VHDL-clock-system/assets/76949032/e9680c2a-11f7-4f2e-80af-fe5d5bb8d8fb">
</div>

<div align="left"> 
    
## 📇 : [TEST BENCH(시계 정상작동)]
</div>


<div align = "center">
<img width="807" alt="image" src="https://github.com/rkdaudgus94/VHDL-clock-system/assets/76949032/22a36da7-a7c0-47d4-a3a5-7ec2e9e19fb5">
</div>

<div align="left"> 
    
## 🧸 : [고찰]
</div>
<br>
디지털시계를 제작하는 데 이론적인 부분이 매우 부족하다는 걸 느꼈습니다. 코드를 작성하면서 이론 공부도 같이 할 수 있어 이론과 실습의 공부가 많이 되었던 것 같습니다.


모듈 작성하면서 모듈 이름을 다르게 쓰는 등 사소한 오류로 인해 컴파일되지 않거나 공식을 잘 못 사용하여 동작하지 않은 오류를 통해 문제를 해결하는 능력을 기를 수 있었고 동작하는 오류를 수정하면서 어떤 동작으로 동작하는지를 알아갈 수 있는 시간이었습니다.

이 수업을 통해 Quartus Prime 프로그램을 통해 새로운 언어를 배울 수 있는 소중한 시간이 되었고 앞으로의 프로젝트를 진행할 때 Quartus Prime 프로그램을 사용하여 진행할 수 있는 능력을 배울 수 있었습니다. 

또한 팀 프로젝트를 진행하면서 새로운 사람과의 만남을 통해 좋은 교류를 나눌 수 있었고 부족한 부분을 채울 수 있었습니다. 앞으로의 학교생활에 있어 좋은 인연을 만들어갈 수 있는 시간도 될 수 있어 좋았던 시간이었습니다.

팀 프로젝트를 시작하고 진행하면서 오류와 동작 확인 실패를 겪으면서 속상하기도 하고 무기력해지기도 했지만, 성공을 확인했을 때의 기분을 잊지 못할 것 같습니다. 이러한 경험으로 앞으로의 팀 프로젝트나 개인 과제 등 수행할 때 이 경험을 떠올려 열심히 해낼 수 있을 것으로 생각됩니다.

디지털시계 제작, 팀 프로젝트 통해 많은 것을 느끼고 배워나갈 수 있는 시간이 되었습니다.
