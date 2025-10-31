# 一、 安装python
1. python官网下载安装包，安装的python3.6.8
2. 双击进行安装，安装时自动配置了环境变量
```
echo $PATH # 查看环境变量
vim ~/.zshrc # 配置用户环境变量
source ~/.zshrc # 让环境变量生效（注意：只需要运行一次，运行多次会有重复）
where python3 # 查看python3的位置
which python3 # 查看当前使用哪个python
```

# 二、 安装vscode
1. 安装vscode，快捷键 `shift + cmd + p` ，将code添加到环境变量
2. 安装插件
- python插件
- jupyter插件（注意：jupyter连接ipykernel连接python）
- mackdown插件：预览快捷键 `shift + cmd + v`

# 三、 安装git
```
xcode-select --install # 换安装很多工具，包括：git、python等（注意：这里又安装了一个版本的python）
xcode-select -p # 查看xcode安装位置
```

# 四、 python虚拟环境
python虚拟环境有很多种，包括 pyenv + venv、anaconda等。
## 1、venv
我将venv创建虚拟环境分为两种：
1. 全局虚拟环境，所有的项目都可以指向该虚拟环境
2. 项目级虚拟环境，将虚拟环境放到当前项目目录下，一般情况只有当前项目使用该环境
```
mkdir model # 为虚拟环境创建目录
cd model
python3 -m venv . # 创建虚拟环境到当前目录
source ./bin/activate # 激活虚拟环境
pip install jupyter -i https://mirrors.aliyun.com/pypi/simple # 安装jupyter其中包含了ipykernel、jupyter notebook、jupyter lab等工具
jupyter lab --notebook-dir="/Users/sunjiajun/Documents/代码" # 启动Jupyter lab服务，并指定工作路径
```