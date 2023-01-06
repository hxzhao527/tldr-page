# 常用命令手册

## 背景
有一些命令的参数真记不住, 翻大部头的man手册又太麻烦.  
之前是找个地方记录下用的命令. 时间长了管理和查找不是很方便.

最近发现了一个有意思的工具 [tealdeer](https://github.com/dbrgn/tealdeer) 可以做这个活.  
它有一些来自社区的内置的常用命令, 也支持`Custom`和`Patch`.

这里记录记录一些自己常用的命令.

## 安装配置

```bash
cargo install tealdeer # 安装
curl -o ~/.antigen/bundles/zsh-users/zsh-completions/src/_tldr "https://raw.githubusercontent.com/dbrgn/tealdeer/main/completion/zsh_tealdeer" # 添加补全

tldr --show-paths | grep Custom | awk '{print $4}' | xargs mkdir -p
```

然后将repo内容放本地的page目录中
