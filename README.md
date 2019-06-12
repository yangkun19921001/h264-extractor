# 如何从Wireshark 中获取 H264 视频码流

1. 首先安装wireshark软件，这个用过的人都知道它的强大之处

2. 查看安装路径下是否存在init.lua，确保disable_lua = false

3. 在init.lua 的最后加上 dofile(DATA_DIR.."rtp_h264_extractor.lua")

4. 把 rtp_h264_extractor.lua 这个文件放在 init.lua 同一个路径下

5. 重新启动 Wireshark 点击 tools 

   ![](<https://ws3.sinaimg.cn/large/005BYqpgly1g3y7dgj57yj30hx037mx3.jpg?referrer=https://cdn.sinaimg.cn.52ecy.cn>)

