---
layout: post
title: Python, Django e Pyenv no Ubuntu
category: main
---

### Como configurar um ambiente desenvolvimento Python no Ubuntu

#### 1 - Instalação das dependências dp pyenv:

```bash
$ ~ sudo apt-get install -y make build-essential libssl-dev zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm libncurses5-dev
```

#### 2 - Instalação do pyenv:

```bash
$ ~ curl -L https://raw.githubusercontent.com/yyuu/pyenv-installer/master/bin/pyenv-installer | bash
```

#### 3 - Configurando o arquivo ~/.bashrc:

```bash
$ cd ~
$ nano .bashrc
$ # adicione as linhas abaixo no final do arquivo:
export PATH="/home/marcello/.pyenv/bin:$PATH"
eval "$(pyenv init -)"
eval "$(pyenv virtualenv-init -)"
$ # por último, atualize o .bashrc com o comando:
$ source .bashrc
```

#### 4 - Visualizando as versões instaladas do python:

```bash
$ ~ pyenv versions
```

#### 5 - Para instalar uma determinada versão (ex. python 3.5.0):

```bash
$ ~ pyenv install 3.5.0
```

#### 6 - Para mudar da versão do sistema para a versão instalada:

```bash
$ ~ pyenv global 3.5.0
```

e com o comando abaixo, é possível ver as versões disponíveis:

```bash
$ ~ pyenv versions
```

#### 7 - Instalação do PyCharm via apt-get (opcional):

```bash
$ ~ sudo add-apt-repository ppa:mystic-mirage/pycharm

$ ~ sudo apt-get update

$ ~ sudo apt-get install pycharm
```

#### REFERÊNCIAS:

* [Pyenv](https://github.com/yyuu/pyenv-installer)

* [Pyenv - Common build problems](https://github.com/yyuu/pyenv/wiki/Common-build-problems)

* [How to Install PyCharm IDE in Ubuntu 14.04/15.04](http://ubuntuhandbook.org/index.php/2015/07/install-pycharm-ubuntu-1404)