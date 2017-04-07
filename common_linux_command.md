# 常见linux命令 (一个快且脏的说明)

## cd 
### 名称 
变更目录 change directory

### 作用
变更工作目录.

### 常见选项和使用实例

1. `$ cd path`
    - `path` 绝对或相对路径
    - 将当前目录变更为 `path`
    - 实例1 |> `$ cd workspace ` 将工作目录变更为当前工作目录下的workspace文件夹

2. `$ cd `
    - 将工作目录变更为当前用户的家目录，即`~`(/home/**用户名**)

## rm
### 名称 
删除 remove

### 作用
删除文件或文件夹

### 常见选项和使用实例
1. `$ rm filename`
    - `filename` 待删除的文件名
    - 实例 |> `$ rm log.txt` 删除log.txt.

2. `$ rm -r directory`
    - `-r` 递归删除目录
    - `directroy` 待删除的目录 
    - 实例 |> `$ rm -r logs` 删除logs目录及它的所有内容.

3. `$ rm -f filename`
    - `-f` 强制删除，将不会询问是否删除写保护文件等
    - `filename` 待删除的文件名
    - 实例 |> `$ rm -r logs.protect` 删除logs.protect文件且不进行询问.

## mkdir

### 名称 
创建目录 make directory 

### 作用
创建目录

### 常见选项和使用实例
1. `$ mkdir directory_name`
    - `directory_name` 待创建目录名称
    - 实例 |> `$ mkdir logs` 在当前目录下创建一个名为logs的目录.


## mv
### 名称 
移动 move

### 作用
移动文件或目录

### 常见选项和使用实例
1. `$ mv filename directory`
    - `filename` 待移动文件**或目录**
    - `directory` 目的地目录
    - 实例 |> `$ mv 100.log logs` 将100.log 移动到 logs 目录下
2. `$ mv filename1 filename2 ... filenameN **directory**`
    - `filename1 filename2 ... filenameN` 多个待移动文件**或目录**
    - `directory` 目的地目录
    - 实例 |> `$ mv 100.log 200.log abc.log 300.log logs` 将100.log, 200.log, abc.log, 300.log 移动到 logs 目录下


## bash
### 名称 
bash 
### 作用
调用bash shell 执行shell脚本
### 常见选项和使用实例
1. `$ bash script`
    - `script` 待执行的脚本文件
    - 实例 |> `$ bash run.sh` 执行run.sh脚本

## df
### 名称 
### 作用
### 常见选项和使用实例

## du
### 名称 
### 作用
### 常见选项和使用实例

## sudo
### 名称 
以超级用户权限执行 superuser do 

### 作用
暂时性的使用超级用户权限(root权限)

### 常见选项和使用实例
1. `$ sudo command `
    - `command` 待执行的命令
    - 实例 |> `$ sudo apt install opencv-python` 以root权限调用包管理器安装软件.


## python, python3
### 名称 
python, python3

### 作用
调用python2, python3解释器执行python脚本

### 常见选项和使用实例
1. `-u` 强制要求输出流不进行缓冲
2. `--version` 显示当前python版本

## nohup
### 名称 
### 作用
### 常见选项和使用实例

## tee
### 名称 
### 作用
### 常见选项和使用实例

## vim
### 名称 
vim 

### 作用
启动vim编辑器编辑文件

### 常见选项和使用实例
1. `vim` 直接启动vim， 启动后进入主界面
2. `vim filename`  调用vim编辑文件
    - `filename` 待编辑的文件名