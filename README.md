
## 🤔 这是什么？
它是一个工作流。可快速构建指定架构/平台的docker镜像

# 下载

参考 [docker 加速](https://zhoukekestar.github.io/notes/2024/10/04/docker.html)

1. 通过 github actions 输入镜像名称并执行下载，并上传到 阿里云oss
2. 痛过 oss 地址，下载镜像 `curl http://xxx.oss-ap-southeast-1.aliyuncs.com/arm64-images.tar.gz > arm64-images.tar.gz`

# 加载

```sh
$ tar -zxvf ./arm64-images.tar.gz
$ docker load -i xxx.tar
```

# 管理删除

* 为避免产生 oss 存储费用，下载完成后，记得在阿里云手机端删除相关文件
