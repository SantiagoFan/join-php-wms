## 通用进销存系统（简单版本）

## 计划功能

┌─库存管理
│  ├─入库管理
│  │  ├─采购入库
│  │  ├─采购退货出库
│  │  ├─盘盈入库
│  │  ├─
│  │  └─其他入库
│  ├─出库管理
│  │  ├─销售出库
│  │  ├─销售退货入库
│  │  ├─盘亏出库
│  │  └─其他出库
│  ├─库存调拨
│  ├─库存盘点
│  ├─实时库存
│  ├─库存报表
│  └─仓库管理

## 数据库表
Consume_Order 出库表
Purchase_Order 入库单
Inventory_Record 库存变化记录表（出入库详情）
Stocking 盘点记录
Stocking_Detail  盘点记录详情

# 使用方法
### 1.创建数据表：sql 脚本
### 2.拷贝模块
### 3.调用函数
创建进库单
```
// 销售出库
$purchase = Purchase_Order::create();//出库单
$purchase->add();//出库详情
$purchase->save()
```
