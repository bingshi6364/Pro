#拉取runtime父镜像，运行aspnet core应用必须要用runtime
FROM microsoft/dotnet:2.2-aspnetcore-runtime
#设置容器工作目录
WORKDIR /DockerDemo
#把当前目录的所有文件copy到工作目录中
COPY . /DockerDemo
#暴露一个端口让外部可以访问
EXPOSE 80
#容器入口命令，即容器启动时执行dotnet DockerDemo.dll命令
ENTRYPOINT ["dotnet", "DockerDemo.dll"]