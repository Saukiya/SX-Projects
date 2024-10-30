---
sidebar_position: 6
---

# Script 指令

#### 调用脚本指令 [脚本启用时生效]

用来查阅物品的NBT数据, 以及修改或删除NBT

### 格式

- `/si script [file] [func] <args>`

### 参数

- `file` - 执行脚本文件名
- `func` - 执行脚本方法
- `args` - 执行脚本参数

### 示例

- `/si script Default testPlayer player Hello` - 调用 `Default` 的 `testPlayer` 方法, 并携带`player` `Hello` 参数