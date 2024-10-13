<div align="center">


<h1>QAvatar</h1>
<h2>自动更换QQ头像</h2>

<div align="center">


  [![Stars](https://img.shields.io/github/stars/Nooniebao/qavatar?label=stars)](https://github.com/Nooniebao/qavatar)
  [![LSP%20Repo](https://img.shields.io/github/downloads/Xposed-Modules-Repo/icu.insomnia.qavatar/total?label=LSP%20Repo&labelColor=F48FB1)](https://github.com/Xposed-Modules-Repo/icu.insomnia.qavatar/releases)
</div>

[![Release](https://img.shields.io/github/v/release/Xposed-Modules-Repo/icu.insomnia.qavatar)](https://github.com/Xposed-Modules-Repo/icu.insomnia.qavatar/releases/latest)

</div>


## 重要信息

**请手动设置url为`https://avatar.corosy.com/`**


## 功能：

- QAvatar**始终**从指定文件夹自动上传`nextTick.jpg`作为QQ头像，你可以手动移入**1:1 jpg**到此目录

  `/storage/emulated/0/Android/data/com.tencent.mobileqq/files/qavatar/`

- QAvatar always try to rename a img in the Dir to `nextTick.jpg` randomly，And rename the used as `timespam-Used.jpg`

- 支持从指定URL下载图片到上述目录（URL如 ~~https://avatar.insomnia.icu/~~ (已变更为https://avatar.corosy.com/ )）

- **如果你选择手动移入1:1 jpg，请确保移动后的文件具有正确的权限。如660**



## 初始化：

- 见`QQ设置首页`或`QQ账号管理`
- <img src="https://github.com/Xposed-Modules-Repo/icu.insomnia.qavatar/blob/main/img/161ff7eff5c18faaee576a6ac07f5bed.jpg?raw=true" alt="img" style="zoom:67%;" />


## 触发条件
1. QAvatar并未设置定时器，HOOK入口点为`android.app.Application#attach`，因此，只有在重启QQ或QQ加载其内部某些组件的时，才会触发上传行为
2. 你可以通过调整冷却时间来调节上传频率


## 测试列表：

| phone        | API        | os              | Q_version          |
| ------------ | ---------- | --------------- | ------------------ |
| Mi 10 Ultra  | Android 11  | MIUI12.5 12.5.10 | QQ9.1.0           |
| Mi 10 Ultra  | Android 11  | MIUI12.5 12.5.10 | QQ8.9.68           |
| K40 pro      | Android 11  | MIUI12.5 12.5.8 | QQ8.9.68           |
| Xiaomi Note3 | Android 11 | crDroid 7.21    | QQ9.0.17 \ QQ8.6.0 |
| MI 6         | Android 9  | MIUI10 9.9.3    | QQ8.9.71           |

在上述设备上测试通过



## 源代码

[仓库](https://github.com/NoonieBao/QAvatar)已公开，欢迎反馈🚀

**如果你喜欢这个项目，就请移步[仓库](https://github.com/NoonieBao/QAvatar)为我点个star吧**🥰
