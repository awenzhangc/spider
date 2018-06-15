# 环境：

基本的环境估计够很多程序员喝一壶的

本地的开发环境的ubuntu

1、pyenv + virtualenv实现不同python版本的切换

参考安装地址

https://blog.csdn.net/databatman/article/details/53955828

https://www.jianshu.com/p/158d880b2d41


## 开始安装

> sudo apt-get install curl git-core

有个github的地址不能访问

下面这个地址访问出错
> curl -L https://raw.githubusercontent.com/pyenv/pyenv-installer/master/bin/pyenv-installer | bash

使用下面这个进行访问
> curl -L https://raw.github.com/yyuu/pyenv-installer/master/bin/pyenv-installer | bash


```
export PYENV_ROOT="${HOME}/.pyenv"

if [ -d "${PYENV_ROOT}" ]; then
  export PATH="${PYENV_ROOT}/bin:${PATH}"
  eval "$(pyenv init -)"
fi

```

搞完环境，就source一下
```
source ~/.bashrc
```


安装python依赖包，没去细理解这个意思，反正都执行了
```
sudo apt-get install python-pip git make build-essential libssl-dev zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev

sudo apt-get install make build-essential libssl-dev zlib1g-dev
sudo apt-get install libbz2-dev libreadline-dev libsqlite3-dev wget curl
sudo apt-get install llvm libncurses5-dev libncursesw5-dev
# sudo apt-get update


```

常用的环境修改命令如下
```
创建环境变量
pyenv virtualenv 2.7.15 env2.7.15
pyenv versions
pyenv activate env2.7.15
pyenv deactivate
pyenv uninstall env2.7.15

```


