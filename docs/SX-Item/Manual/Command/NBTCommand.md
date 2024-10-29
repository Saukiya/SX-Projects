---
sidebar_position: 4
---

# NBT 指令

#### 显示, 修改或删除`NBT`

用来查阅物品的NBT数据, 以及修改或删除NBT

### 格式

- `/si nbt <set/remove> <key> <value>`

### 参数

- `set/remove` - 需要执行的操作, 默认`all`
  - `set` 是设置, `remove` 是删除, `all` 是查看
- `key` - 需要操作的NBT路径
- `value` - 需要修改的NBT数值 \(`set`操作下使用\)

### 示例

玩家:

- `/si nbt` - 查看手持物品的NBT标签
- `/si nbt set SXItem.ItemKey Default-1` - 设置手持物品的指定NBT
- `/si nbt remove SXItem` - 移除手持物品的指定NBT

控制台:

- `/si nbt Default-1` - 查看`Default-1`的NBT标签
- `/si nbt Default-1 player` - 查看`Default-1`的NBT标签 (通过`player`生成)