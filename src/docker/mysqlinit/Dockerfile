#  这个是构建MySQL的dockerfile
FROM mysql:5.7

# mysql的工作位置
ENV WORK_PATH /usr/local/

# 定义会被容器自动执行的目录
ENV AUTO_RUN_DIR /docker-entrypoint-initdb.d

COPY xyy.sql  $AUTO_RUN_DIR/
#把要执行的shell文件放到/docker-entrypoint-initdb.d/目录下，容器会自动执行这个shell

# 设置容器启动时执行的命令
#CMD ["sh", "/docker-entrypoint-initdb.d/import.sh"]
