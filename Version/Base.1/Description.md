Nvidia 그래픽 문제가 있어서 Dockerfile을 만들고 다음과 같이 작성함.

```
FROM ghcr.io/yoonchulchung/juhang_box:base

# Arguments picked from the command line!
ARG user
ARG uid
ARG gid

# nvidia-docker container
ENV NVIDIA_VISIBLE_DEVICES \
    ${NVIDIA_VISIBLE_DEVICES:-all}
ENV NVIDIA_DRIVER_CAPABILITIES \
    ${NVIDIA_DRIVER_CAPABILITIES:+$NVIDIA_DRIVER_CAPABILITIES,}graphics
```

이후 Dockerfile을 build 하여 다시 이미지를 생성함.

```bash
docker build -f Dockerfile -t ghcr.io/yoonchulchung/juhang_box:base.1
```
