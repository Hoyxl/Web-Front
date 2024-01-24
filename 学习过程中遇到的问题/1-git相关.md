# Git 相关问题
## git clone报错
- 报错如下：fatal: unable to access 'https://github.com/Hoyxl/Web-Front.git/': Failed to connect to github.com port 443 after 21111 ms: Couldn't connect to server
- 实际上是代理端口不对，报错解决为查看Clash对应的代理端口，并做如下设置：
  ```git config --global https.proxy http://127.0.0.1:49814```，```git config --global https.proxy http://127.0.0.1:49814```
- 再尝试`git clone`，发现成功了。

