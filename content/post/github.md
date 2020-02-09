---
title: "Github 更换代理设置"
date: 2020-02-09T20:56:07+08:00
draft: false
---

# github代理设置

### 两种形式： 
#### http形式：
`git clone https://github.com/xxx/git.git`


#### 修改git config：
#### 走http代理：
```
    git config --global http.proxy "http://127.0.0.1:8080" 
    git config --global https.proxy "http://127.0.0.1:8080"
```
走 socks5 代理（如 Shadowsocks）
```
    git config --global http.proxy "socks5://127.0.0.1:1080"
    git config --global https.proxy "socks5://127.0.0.1:1080"
```
注意：8080为端口号，需要查看vpn的http/socks5端口号

#### 取消设置：
```
    git config --global --unset http.proxy
    git config --global --unset https.proxy
```


