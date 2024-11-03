---
sidebar_position: 2
---

# 物品配置

:heavy_check_mark: :x: :warning: :hourglass:

## 示例

```yaml <title="plugins/SX-Item/Item/Demo.yml"/>
Demo:
  Name: '&b慢剑'
  #  ID: 267
  ID:
    - 268
    - 272
    - 283
    - 267
    - 276
  #设置耐久为最大值*20%
  Durability: 20%
  Lore:
    - '&7很慢很慢的剑'
  Attributes:
    - "GENERIC_ATTACK_SPEED:-0.7:1:HAND"
    # - "GENERIC_ATTACK_SPEED:-1:2:HAND" # - 工具将无法抬起
  # 自定义材质ID
  CustomModelData: 1002
  Update: true
```

## 可选参数

| 字段名                         | 字段介绍            | 示例参数                                                 | [表达式](../Expression) |
|:----------------------------|:----------------|:-----------------------------------------------------|:--------------------:|
| [Name](#name)               | 名称              | `自定义的物品名称`                                           |  :heavy_check_mark:  |
| [ID](id)                    | 材质ID            | `APPLE` / `267`                                      |  :heavy_check_mark:  |
| [Durability](#durability)   | 耐久度             | `20` / `<20` / `20%`                                 |  :heavy_check_mark:  |
| [Amount](#amount)           | 数量              | `1` / `<i:1_5>`                                      |  :heavy_check_mark:  |
| [Lore](#lore)               | 描述              | - `多行文本1`<br/> - `多行文本2`                             |  :heavy_check_mark:  |
| [EnchantList](#enchantlist) | 附魔列表            | `附魔名称:等级` / `DURABILITY:1`                           |  :heavy_check_mark:  |
| ItemFlagList                | 隐藏选项            | `HIDE_ENCHANTS` / `HIDE_ATTRIBUTES`                  |         :x:          |
| Attributes                  | 原版属性            | `属性名:等级:模式:生效位置`<br/>`GENERIC_MAX_HEALTH:0.5:1:HAND` |  :heavy_check_mark:  |
| Unbreakable                 | 是否为无限耐久         | `true` / `false`                                     |  :heavy_check_mark:  |
| Potion                      | 药水效果            | 复杂类型                                                 |  :heavy_check_mark:  |
| SkullName                   | 玩家头颅的展示ID       | `Saukiya`<br/>`fha0cd1e-3ehb-4h01-aa95-d2f008908f49` |  :heavy_check_mark:  |
| Color                       | 皮革物品颜色          | `000000` / `FFFFFF`                                  |  :heavy_check_mark:  |
| CustomModelData             | 自定义材质ID         | `自定义材质ID` / `1000`                                   |         :x:          |
| ClearAttribute              | 清除默认属性          | `true` / `false`                                     |         :x:          |
| NBT                         | 自定义标签           | 复杂类型                                                 |  :heavy_check_mark:  |
| Components                  | 自定义组件 [1.21.1+] | 复杂类型                                                 |         :x:          |
| ProtectNBT                  | 保护NBT不被更新覆盖     | - `Enchantments`                                     |         :x:          |
| Update                      | 自动更新            | `true` / `false`                                     |         :x:          |
| Random                      | 局部随机            | 复杂类型                                                 |  :heavy_check_mark:  |

## 参数详情

- ### Name
  用来设置物品可变名称, 这个名称是可以被铁砧修改的
  ```yaml
  Demo:
    Name: '&c物品名称'
  ```

<br/>

- ### ID
  - 可以使一行或多行
  - 可以是英文ID, 也可以是[数字ID](../../Other/ItemNumberID.md)
  - 可以衔接子ID, 或者Durability `260:15` `DIAMOND_SWORD:20%`
  ```yaml
  Demo1:
    ID: 260:15
  Demo2:
    ID: 
    - 276:20%
    - DIAMOND_SWORD:20%
  ```

<br/>

- ### Durability
  物品耐久度, 总共有三种格式:
  - `20` 原版耐久，相当于 "物品少了20耐久度"
  - `<20` 反算耐久，相当于 "物品只有20耐久度"
  - `20%` 百分比耐久，相当于 "物品有20%的耐久度"
  ```yaml
  Demo1:
    Durability: 20 # 物品少了20耐久度
  Demo2:
    Durability: 20% # 物品有20%的耐久度
  ```

<br/>

- ### Amount
  物品数量, 单次使用 `/si give Demo` 时给予的数量
  ```yaml
  Demo:
    Amount: 20 # 一次给与20个
  ```

<br/>

- ### Lore
  物品描述, 如果配置错误, 需要注意双引号`"`和`'`的区别
  ```yaml
  Demo:
    Lore:
    - "&a物品描述第一行"
    - "&b物品描述第二行"
  ```

<br/>

- ### EnchantList
  附魔列表 -> [参考链接](https://minecraft.fandom.com/zh/wiki/%E9%99%84%E9%AD%94)
  ```yaml
  Demo:
    EnchantList:
    - "DURABILITY:1"
  ```

<br/>

- ### XXX
  XX
  ```yaml
  Demo:
    XXX:
  ```