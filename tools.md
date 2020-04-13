## shell

- [Advanced Bash-Scripting Guide](http://tldp.org/LDP/abs/html/) (The Linux Document Project)
- [编写可靠 bash 脚本的一些技巧](https://mp.weixin.qq.com/s/VmM_U4RefRBHwIw8NegC8Q)
- [教你写出健壮可靠的shell脚本](https://mp.weixin.qq.com/s/mUt7yNBn5_eCcb9RHCKUbQ)
- [有了这个神器，再也不怕shell写得不对了](https://mp.weixin.qq.com/s?__biz=MzI2OTA3NTk3Ng==&mid=2649285685&idx=2&sn=cf431bfad1dc3d017b7e0ed9fafb59f2&chksm=f2f99752c58e1e44a79e1a659c087cbf4b9c3f14c4438c2d8c900ad3837389b6ae6cb0b3d33e&scene=21#wechat_redirect)




## vim

[精通 VIM ，此文就够了](https://zhuanlan.zhihu.com/p/68111471)

- 删除光标到行末的内容: `d$`
- 撤销撤销:`ctrl + r`


## linux-command-line

### find

`find . -type d -iname "__pycache__" | xargs rm -rf`

这行命令的执行的任务是:
找到当前目录及其子目录下名为`__pycache__`的目录，并且删除.

举个例子🌰，假设我执行了一个python项目，导致生成了一些cache文件，目录树🌲变成下面这样:

```bash
.
├── shell.py
└── yosh
    ├── __init__.py
    ├── __pycache__
    │   ├── __init__.cpython-36.pyc
    │   └── constants.cpython-36.pyc
    ├── buildins
    │   ├── __init__.py
    │   ├── __pycache__
    │   │   ├── __init__.cpython-36.pyc
    │   │   └── cd.cpython-36.pyc
    │   ├── cd.py
    │   └── exit.py
    ├── constants.py
    └── test_dir

```
在执行完上面这行目录之后，目录树又可以变成最开始的样子:
```bash
.
├── shell.py
└── yosh
    ├── __init__.py
    ├── buildins
    │   ├── __init__.py
    │   ├── cd.py
    │   └── exit.py
    ├── constants.py
    └── test_dir

```

 
`find . -name "*.go" | xargs grep -in "dup"`
> 在当前目录下go文件中寻找包含"dup"的行.


`sudo find / -size +1G | xargs ls -lhS`
> 清理系统中大文件用.

## git

[Git 分支管理实践 | 码云最佳实践](https://mp.weixin.qq.com/s/RSREs3MqxidPX8h8wJfv4Q)

[🌳🚀 CS Visualized: Useful Git Commands](https://dev.to/lydiahallie/cs-visualized-useful-git-commands-37p1)







## 容器


[一个在容器外用 tcpdump 命令对容器内的网络请求抓包的方法](https://mozillazg.com/2020/04/use-tcpdump-for-a-container-but-outside-container.html)




































