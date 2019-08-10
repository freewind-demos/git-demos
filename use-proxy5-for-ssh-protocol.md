首先本地有一个socks的代理，端口为1080

```
Host github.com
    User git
    PreferredAuthentications publickey
    IdentityFile ~/.ssh/id_rsa
    ProxyCommand nc -X 5 -x 127.0.0.1:1080 %h %p
```