# ArkPixels 介绍

ArkPixels是一个开源的图片浏览系统，可以方便地管理和展示图片。
注意：ArkPixels还处于开发阶段，功能还不完整，请不要在生产环境中使用。

# 部署

要部署ArkPixels，请按照以下步骤进行：

1. 下载ArkPixels源码：

```shell
git clone https://github.com/DemonPlayer00/ArkPixels.git
```

2. 安装依赖：

```shell
sudo apt install nodejs npm mariadb #Debian/Ubuntu
sudo yum install nodejs npm mariadb #CentOS/Fedora
sudo pacman -S nodejs npm mariadb #Arch Linux

cd ArkPixels
npm install
```

3. 配置数据库：

```shell
sudo mariadb -u root -p # 输入密码
SOURCE struct.sql; # 导入数据库结构
```

4. 填写配置文件：

```shell
cp .env_list .env # 复制配置文件
vim .env # 编辑配置文件
```

5. 启动服务：

```shell
sudo node index.js # 启动服务
```