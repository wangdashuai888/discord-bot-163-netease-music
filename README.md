# discord-bot-163-netease-music
该机器人能播放网易云音乐

[![discord-bot-163-netease-meusic](https://socialify.git.ci/vinelin/discord-bot-163-netease-meusic/image?description=1&font=Inter&language=1&owner=1&pattern=Brick%20Wall&theme=Light)](https://github.com/vinelin/discord-bot-163-netease-meusic/)

python3版本：3.6.12

# 使用
### 1.首先安装 discord.py[voice]

     # Linux/macOS
     python3 -m pip install -U "discord.py[voice]"

     # Windows
     py -3 -m pip install -U discord.py[voice]

### 2.安装requests库和pycryptodome库
     安装 ffmpeg 和 opus
     # ubuntu 
          libogg0 (>= 1.3.0)
          libopus0
          opus-tools

### 3.将自己的TOKEN和USERNAME加入config_forexample.ini，并修改文件名为config.ini

### 4.根据运行环境取消需要的注释
     #windows
     # if not discord.opus.is_loaded():
     #     discord.opus.load_opus('opus')

     # #linux
     # if not discord.opus.is_loaded():
     #     discord.opus.load_opus('/usr/lib/x86_64-linux-gnu/libopus.so.0')
     
### 5.运行
    python3 main.py
 
# 文件说明
main.py - bot主要代码
encode.py - 为网易云请求加密和解密使用的代码
netease_dl.py - 音乐搜索，下载，删除代码
    
# 功能介绍
.join 
让机器人加入语音
.quit  
让机器人退出语音   
.play 关键字  
播放网易云上的音乐  
.skip  
切换到下一首歌  
.queue  
查看等待播放的歌曲  
.remove 序号  
删除所选歌曲  
.stop  
停止播放  

# TODO
  增加搜索结果列表选歌
  解决异步并发支持
  优化Timing
  增加歌单播放
  支持Spotify

# 致谢
### [discord.py](https://github.com/Rapptz/discord.py)
### [网易云API分析](https://www.dazhuanlan.com/2020/03/20/5e73cb9a327c6/)
### [Netease Music Bot for Discord](https://github.com/vinelin/discord-netease-music-bot)
### [Discord-bot-163-netease-music](https://github.com/vinelin/discord-bot-163-netease-music)
