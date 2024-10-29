---
sidebar_position: 5
---

# Component 指令 [1.21+]

#### 显示, 修改或删除`Component`

用来查阅物品的NBT数据, 以及修改或删除Component

### 格式

- `/si component <set/remove> <key> <value>`

### 参数

- `set/remove` - 需要执行的操作, 默认`all`
  - `set` 是设置, `remove` 是删除, `all` 是查看
- `key` - 需要操作的组件名称
- `value` - 需要修改的组件参数

### 示例

玩家:

- `/si component` - 查看手持物品的组件功能
- `/si component set minecraft:max_damage 233` - 设置手持物品的最大耐久值为233
- `/si component remove minecraft:max_damage` - 移除手持物品的最大耐久值设定

控制台:

- `/si component Default-1` - 查看`Default-1`的组件功能
- `/si component Default-1 player` - 查看`Default-1`的组件功能 \(通过`player`生成\)