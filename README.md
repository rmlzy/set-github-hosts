# set-github-hosts

一键配置 github 可用的 hosts (仅支持 MacOS)


## 如何使用

```shell script
# 下载代码
git clone git@github.com:rmlzy/set-github-hosts.git

# 安装依赖
cd set-github-hosts
pip3 install requests

# 执行 set-github-hosts.py
# 由于需要改动 /etc/hosts 文件, 需要 sudo 权限
sudo python3 ./set-github-hosts.py
```


## 配置到 zsh 中

```shell script
vi ~/.zshrc

# 添加一行
alias updategithub= "sudo python /your_path/set-github-hosts/set-github-hosts.py"

# 使 .zshrc 配置生效
source ~/.zshrc

# 执行 updategithub 即可
updategithub
```


## LICENSE
MIT