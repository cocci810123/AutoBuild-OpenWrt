1. 点击 public.zip 进入文件界面并点击Download按钮下载保存

2. 把 public.zip 解压并上传至Linux系统根目录

3. 然后按需执行以下命令:

    **x86-64系统使用**
    ```docker volume create portainer_data
    docker run -d -p 9000:9000 -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data -v /public:/public portainer/portainer:1.20.2
    ```
      
    **ARM64系统使用**
    ```docker volume create portainer_data
    docker run -d -p 9000:9000 -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data -v /public:/public portainer/portainer:linux-arm64-1.20.2
    ```
    
4. 您只需要使用浏览器访问运行Portainer的Docker引擎的端口9000即可, 官方安装文档详见 [Portainer官方网站](https://www.portainer.io/installation/)

5. 如果遇到错误或者汉化不成功, 请停止或者删除Portainer容器, 重新覆盖public中的文件, 再执行一次RUN命令
