# docker-compose-wordpress
docker 构建WordPress 一代经典建站


# 构建，启动项目中的 全部/部分 服务容器（建议先拉取镜像，这样会跳过构建过程）
docker-compose up -d
docker-compose up -d   wordpress-db redis phpredisadmin wordpress

# 重启项目中的 全部/部分 服务容器
docker-compose restart
docker-compose restart wordpress-db redis phpredisadmin wordpress
# 停止并移除项目中的 全部/部分 服务容器
docker-compose rm -f -s
docker-compose rm -f -s wordpress-db redis phpredisadmin wordpress
# 列出项目中的服务容器
docker-compose ps
# 查看项目中的服务容器内运行的进程
docker-compose top


