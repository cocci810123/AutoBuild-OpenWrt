1. 把 public.zip 解压至系统根目录 

2. 然后按需执行以下命令:

   x86-64系统使用
   ```  docker volume create portainer_data
     docker run -d -p 9000:9000 -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data -v /public:/public portainer/portainer:1.20.2
     
      
   ARM64系统使用
   ```  docker volume create portainer_data
     docker run -d -p 9000:9000 -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data -v /public:/public portainer/portainer:linux-arm64-1.20.2
     ```

3. 您只需要使用浏览器访问运行Portainer的Docker引擎的端口9000即可, 官方安装文档详见 https://www.portainer.io/installation/

4. 如果遇到错误或者汉化不成功, 请停止或者删除Portainer容器, 重新覆盖public中的文件, 再执行一次RUN命令
