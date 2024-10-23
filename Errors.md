# git clone xxxx
错误提示：
> fatal: unable to access 'https://github.com/Carolynhomes/Office.git/': OpenSSL SSL_read: SSL_ERROR_SYSCALL, errno 0

解决办法：

执行完这两行就可以继续 git clone了
> git config --global --unset http.proxy
> 
> git config --global --unset https.proxy
