# JuHang_Box
2023 위치기반 우수 BM 공모전 아이디어를 기반한 개발 프로그램입니다. 

![2023 대한민국 위치정보 우수 비지니스 모델 공모전](https://github.com/Yoonchulchung/JuHang_Box/blob/main/2023%20%EB%8C%80%ED%95%9C%EB%AF%BC%EA%B5%AD%20%EC%9C%84%EC%B9%98%EA%B8%B0%EB%B0%98%20%EA%B3%B5%EB%AA%A8%EC%A0%84.PNG)

2023.08 - 2023.12 

정윤철 | 자율주행 로봇 위치기반 동선 최적화 서비스

Docker를 활용하여 ROS melodic으로 개발을 진행했습니다. 백업을 위해 개발 버젼을 달리하여 GITHUB를 통해 배포하고 있습니다.

version
---
```
$ docker pull ghcr.io/yoonchulchung/juhang_box:base.1
$ docker pull ghcr.io/yoonchulchung/juhang_box:base
```

개발 환경:
---
CPU: Ryzen7 6800HS

GPU: RTX3060 6GB



---
### 환경변수 및 GUI 설정

#### 그래픽 문제 해결:

```bash
export LIBGL_ALWAYS_INDIRECT=1 # Container 안에서
xhost +local:docker # Host 에서
```

#### ROS 환경변수:
```bash
source /opt/ros/melodic/setup.zsh # Container 안에서
```

