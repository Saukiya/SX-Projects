---
sidebar_position: 3
---

# Save 指令

#### 根据格式保存物品

物品会被保存到`Item/Type-Default`或`Item/Type-Import`中

### 格式

- `/si save [item] <type>`

### 参数

- `item` - 需要保存的 物品名称
- `type` - 需要保存的 物品类型, 默认 `Default`
  - `Default` SX-Item的默认物品类型
  - `Import` 原版的保存方式, 保存完整的物品数据

### 示例

- `/si save Temp1` - 将手持物品保存为 `Default` 类型的 `Temp1` 物品
- `/si save Temp2 Import` - 将手持物品保存为 `Import` 类型的 `Temp2` 物品