# Docker Images Sync

利用 GitHub Actions 同步 Docker Hub 上的镜像到阿里云容器镜像服务。

Sync Docker images from Docker Hub to Alibaba Cloud Container Registry using GitHub Actions.


## 使用方法

1. Fork 本仓库到你的 GitHub 账号；
2. 在你的仓库中创建 Actions secrets，添加以下变量：
   - `ALIYUN_USERNAME`: 阿里云容器镜像服务用户名；
   - `ALIYUN_PASSWORD`: 阿里云容器镜像服务密码。
3. 在你的仓库中创建 Actions variables，添加以下变量：
   - `ALIYUN_REGISTRY_URL`: 阿里云容器镜像服务仓库地址，例如 `crpi-m3uf6x9vqbvzhd0p.cn-hongkong.personal.cr.aliyuncs.com；
   - `ALIYUN_REGISTRY_NAMESPACE`: 阿里云容器镜像服务命名空间，例如 `my-namespace`。
4. 将你需要同步的镜像以 `name:tag` 的格式添加到 images.txt 文件中。

## How To Use

1. Fork this repository to your GitHub account;
2. Create Actions secrets in your repository and add the following variables:
   - `ALIYUN_USERNAME`: username for Alibaba Cloud Container Registry;
   - `ALIYUN_PASSWORD`: password for Alibaba Cloud Container Registry.
3. Create Actions variables in your repository and add the following variables:
   - `ALIYUN_REGISTRY_URL`: Alibaba Cloud Container Registry repository URL, e.g. `crpi-m3uf6x9vqbvzhd0p.cn-hongkong.personal.cr.aliyuncs.com`;
   - `ALIYUN_REGISTRY_NAMESPACE`: Alibaba Cloud Container Registry namespace, e.g. `my-namespace`.
4. Add the images you want to sync in the `images.txt` file in the format `name:tag`.
