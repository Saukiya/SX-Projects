---
sidebar_position: 1
---

# SX-Item Wiki

SX-Item是Spigot服务器的物品插件, 为服务器提供物品管理功能, 这些功能包括:

- 配置任何物品
- 高度自定义的表达式功能
- 可控的自动更新
- 查看并编辑 NBT/Components 数据
- 主流版本支持以及新版本支持

## 入门

请确保你运行的是主流的服务器平台, 比如 `Paper`|`Spigot`. 根据统计, 还有存在`CatServer`|`Arclight`|`Mohist`|`Purper`
的平台在使用此插件.

### 支持版本

| Version | ------ | ------ | ------ | ------ | ------ |
|:-------:|:------:|:------:|:------:|:------:|:------:|
|  1.8.8  | 1.11.2 | 1.12.2 | 1.13.2 | 1.14.4 | 1.15.2 |
| 1.16.5  | 1.17.1 | 1.18.2 | 1.19.2 | 1.19.4 | 1.20.1 |
| 1.20.2  | 1.20.3 | 1.20.4 | 1.21.1 | 1.21.3 |

### 下载插件

- [SpigotMC](https://www.spigotmc.org/resources/sx-item-%E2%AD%90-random-expression-update-1-8-8-1-21-3.119751/)
- [GitHub Release](https://github.com/Saukiya/SX-Item/releases/latest)

下载后移动到目录`plugins`中, 启动服务器. 执行 `/si give Default-1` 大功告成!

### 目录结构

插件的配置会解压到`plugins/SX-Item`文件夹中, 具体如下:

- `Item/` - 物品配置目录
- `RandomString/` - 随机字符串目录
- `Scripts/` - 脚本目录
- `log/` - 日志目录
- `Config.yml` - 配置文件
- `Message.yml` - 消息文件

### 联动功能

插件还支持通过部分插件, 实现额外的功能, 当然这不是必要的:

- `MythicMobs` - 可以配置怪物的掉落/穿戴
- `PlaceHolderAPI` - 可以在物品配置中调用`papi`变量

### 扩展插件

使用下列插件, 可以实现一些额外功能:

- `没写出来`