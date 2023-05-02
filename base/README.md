# 本地基础镜像
- 添加本地yum源

docker build -t wuzhenhua/base:1.0.0 .

docker run -dit -v /tmp:/tmp wuzhenhua/base bash
