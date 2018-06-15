# 环境：
基本的环境估计够很多程序员喝一壶的
本地的开发环境的ubuntu

1、pyenv + virtualenv实现不同python版本的切换
参考安装地址
https://blog.csdn.net/databatman/article/details/53955828

sudo apt-get install curl git-core
有个github的地址不能访问
curl -L https://raw.github.com/yyuu/pyenv-installer/master/bin/pyenv-installer | bash

‘’‘
export PYENV_ROOT="${HOME}/.pyenv"

if [ -d "${PYENV_ROOT}" ]; then
  export PATH="${PYENV_ROOT}/bin:${PATH}"
  eval "$(pyenv init -)"
fi
’‘’

sudo apt-get install python-pip git make build-essential libssl-dev zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev


2、