# Kubernetes
Kubernetes编排示例
阿里云镜像地址：www.aliyun.com
1 apollo.yaml包括configservice和adminservice，容器namespace：goa
1.1 configservice定义端口7007，adminservice定义端口7008，如需要使用默认端口，需要从新下载apollo，并制作镜像
1.1 使用前先创建configmap：
  数据库链接信息 kubectl create configmap -n goa --from-file=/zhouc/apollo-configservice/config/application-github.properties
