# 让包上挂件晚一拍停下

2026-11-24

人物快步走到门口停住。包身停稳时，松垂的挂件还会沿着人物刚才的行进方向摆出去，回摆后才垂直落下。画这个动作时，先确认包身的停点，再安排挂件到达摆动顶点的时刻。

Toon Boom 的动画原则文档用衣物和附属部分解释主动作结束后的延迟。动画师 Anthony Wong 在 Animation Mentor 的摆动示范中先排基座的位置和速度，再把链节的摆动顶点排在基座停下或变向之后。他也示范了怎样用偏移和幅度调整，让链条各处依次到位。这里把方法用在只有一个吊点的短挂件上。 [Toon Boom 官方文档](https://helpcentre.toonboom.com/hc/en-ca/articles/57087608774931-About-the-12-Principles-of-Animation) · [Anthony Wong 的示范与讲解](https://www.animationmentor.com/blog/tutorial-overlap-pendulum-motion-animation/)

## 先定包身，再画挂件

1. 在包口或缝线上选一个看得见的挂点。先排人物和包身的动作，标出挂点最后一次移动的位置。减速时可以先检查包身在相邻帧之间走了多少。 [用逐帧位置的间距画出减速停下](spacing-for-a-decelerating-stop.md)
2. 画挂件落后、越过悬垂线、反向回摆、静止的几个姿势。以挂点为圆心检查弧线。短挂件的摆幅可以很小。它碰到包身或被衣袖挡住时，顺着接触面调整后续路径。
3. 画连续漫画时，可从减速、包身停稳后挂件仍朝前、两者都静止这三个时刻取格。前后两格保留同一处包扣或缝线，读者可以沿包扣辨认变化发生在哪个部位。
4. 用生成工具时，先给同一张包身画稿和几个关键姿势。做动画时可以复用包身层，单独调整挂件。逐格回看挂点有没有在缝线上滑动，摆动幅度有没有逐次收小。

## 固定机位的两段试片

自画侧面的帆布包和短挂件，做成两段各 20 帧的试片，相邻帧的间隔为 80 ms，结尾另作停留。两段共用包身的所有画面。包朝右移动，停住的时刻记为第 0 帧，挂点此后固定在画面的 (135, 82)。挂点到挂件末端保持 42 px。朝右的摆角记为正数。

| 相对帧 | 包身 | A 同时停 | B 继续摆 |
| --- | --- | ---: | ---: |
| −1 | 减速 | −15° | −15° |
| 0 | 停住 | 0° | −7° |
| +3 | 位置固定 | 0° | +24° |
| +9 | 位置固定 | 0° | −12° |
| +16 | 位置固定 | 0° | 0° |

逐帧比较包身图层，两版的 20 帧逐像素一致。A 的挂件在第 0 帧垂下，之后保持原位。B 的挂件晚 3 帧到达前摆顶点，末端在挂点右侧约 17.1 px，反摆到另一侧时约为 8.7 px。最后一帧两版画面一致。角度和间隔是这两段试片的取值，可以按物件长度、碰撞和镜头节奏重排。

## 资料

- Toon Boom Help Centre，*About the 12 Principles of Animation*，Follow Through and Overlapping Action 与 Arcs 小节（2026-11-24 查阅）。 [官方文档](https://helpcentre.toonboom.com/hc/en-ca/articles/57087608774931-About-the-12-Principles-of-Animation)
- Anthony Wong 在 Animation Mentor 的 *Tutorial: Overlap and Pendulum Motion in Animation*（2026-11-24 查阅）。 [示范与讲解](https://www.animationmentor.com/blog/tutorial-overlap-pendulum-motion-animation/)
