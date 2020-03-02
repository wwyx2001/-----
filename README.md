# -----
Day1
达成：
在linux服务器上Docker拉取CoolQ环境

sudo docker pull richardchien/cqhttp:latest

创建镜像的参数

docker run -ti --rm --name cqhttp-test \
--network host \
-v $(pwd)/coolq:/home/user/coolq \
-e COOLQ_ACCOUNT=XXXXX \(QQ号）
-e CQHTTP_POST_URL=http://127.0.0.1:9999 \
-e CQHTTP_SERVE_DATA_FILES=yes \
richardchien/cqhttp:latest
