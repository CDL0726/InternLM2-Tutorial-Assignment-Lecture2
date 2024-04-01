# InternLM2-Tutorial-Assignment-Lecture2
## Lecture 2
## 第2节课 【轻松玩转书生·浦语大模型趣味 Demo】
[视频](https://www.bilibili.com/video/BV1AH4y1H78d/)   2024.3.31  书生·浦语角色扮演小组长【那路】 

### 第2节课 笔记

#### 模型下载
按路径创建文件夹，
```
mkdir -p /root/demo
touch /root/demo/cli_demo.py
touch /root/demo/download_mini.py
cd /root/demo
```

双击打开 /root/demo/download_mini.py 文件，复制模型下载代码
[模型下载代码](https://github.com/InternLM/Tutorial/blob/camp2/helloworld/hello_world.md)  

执行命令，下载模型参数文件：   
`python /root/demo/download_mini.py`  

运行 cli_demo   

双击打开 /root/demo/cli_demo.py 文件，复制`cli_demo` 代码    
[cli_demo代码](https://github.com/InternLM/Tutorial/blob/camp2/helloworld/hello_world.md)   

输入命令，执行 Demo 程序：    
```
conda activate demo
python /root/demo/cli_demo.py
```

模型对话效果：   
!stortytelling2.png




#### windows PowerShell 端口环境配置
对端口环境配置本地 `PowerShell`
```
# 从本地使用 ssh 连接 studio 端口
# 将下方端口号 38374 替换成自己的端口号 40491
ssh -CNg -L 6006:127.0.0.1:6006 root@ssh.intern-ai.org.cn -p 40491
# 复制密码
```

### 第2节课 作业


