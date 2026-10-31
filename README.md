# furrypkgs — CloudFurry Linux 官方软件源

由 **fpt** 包管理器（CloudFurry Linux 内置）完全以 git 仓库方式下载：

```
fpt update            # git clone/fetch 本仓库
fpt list              # 列出 packages/ 下全部包
fpt install <pkg>     # 安装
```

仓库布局（与 deep-repo 兼容）:

```
packages/<name>/description   包描述
packages/<name>/version       版本
packages/<name>/files/...     安装载荷（相对 / 复制到目标系统；
                              无 files/ 时安装包目录内可执行文件到 /usr/bin）
```
