### 给予物品指令

#### 格式

- `/si give [item] <player> <count> <key:value...>`

#### 参数
- `item` 需要获取的 物品ID
- `player` 需要给与的 玩家ID
- `count` 给与物品的次数
- `key:value` 指定键 `key` 值 `value` , 将在 `<s:key>` 和 `<l:key>` 中生效

#### 使用例子

- `/si give`
    - 查看物品列表

- `/si give Def`
    - 查看包含 `Def` 的物品列表

- `/si give Default-1`
    - 给与 自己 `1` 个 `Default-1` 物品

- `/si give Default-1 player 5`
    - 给与 `player` `5` 个 `Default-1` 物品

- `/si give Default-1 player 5 key1:value1`
    - 给与 `player` `5` 个 `Default-1` 物品, 并指定变量 `key1` 的结果为 `value1`

- `/si give 267`