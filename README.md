setup-ubuntu
============

### 下载 GIT 版本控制软件，接下来用它来下载设置脚本。 ###
`
sudo apt-get install git -y
`

### 下载自动安装软件包的脚本 ###
`
git clone https://github.com/zhang3/setup-ubuntu.git
`

### 执行脚本，这些脚本用来安装各种软件包。 ###
`
bash setup-android.txt
bash setup-buildroot.txt
bash setup-kernel.txt
bash setup-network.txt
bash setup-rest.txt
bash setup-server.txt
bash setup-ubuntu.txt
`
### 也可以使用一点技巧，一次性执行多个脚本： ###
`
bash setup-android.txt; bash setup-buildroot.txt; bash setup-kernel.txt; bash setup-network.txt; bash setup-rest.txt; bash setup-server.txt; bash setup-ubuntu.txt
`
或许这不叫什么技巧，但是要学会在知识不够的情况下也能达到相同的效果！
如果真的要来点技巧，那就这么做吧：
`
for f in setup*
do
bash $f
done
`

