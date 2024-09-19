# Bugs
- 执行`git clone xxxx`的时候显示：`error setting certificate file: F:/桌面/Git/mingw64/etc/ssl/certs/ca-bundle.crt`。
  - 你需要检查 ca-bundle.crt 文件是否存在。如果你确定文件确实存在，那么路径可能配置错误。
    - 检查文件是否存在于 F:/桌面/Git/mingw64/etc/ssl/certs/ca-bundle.crt 这个路径。
    - 如果不存在，你可以尝试重新安装 Git，确保安装时包含了证书文件。
  - 如果存在，那此时是由于 Git 无法找到或无法访问正确的证书文件导致的，此时可以手动设置正确的证书文件路径。使用以下命令重新配置 Git 的证书路径：`git config --global http.sslCAInfo "xxxx"
  - xxx 是你的 `ca-bundle.crt`路径`
