# InternLM2-Tutorial-Assignment-Lecture2
## Lecture 2
## 第2节课 【轻松玩转书生·浦语大模型趣味 Demo】
[视频](https://www.bilibili.com/video/BV1AH4y1H78d/)   2024.3.31  书生·浦语角色扮演小组长【那路】 

### 第2节课 笔记

#### 环境配置, 过入开发机后，执行下列命令：   
```
studio-conda -o internlm-base -t demo
# 与 studio-conda 等效的配置方案
# conda create -n demo python==3.10 -y
# conda activate demo
# conda install pytorch==2.0.1 torchvision==0.15.2 torchaudio==2.0.2 pytorch-cuda=11.7 -c pytorch -c nvidia
```

配置完成后，进入到新创建的 conda 环境之中：  
```
conda activate demo
```
  

####  环境包安装，执行下列命令：
```
pip install huggingface-hub==0.17.3
pip install transformers==4.34 
pip install psutil==5.9.8
pip install accelerate==0.24.1
pip install streamlit==1.32.2 
pip install matplotlib==3.8.3 
pip install modelscope==1.9.5
pip install sentencepiece==0.1.99
```
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

InternLM2-chat-1.8B 模型对话效果：   
![](./storytelling.png)   


猪猪chat-InternLM2 模型对话效果：   
![](./storytelling2.png)   




#### windows PowerShell 端口环境配置
对端口环境配置本地 `PowerShell`
```
# 从本地使用 ssh 连接 studio 端口
# 将下方端口号 38374 替换成自己的端口号 40491
ssh -CNg -L 6006:127.0.0.1:6006 root@ssh.intern-ai.org.cn -p 40491
# 复制密码
```

### 第2节课 作业


