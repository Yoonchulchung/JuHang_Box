# JuHang_Box
2023 위치기반 우수 BM 공모전 아이디어를 기반한 개발 프로그램입니다. 

![2023 대한민국 위치정보 우수 비지니스 모델 공모전](https://github.com/Yoonchulchung/JuHang_Box/blob/main/2023%20%EB%8C%80%ED%95%9C%EB%AF%BC%EA%B5%AD%20%EC%9C%84%EC%B9%98%EA%B8%B0%EB%B0%98%20%EA%B3%B5%EB%AA%A8%EC%A0%84.PNG)
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

