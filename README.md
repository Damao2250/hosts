# hosts
收集的 hosts 文件


## hosts 文件在哪里？

+ Windows：%SystemRoot%\System32\drivers\etc\hosts（一般的：C:\Windows\System32\drivers\etc\hosts）

+ Android：/etc/hosts（指向/system/etc/hosts的符号链接)

+ iOS：/etc/hosts（指向/private/etc/hosts的符号链接)

+ Mac OS X 10.0–10.1.5：通过NetInfo或niload设置

+ Mac OS X 10.2和更新版本：/etc/hosts（指向/private/etc/hosts的符号链接）

+ Unix、类Unix系统（例如Linux等）：/etc/hosts

+ Windows Mobile、Windows Phone：注册表项HKEY_LOCAL_MACHINE\Comm\Tcpip\Hosts

+ Symbian OS 6.1–9.0：C:\system\data\hosts

+ Symbian OS 9.1+：C:\private\10000882\hosts


## 如何使用？

1. + 粘贴到对应目录下，替换原来的hosts（最好备份原来的hosts） 

2.  + Windows：使用快捷键 `win + r` 打开运行窗口，然后输入 `cmd`, 回车, 输入：`ipconfig /flushdns`, 回车, 即可刷新hosts文件
    + Mac： 使用 Root 权限：`sudo vi /etc/hosts` 编辑hosts, 然后  `sudo killall -HUP mDNSResponder`
    + Linux: 使用 Root 权限：`sudo vi /etc/hosts` 编辑hosts, 然后  `sudo rcnscd restart`
    + 其他平台, 暂无测试。

