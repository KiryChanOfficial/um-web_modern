# 关于此仓库  

这并不是官方仓库  

目前官方仓库地址 [Unlock Music - Web Edition](https://github.com/ipid/unlock-music)  

你所看到的这个仓库是依照 **MIT License** 授权转载，代码与仓库管理者无关。  

---

# Unlock Music 音乐解锁  

- [x] 在浏览器中解锁加密的音乐文件。  
- [x] Unlock Music 项目是以学习和技术研究的初衷创建的，修改、再分发时请遵循[**MIT License**](https://mit-license.org/)。  
- [x] Unlock Music 的 CLI 版本可以在 [unlock-music/cli](https://git.unlock-music.dev/um/cli) 找到，大批量转换建议使用 CLI 版本。  
- [x] 我们新建了 Telegram 群组 [@unlock_music_chat](https://t.me/unlock_music_chat) ，欢迎加入！  
- [x] CI 自动构建已经部署，可以在 [UM-Packages](https://git.unlock-music.dev/um/-/packages/generic/web-build/) 下载  

# 支持的的格式  
- [x] QQ 音乐 (.qmc0/.qmc2/.qmc3/.qmcflac/.qmcogg/.tkm)  
- [x] Moo 音乐格式 (.bkcmp3/.bkcflac/...)  
- [x] QQ 音乐 Tm 格式 (.tm0/.tm2/.tm3/.tm6)  
- [x] QQ 音乐新格式 (.mflac/.mgg/.mflac0/.mgg1/.mggl)  
- [x] QQ 音乐海外版JOOX Music (.ofl_en)  
- [x] 网易云音乐格式 (.ncm)  
- [x] 虾米音乐格式 (.xm)  
- [x] 酷我音乐格式 (.kwm)  
- [x] 酷狗音乐格式 (.kgm/.vpr)  
- [x] Android版喜马拉雅文件格式 (.x2m/.x3m)  
- [x] 咪咕音乐格式 (.mg3d)  

# 其他特性  
- [x] 在浏览器中解锁  
- [x] 拖放文件  
- [x] 批量解锁  
- [x] 渐进式 Web 应用 (PWA)  
- [x] 多线程  
- [x] 写入和编辑元信息与专辑封面  

# 使用方法  

## 使用预构建版本  
1. 从[Release](https://git.unlock-music.dev/um/web/releases/latest)或[CI构建](https://git.unlock-music.dev/um/-/packages/generic/web-build/)下载预构建的版本
> ⚠️ 本地使用请下载**legacy版本**（**modern版本**只能通过**http(s)协议**访问）  
2. 解压缩后即可部署或本地使用（请勿直接运行源代码）  

## 自行构建  
- 环境要求  
  - nodejs (v16.x)  
  - npm  

1. 获取项目源代码后安装相关依赖：  
```
npm install
npm ci
```

2. 然后进行构建：  
```
npm run build
```
  - 构建后的产物可以在 dist 目录找到。
  - 如果是用于开发，可以执行 npm run serve。
  - 如需构建浏览器扩展，构建成功后还需要执行：
```
npm run make-extension
```
