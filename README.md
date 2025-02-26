# 关于

本项目克隆自[cabins](https://github.com/cabins/emacs.d),其说明文档见[原项目文档](cabins-emacs.md)

本项目目前以自用为主，重点保证中文工作环境和中国大陆互联网环境下的正常使用。

# 项目的功能改动

本项目创建于 2024年2月1日，未来将持续更新。

## 已有功能

### emacs内置


### 新增且通过测试



## 新增的功能(包括调试中)
原项目较为简洁，我在其基础上增加了如下功能
- AucTeX的相关配置
  - 将XeLaTeX设为默认的编译器
- Org mode的相关配置
  - 增加了公式的渲染
  - 增加了图片的渲染，且控制图片显示的宽度
  - 将org mode导出pdf时默认的编译器为XeLaTeX，减少了编译中文文档时的障碍
- NeoTree
  - 主题：尝试all-the-icons,但相关的素材文件过于庞大，展示搁置
  - 绑定快捷键F8
- pdf-tools插件的配置
  - [ ] TODO 安装之后出现了到emacs启动时闪退的问题，暂时搁置
- ivy的插件
  - 关于该插件的配置，需要进一步了解
    - ivy-counsel
    - ivy-rich
- 美化工作
  - 主界面设置
    - 字体位置，Nerd字体，支持图标
    - 高亮显示
    - 光标的定位
  - mode-line主题安装：采用了doom-modeline
  - 主题设置：设置了默认主题，同时保留了原像所设有的dark-theme和light-theme

## 计划改进的功能
- [ ] 调整配置文件的组织架构，将类似的功能存入一个init-*.el文件中，由init.el调用，增强配置文件的可读性
- [ ] 设置emacs与系统的阅读器等软件的调用关系
  - [ ] pdf阅读器
- [ ] 增强对window系统的支持
  - [ ] 网络问题
  - [ ] 字体支持
  

## emacs的性能优化

随着配置增加，emacs的性能会受到一定的影响，未来将着手对emacs的性能进行优化。


# 安装

1. 运行如下命令:

```bash
git clone https://github.com/PeakHan618/start.emacs.d ~/.emacs.d

```

2. 启动emacs, 等待安装。
   1. 在windws中，安装路径可能有所不同，请查看自己的emacs实际安装路径再进行配置。
   2. 需要注意，中国大陆地区可能会因为某些客观原因，在项目克隆和插件安装的过程中需要通过VPN来解决。
   3. 在项目的init.el中提供有清华大学镜像源的链接，如需要可将其设置为插件安装源。
3. Happy Hacking!

