# TP78FOC_智能旋钮键盘扩展模块

> 来源：[立创开源硬件平台](https://oshwhub.com/chnmasterog/tp78_foc_-zhi-neng-xuan-niu-jian-pan-kuo-zhan-mo-kuai)

![封面图](https://image.lceda.cn/oshwhub/19e5865af7e7494297f14161af81ea28.png)

## 简介

一个 FOC（Field-Oriented Control，磁场定向控制）控制无刷电机旋钮小键盘扩展模块，支持作为 TP78 从模块使用。具有以下功能：

- VIA 改键
- USB 模式下神光（Lighting）同步
- 音量控制
- Surface Dial 控制
- 番茄钟
- 自由键鼠快捷键组合键映射

支持作为 TP78 从模块使用，与 TP78 同步灯效、睡眠唤醒。固件升级方面支持 USB 在线升级。

**演示视频**：[https://www.bilibili.com/video/BV1jVpneNEpq/](https://www.bilibili.com/video/BV1jVpneNEpq/)

![作为TP78从模块使用](https://image.lceda.cn/oshwhub/c5a7dc2c7fd84d26bad137ca93e4b57a.png)

![商品图（白色背景）](https://image.lceda.cn/oshwhub/cf9809747c534b7a9b95ef248e5a5bb7.png)

## 硬件兼容性

硬件兼容**磁轴**和**机械轴**两种轴体。

![磁轴示例](https://image.lceda.cn/oshwhub/fc4097af87a445d0841e647127a77f7a.png)

![机械轴示例](https://image.lceda.cn/oshwhub/958df23292ad4b0597786737f7425a3d.png)

## 材料清单

### 1. 五金件

| 名称 | 数目 |
| --- | --- |
| 滚花螺母 M2 × 3 × 3 | 12 |
| 螺丝 M2 × 7 | 2 |
| 螺丝 M2 × 5 | 4 |
| 螺丝 M2 × 3 | 8 |
| 螺丝 M2 × 12 | 5 |

### 2. 排线

| 名称 | 数目 |
| --- | --- |
| 0.5mm 间距 FPC 排线反向 6cm 4p | 2 |
| 0.5mm 间距 FPC 排线反向 10cm 12p | 1 |
| 1.25mm 10p 反向排线 | 1 |

### 3. 其他焊接元件

| 名称 | 数目 | 购买链接 |
| --- | --- | --- |
| 磁吸连接器 4p 2.54 间距（公+母） | 1 | - |
| 应变片 BF120-3AA | 4 | [淘宝](https://m.tb.cn/h.gOxxHMXD9mmKU2Z?tk=Nbgi34SweAL) |
| OK 线 | 1 | - |

### 4. 非焊接零件

| 名称 | 数目 | 购买链接 |
| --- | --- | --- |
| 1.28 寸圆形 LCD 屏幕 | 1 | - |
| 800mAh 锂电池 PH2.0 正向接口 | 1 | - |
| 8mm × 1mm 圆形脚垫 | 4 | - |
| 亚克力手工胶 | 1 | - |
| 502 胶水 | 1 | - |
| 双面胶 | 1 | - |

## 成品/半成品购买

淘宝链接：[https://item.taobao.com/item.htm?id=828180761483](https://item.taobao.com/item.htm?id=828180761483)

## 3D 模型开源地址

[https://makerworld.com/zh/models/604167](https://makerworld.com/zh/models/604167)

## 安装步骤

### 1. 焊接核心板 PCB

![核心板 PCB](https://image.lceda.cn/oshwhub/24216bb21b3e4a1f9841005fe4cae252.png)

焊接完成图片：

![核心板焊接完成](https://image.lceda.cn/oshwhub/513b4d532b0f4e3f81fbcb81e5eda22a.png)

**注意**：
- 记住 OK 线颜色顺序，从左到右分别对应：**VCC / BLK / DC / SCL / SDA / RES / GND**
- 焊接磁编码器时，**丝印白色圆圈和芯片的圆圈应该是一个方向**，请仔细观察焊接完成图片，避免焊错导致烧坏磁编码器（进口芯片价格很贵）！！！

### 2. 沉入滚花螺母

红圈部分需要烫入 M2 × 3 × 3 滚花螺母。

![滚花螺母位置 1](https://image.lceda.cn/oshwhub/cc11fbcc7dc341b5aeba88c3aaa52680.png)

![滚花螺母位置 2](https://image.lceda.cn/oshwhub/53607d4abfdb4d9ea5e62503e047d3a2.png)

### 3. 安装电机

将电机与核心板用 LCD 支撑底座打印件连接，抽出 7 根 OK 线，并将电机排线插入 PCB 顶面端子中，最后使用 3 个 M2 × 12 的螺丝旋紧背面。

![电机安装](https://image.lceda.cn/oshwhub/69157c2d902348e7b241083fd3739e71.png)

### 4. 安装轴体板

将轴体和键帽安装好，并装好定位板硅胶粒。

![轴体板安装](https://image.lceda.cn/oshwhub/90557d10bee54fdf8c9b4a047e67c722.png)

### 5. 安装底座

- 先使用 4 个 M2 × 3 的螺丝安装左右侧磁吸小板，然后将核心板的排线都接好；
- 使用 4p FPC 排线连接左右侧磁吸，**保证靠近开关侧的位置为 5V**，最后锁紧周围 4 个螺丝；
- 之后将安装好电机的核心板用 4 个 M2 × 3 的螺丝固定；
- 使用 1.25mm 反向 10p 排线连接供电板和核心板；
- 使用 FPC 12p 反向线连接轴体板和核心板；
- 将电池用双面胶和底盖粘住，再连接电池和供电板。

![底座安装](https://image.lceda.cn/oshwhub/2dfb1fc88e0543158cdb46f31555f78f.png)

此时装好的模型如下图：

![底座安装完成](https://image.lceda.cn/oshwhub/d3775efa7ae842cba25cbed05f34003f.png)

### 6. 安装上盖

- 用 2 个 M2 × 7 螺丝旋紧供电板侧的孔洞；
- 用 2 个 M2 × 12 螺丝旋紧剩余 2 个孔洞。

### 7. 安装旋钮外壳下侧

使用 4 个 M2 × 5 螺丝旋紧 3D 打印件和电机。

![旋钮外壳下侧安装](https://image.lceda.cn/oshwhub/831c812eb64f4a0191e7347436088211.png)

### 8. 安装 LCD 支撑上平面

保证该位置需要卡紧，若很容易脱落建议使用 502 胶辅助粘牢。

![LCD 支撑上平面](https://image.lceda.cn/oshwhub/494d905b53ff4a72b0e89a99fe5582af.png)

### 9. 安装 LCD 面板

- 将 LCD 和 LCD 转接板连接好；
- 之后焊好 LCD 转接板和 7 根 OK 线，根据之前记得顺序和 PCB 对应丝印进行焊接；
- 之后将 LCD 转接板放在 LCD 支撑上平面的位置，使用适量 502 胶水进行固定；

![LCD 面板安装](https://image.lceda.cn/oshwhub/4502a1d22e4a4e83a6b04329d94926cb.png)

- 最后将 LCD 屏幕和 LCD 面板使用双面胶粘好，**这里需要保证 LCD 是正着，注意不要贴歪**。

### 10. 最后的组装

盖上旋钮上盖，使用**亚克力手工胶**将圆形亚克力和旋钮上盖固定。最后安装脚垫。

![最终成品](https://image.lceda.cn/oshwhub/ccac85687fd348ddb4017bc4641d82ec.png)

## 重要注意事项

> 本模块是**旋钮模块**，**非电机模块**，因此：
> - **不建议高速旋转**
> - **不建议在限位模式下强行转动电机**

**首次上电**需要执行：
- 电机校准
- 按键编码重置
- 屏幕校准
- 压力校准

具体参考指导文档文档部分。
