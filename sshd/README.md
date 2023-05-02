# 带有ssh的镜像
 基于systemd镜像创建

docker build -t wuzhenhua/sshd:1.0.0 .

docker run --privileged -d wuzhenhua/systemd:1.0.0
