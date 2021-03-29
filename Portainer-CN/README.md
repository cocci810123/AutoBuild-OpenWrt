# Docker管理面板Portainer中文汉化说明

由于Lean大神的固件中，使用的是Portainer英文版Docker管理面板, 所以需要编译安装后, 自己汉化成中文版，具体汉化方法如下:

1. 点击Portainer-CN.zip进入文件界面, 点击Download按钮下载, 并解压至public目录

2. 将解压后的public目录上传至Linux系统根目录

3. 然后按需执行以下命令:

    **x86-64系统使用**
    ```docker volume create portainer_data
    docker run -d -p 9000:9000 -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data -v /public:/public portainer/portainer:1.20.2
    ```
      
    **ARM64系统使用**
    ```docker volume create portainer_data
    docker run -d -p 9000:9000 -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data -v /public:/public portainer/portainer:linux-arm64-1.20.2
    ```
    
4. 您只需要使用浏览器访问运行Portainer的Docker引擎的端口9000即可

5. 如果遇到错误或者汉化不成功, 请停止或者删除Portainer容器, 重新覆盖public中的文件, 再执行一次RUN命令

---
+ *Portainer官方安装文档请详见 [Portainer官方网站](https://www.portainer.io/installation/)*
+ *此文档说明及汉化文件的版权归Mark's Blog所有, 具体请详见 [原文链接](https://www.quchao.net/Portainer-CN.html)*
