---
sidebar_position: 2
---

# Give 指令

#### 给予玩家指定数量

获取`plugins/SX-Item/Item`下的物品, 或者是原版物品

### 格式

- `/si give [item] <player> <count> <key:value...>`

### 参数

- `item` - 需要获取的物品名称
  - 也可以是数字ID `267` `260:3` - [物品数字ID列表](../../Other/ItemNumberID.md)
- `player` - 需要给与的玩家名称, 默认`自己`
- `count` - 给与物品的次数, 默认`1`
- `key:value` - 指定键 `key` 值 `value` , 将在 `<s:key>` 和 `<l:key>` 中生效
  - 可以使用表达式, 可以配置多个`k:v`, 使用空格隔开

### 示例

- `/si give` - 查看物品列表
- `/si give Def` - 查看包含 `Def` 的物品列表
- `/si give Default-1` - 给与 自己 `1` 个 `Default-1` 物品
- `/si give Default-1 player 5` - 给与 `player` `5` 个 `Default-1` 物品
- `/si give Default-1 player 5 k1:v1` - 给与 `player` `5` 个 `Default-1` 物品, 并指定变量 `k1` 的返回值为 `v1`
- `/si give 267` - 获取数字ID为 `267` 的物品 \(钻石剑\)