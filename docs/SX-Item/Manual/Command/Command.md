---
sidebar_position: 1
---

# 指令

指令支持缩写执行, 例如 `/si give` 可以简化成 `/si g` `/si gi` `/si giv`

### 指令列表

注意: `[]`表示可以必须参数, `<>`表示可选参数

- `/si give [item] <player> <count> <key:value...>` - 给予玩家物品
- `/si save [item] <type>` - 保存当前的物品到配置文件
- `/si nbt <set/remove> <key> <value>` - 查看和修改物品NBT数据
- `/si component <set/remove> <key> <json>` - 查看和修改物品组件数据
- `/si script [file] [func] <args>` - 调用脚本函数
- `/si reload` - 重新加载这个插件的配置