# 杯口和杯底分别定椭圆开度

2026-11-24 · 查阅画师的圆柱练习和针孔投影说明，并做了两张直筒杯对照。

用水平机位画摆正的直筒杯，若杯口和杯底都在眼平线下方，杯底离眼平线更远，椭圆在上下方向更展开。判断时把开度看成椭圆的高与宽之比，便于把轮廓大小和圆面的朝向分开检查。

Proko 的圆柱练习用不同观察角度说明圆面怎样从接近一条线到接近圆。Brent Eviston 示范画咖啡杯时，在草稿上把被遮住的杯底也补成一整圈，用完整的椭圆检查露出来的那段弧线。 [Proko · Assignment – Cylinders and Ellipses](https://www.proko.com/course-lesson/assignment-cylinders-and-ellipses) · [Brent Eviston · Form & Space / 3D Drawing & Perspective](https://www.skillshare.com/en/classes/form-and-space-3d-drawing-and-perspective/321249278)

## 落笔方法

1. 先定眼平线、杯身中轴和上下端的位置。这个练习使用等径直筒杯，杯口和杯底的左右切点落在同一对竖线上。杯身有收口时，按两端的实际直径分别起形。 [定眼平线的练习](eye-level-and-figure-scale.md)
2. 分别画两条完整椭圆。水平机位里，与眼睛等高的水平圆面投影成横线。圆面在眼平线下方时，离眼平线更远的一端在上下方向更展开。两端都在眼平线上方时，沿用离线远近的判断。
3. 留下杯底靠下的可见弧线，让弧线顺着杯壁两侧转过去。用轻线保留背面的弧度做结构校对，出稿时擦掉被遮住的一段。整理生成图时，可以叠这两条结构线检查，杯口校对无误后再局部修整底部。

## 同一只杯子的对照

小样用水平针孔相机。相机到杯轴的前向距离为 4.30 个场景单位，圆面半径为 0.80，焦距为 330 像素。杯口和杯底分别位于眼平线下 0.60 和 1.70 个场景单位。每个圆取 7,200 点，对各点用横纵坐标除以前向深度并乘以焦距，计算画面上包围框的宽与高。 [Scratchapixel · Implementing a Virtual Pinhole Camera](https://www.scratchapixel.com/lessons/3d-basic-rendering/3d-viewing-pinhole-camera/implementing-virtual-pinhole-camera.html)

| 对照 | 杯口的宽 × 高 | 杯底的宽 × 高 | 两处开度 |
| --- | ---: | ---: | ---: |
| A · 杯底沿用杯口的开度 | 124.97 × 17.75 px | 124.97 × 17.75 px | 0.142 / 0.142 |
| B · 各自按高度投影 | 124.97 × 17.75 px | 124.97 × 50.29 px | 0.142 / 0.402 |

两张图共用杯口、杯身切点和杯底中心。B 的杯底椭圆高出约 32.54 像素，露出的轮廓也更弯。换成俯仰镜头或倾斜的杯子时，按新机位和杯身朝向重画两个圆面。
