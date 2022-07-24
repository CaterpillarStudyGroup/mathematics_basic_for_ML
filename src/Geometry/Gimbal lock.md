# Gimbal lock 万向节死锁

![](图片/21.jpg)

>- "Phantom 4 Pro V2 Gimbal Holder" by Jordan Raychev  
Jordan Raychev 的 Phantom 4 Pro V2 万向支架

![](图片/22.png)

>- Adding a fourth rotational axis can solve the problem of gimbal lock, but it requires the outermost ring to be actively driven so that it stays 90 degrees out of alignment with the innermost axis (the flywheel shaft). Without active driving of the outermost ring, all four axes can become aligned in a plane as shown above, again leading to gimbal lock and inability to roll.  
添加第四个旋转轴可以解决万向死锁问题，但它需要主动驱动最外圈，使其与最内轴（飞轮轴）保持90度不对齐。 如果没有主动驱动最外环，所有四个轴都可以在一个平面上对齐，如上图所示，再次导致万向节死锁和无法滚动。

Gimbal lock is the loss of one degree of freedom in a three-dimensional, three-gimbal mechanism that occurs when the axes of two of the three gimbals are driven into a parallel configuration, "locking" the system into rotation in a degenerate two-dimensional space.

万向节死锁是三维、三万向节机构中一个自由度的损失，当三个万向节中的两个的轴被驱动成平行配置时，就会发生这种情况，将系统“死锁”成退化的两轴旋转维空间。

The word lock is misleading: no gimbal is restrained. All three gimbals can still rotate freely about their respective axes of suspension. Nevertheless, because of the parallel orientation of two of the gimbals' axes there is no gimbal available to accommodate rotation about one axis.

死锁一词具有误导性：没有万向节受到限制。 所有三个万向节仍然可以围绕各自的悬挂轴自由旋转。 然而，由于两个万向节轴的平行方向，没有万向节可用于容纳围绕一个轴的旋转。


Contents

1	Gimbals

2	In engineering

2.1	In two dimensions

2.2	In three dimensions

2.3	Solutions

2.4	On Apollo 11

2.5	Robotics

3	In applied mathematics

3.1	Loss of a degree of freedom with Euler angles

3.2	Alternate orientation representation

4	See also

5	References

6	External links

# Gimbals 万向节

Main article: Gimbal

主条目：万向节

A gimbal is a ring that is suspended so it can rotate about an axis. Gimbals are typically nested one within another to accommodate rotation about multiple axes.

万向节是一个悬挂的环，因此它可以绕轴旋转。 万向节通常嵌套在另一个中，以适应围绕多个轴的旋转。

They appear in gyroscopes and in inertial measurement units to allow the inner gimbal's orientation to remain fixed while the outer gimbal suspension assumes any orientation. In compasses and flywheel energy storage mechanisms they allow objects to remain upright. They are used to orient thrusters on rockets.[1]

它们出现在陀螺仪和惯性测量单元中，以允许内部万向节的方向保持固定，而外部万向节悬架采用任何方向。 在指南针和飞轮储能机制中，它们允许物体保持直立。 它们用于定位火箭上的推进器。 [1]

Some coordinate systems in mathematics behave as if there were real gimbals used to measure the angles, notably Euler angles.

数学中的一些坐标系表现得好像有用于测量角度的真实万向节，特别是欧拉角。

For cases of three or fewer nested gimbals, gimbal lock inevitably occurs at some point in the system due to properties of covering spaces (described below).

对于三个或更少的嵌套万向节的情况，由于覆盖空间的特性（如下所述），在系统中的某些点不可避免地会发生万向节死锁。

# In engineering 在工程

While only two specific orientations produce exact gimbal lock, practical mechanical gimbals encounter difficulties near those orientations. When a set of gimbals is close to the locked configuration, small rotations of the gimbal platform require large motions of the surrounding gimbals. Although the ratio is infinite only at the point of gimbal lock, the practical speed and acceleration limits of the gimbals—due to inertia (resulting from the mass of each gimbal ring), bearing friction, the flow resistance of air or other fluid surrounding the gimbals (if they are not in a vacuum), and other physical and engineering factors—limit the motion of the platform close to that point.

虽然只有两个特定的方向可以产生精确的万向节死锁，但实际的机械万向节在这些方向附近会遇到困难。 当一组万向节接近死锁配置时，万向节平台的小旋转需要周围万向节的较大运动。 尽管该比率仅在万向节死锁点是无限的，但由于惯性（由每个万向节环的质量引起）、轴承摩擦、空气或其他流体周围的流动阻力，万向节的实际速度和加速度限制 万向节（如果它们不在真空中）以及其他物理和工程因素 - 将平台的运动限制在该点附近。

## In two dimensions 在二维
 
Gimbal lock can occur in gimbal systems with two degrees of freedom such as a theodolite with rotations about an azimuth and elevation in two dimensions. These systems can gimbal lock at zenith and nadir, because at those points azimuth is not well-defined, and rotation in the azimuth direction does not change the direction the theodolite is pointing.

万向节死锁可能发生在具有两个自由度的万向节系统中，例如具有围绕方位角和二维仰角旋转的经纬仪。 这些系统可以在天顶和天底死锁万向节，因为在这些点方位角没有明确定义，并且在方位角方向上的旋转不会改变经纬仪指向的方向。

Consider tracking a helicopter flying towards the theodolite from the horizon. The theodolite is a telescope mounted on a tripod so that it can move in azimuth and elevation to track the helicopter. The helicopter flies towards the theodolite and is tracked by the telescope in elevation and azimuth. The helicopter flies immediately above the tripod (i.e. it is at zenith) when it changes direction and flies at 90 degrees to its previous course. The telescope cannot track this maneuver without a discontinuous jump in one or both of the gimbal orientations. There is no continuous motion that allows it to follow the target. It is in gimbal lock. So there is an infinity of directions around zenith for which the telescope cannot continuously track all movements of a target.[2] Note that even if the helicopter does not pass through zenith, but only near zenith, so that gimbal lock does not occur, the system must still move exceptionally rapidly to track it, as it rapidly passes from one bearing to the other. The closer to zenith the nearest point is, the faster this must be done, and if it actually goes through zenith, the limit of these "increasingly rapid" movements becomes infinitely fast, namely discontinuous.

考虑跟踪一架直升机从地平线飞向经纬仪。经纬仪是安装在三脚架上的望远镜，它可以在方位角和仰角上移动以跟踪直升机。直升机飞向经纬仪，并由望远镜在仰角和方位角上进行跟踪。当直升机改变方向并以 90 度角飞行到之前的航线时，它会立即飞到三脚架上方（即它位于天顶）。如果没有在一个或两个万向节方向上的不连续跳跃，望远镜就无法跟踪这个机动。没有允许它跟随目标的连续运动。它在万向节死锁中。因此，天顶周围有无限的方向，望远镜无法连续跟踪目标的所有运动。 [2]请注意，即使直升机没有通过天顶，而只是靠近天顶，因此不会发生万向架死锁，系统仍必须非常快速地移动以跟踪它，因为它从一个轴承快速移动到另一个轴承。离天顶最近的点越接近天顶，必须越快，如果真的经过天顶，这些“越来越快”的运动的极限就变得无限快，即不连续。

To recover from gimbal lock the user has to go around the zenith – explicitly: reduce the elevation, change the azimuth to match the azimuth of the target, then change the elevation to match the target.

要从万向节死锁中恢复，用户必须绕过天顶 - 明确：降低仰角，更改方位角以匹配目标的方位角，然后更改仰角以匹配目标。

Mathematically, this corresponds to the fact that spherical coordinates do not define a coordinate chart on the sphere at zenith and nadir. Alternatively, the corresponding map T2→S2 from the torus T2 to the sphere S2 (given by the point with given azimuth and elevation) is not a covering map at these points.

在数学上，这对应于球坐标没有在天顶和最低点定义球体坐标图的事实。 或者，从圆环 T2 到球体 S2 的对应图 T2→S2（由具有给定方位角和仰角的点给出）不是这些点的覆盖图。

## In three dimensions 在三维

![](图片/23.gif)

>- Gimbal with 3 axes of rotation. A set of three gimbals mounted together to allow three degrees of freedom: roll, pitch and yaw. When two gimbals rotate around the same axis, the system loses one degree of freedom.  
具有 3 个旋转轴的万向节。 一组三个安装在一起的万向节允许三个自由度：滚动、俯仰和偏航。 当两个万向节绕同一轴旋转时，系统失去一个自由度。

![](图片/24.png)

>- Normal situation: the three gimbals are independent  
正常情况：三个万向节独立

![](图片/25.png)

>- Gimbal lock: two out of the three gimbals are in the same plane, one degree of freedom is lost  
万向节死锁：三个万向节中有两个在同一平面，失去一个自由度

Consider a case of a level-sensing platform on an aircraft flying due north with its three gimbal axes mutually perpendicular (i.e., roll, pitch and yaw angles each zero). If the aircraft pitches up 90 degrees, the aircraft and platform's yaw axis gimbal becomes parallel to the roll axis gimbal, and changes about yaw can no longer be compensated for.

考虑一个水平传感平台的情况，飞机正北飞行，其三个万向节轴相互垂直（即横滚、俯仰和偏航角各为零）。 如果飞行器俯仰 90 度，飞行器和平台的偏航轴万向节与横滚轴万向节平行，偏航角的变化无法补偿。

## Solutions 解决方案

This problem may be overcome by use of a fourth gimbal, actively driven by a motor so as to maintain a large angle between roll and yaw gimbal axes. Another solution is to rotate one or more of the gimbals to an arbitrary position when gimbal lock is detected and thus reset the device.

这个问题可以通过使用第四个万向节来克服，该万向节由电机主动驱动，以保持滚动和偏航万向节轴之间的大角度。 另一种解决方案是当检测到万向节死锁时，将一个或多个万向节旋转到任意位置，从而重置设备。

Modern practice is to avoid the use of gimbals entirely. In the context of inertial navigation systems, that can be done by mounting the inertial sensors directly to the body of the vehicle (this is called a strapdown system)[3] and integrating sensed rotation and acceleration digitally using quaternion methods to derive vehicle orientation and velocity. Another way to replace gimbals is to use fluid bearings or a flotation chamber.[4]

现代做法是完全避免使用万向节。 在惯性导航系统的背景下，这可以通过将惯性传感器直接安装到车辆车身（这称为捷联系统）[3] 并使用四元数方法以数字方式集成感测到的旋转和加速度来获得车辆方向和速度。 更换万向节的另一种方法是使用流体轴承或浮选室。 [4]

## On Apollo 11 在阿波罗 11 号上

A well-known gimbal lock incident happened in the Apollo 11 Moon mission. On this spacecraft, a set of gimbals was used on an inertial measurement unit (IMU). The engineers were aware of the gimbal lock problem but had declined to use a fourth gimbal.[5] Some of the reasoning behind this decision is apparent from the following quote:

阿波罗 11 号登月任务中发生了著名的万向节死锁事件。 在这艘航天器上，惯性测量单元（IMU）上使用了一组万向节。 工程师们知道万向节死锁问题，但拒绝使用第四个万向节。 [5] 从以下引用中可以明显看出该决定背后的一些原因：

The advantages of the redundant gimbal seem to be outweighed by the equipment simplicity, size advantages, and corresponding implied reliability of the direct three degree of freedom unit.
— David Hoag, Apollo Lunar Surface Journal

冗余万向节的优势似乎被直接三自由度单元的设备简单性、尺寸优势和相应的隐含可靠性所抵消。
— David Hoag，阿波罗月球表面杂志

They preferred an alternate solution using an indicator that would be triggered when near to 85 degrees pitch.

他们更喜欢使用指示器的替代解决方案，该指示器将在接近 85 度俯仰角时触发。

Near that point, in a closed stabilization loop, the torque motors could theoretically be commanded to flip the gimbal 180 degrees instantaneously. Instead, in the LM, the computer flashed a 'gimbal lock' warning at 70 degrees and froze the IMU at 85 degrees
— Paul Fjeld, Apollo Lunar Surface Journal

在那一点附近，在一个封闭的稳定回路中，理论上可以命令扭矩马达将万向架瞬时翻转 180 度。 相反，在 LM 中，计算机在 70 度时闪烁“万向节死锁”警告，并将 IMU 冻结在 85 度
— Paul Fjeld，阿波罗月球表面杂志

Rather than try to drive the gimbals faster than they could go, the system simply gave up and froze the platform. From this point, the spacecraft would have to be manually moved away from the gimbal lock position, and the platform would have to be manually realigned using the stars as a reference.[6]

系统并没有试图以更快的速度驱动万向节，而是简单地放弃并冻结了平台。 从这一点开始，必须手动将航天器从万向节死锁位置移开，并且必须使用星星作为参考手动重新调整平台。 [6]

After the Lunar Module had landed, Mike Collins aboard the Command Module joked "How about sending me a fourth gimbal for Christmas?"

登月舱着陆后，指挥舱上的迈克·柯林斯开玩笑说：“圣诞节送我第四个万向节怎么样？”

## Robotics 机器人技术

![](图片/26.jpg)

>- Industrial robot operating in a foundry.  
在铸造厂工作的工业机器人。

In robotics, gimbal lock is commonly referred to as "wrist flip", due to the use of a "triple-roll wrist" in robotic arms, where three axes of the wrist, controlling yaw, pitch, and roll, all pass through a common point.

在机器人技术中，万向节死锁通常被称为“手腕翻转”，因为在机械臂中使用了“三滚腕”，其中手腕的三个轴，控制偏航，俯仰和滚动，都通过一个共同点。

An example of a wrist flip, also called a wrist singularity, is when the path through which the robot is traveling causes the first and third axes of the robot's wrist to line up. The second wrist axis then attempts to spin 180° in zero time to maintain the orientation of the end effector. The result of a singularity can be quite dramatic and can have adverse effects on the robot arm, the end effector, and the process.

手腕翻转的一个例子，也称为手腕奇点，是当机器人行进的路径导致机器人手腕的第一轴和第三轴对齐时。 然后，第二腕轴尝试在零时间内旋转 180°，以保持末端执行器的方向。 奇点的结果可能非常显着，并且可能对机器人手臂、末端执行器和过程产生不利影响。

The importance of avoiding singularities in robotics has led the American National Standard for Industrial Robots and Robot Systems – Safety Requirements to define it as "a condition caused by the collinear alignment of two or more robot axes resulting in unpredictable robot motion and velocities".[7]

避免机器人技术中的奇异性的重要性导致美国工业机器人和机器人系统国家标准 - 安全要求将其定义为“由两个或多个机器人轴共线对齐导致的机器人运动和速度不可预测的情况”。 7]

# In applied mathematics 在应用数学中

This section includes a list of references, related reading or external links, but its sources remain unclear because it lacks inline citations. Please help to improve this section by introducing more precise citations. (July 2013) (Learn how and when to remove this template message)

本节包括参考文献列表、相关阅读或外部链接，但由于缺少内联引文，其来源仍不清楚。 请通过引入更精确的引用来帮助改进本节。 （2013 年 7 月）（了解如何以及何时删除此模板消息）

The problem of gimbal lock appears when one uses Euler angles in applied mathematics; developers of 3D computer programs, such as 3D modeling, embedded navigation systems, and video games must take care to avoid it.

应用数学中使用欧拉角会出现万向节死锁问题； 3D 计算机程序（例如 3D 建模、嵌入式导航系统和视频游戏）的开发人员必须小心避免这种情况。

In formal language, gimbal lock occurs because the map from Euler angles to rotations (topologically, from the 3-torus T3 to the real projective space RP3 which is the same as the space of 3d rotations SO3) is not a local homeomorphism at every point, and thus at some points the rank (degrees of freedom) must drop below 3, at which point gimbal lock occurs. Euler angles provide a means for giving a numerical description of any rotation in three-dimensional space using three numbers, but not only is this description not unique, but there are some points where not every change in the target space (rotations) can be realized by a change in the source space (Euler angles). This is a topological constraint – there is no covering map from the 3-torus to the 3-dimensional real projective space; the only (non-trivial) covering map is from the 3-sphere, as in the use of quaternions.

在形式语言中，万向节死锁的发生是因为从欧拉角到旋转的映射（拓扑上，从 3-环 T3 到与 3d 旋转空间 SO3 相同的实投影空间 RP3）不是每个点的局部同胚 ，因此在某些点，等级（自由度）必须降至 3 以下，此时会发生万向节死锁。 欧拉角提供了一种使用三个数字对三维空间中的任何旋转进行数值描述的方法，但这种描述不仅不是唯一的，而且在某些点上并不是目标空间（旋转）的每一个变化都可以实现 通过源空间的变化（欧拉角）。 这是一个拓扑约束——没有从 3 环面到 3 维实射影空间的覆盖图； 唯一的（非平凡的）覆盖图来自 3 球体，就像使用四元数一样。

To make a comparison, all the translations can be described using three numbers ${\displaystyle x}$, ${\displaystyle y}$, and ${\displaystyle z}$, as the succession of three consecutive linear movements along three perpendicular axes ${\displaystyle X}$, ${\displaystyle Y}$ and ${\displaystyle Z}$ axes. The same holds true for rotations: all the rotations can be described using three numbers ${\displaystyle \alpha }$ , ${\displaystyle \beta }$, and ${\displaystyle \gamma }$ , as the succession of three rotational movements around three axes that are perpendicular one to the next. This similarity between linear coordinates and angular coordinates makes Euler angles very intuitive, but unfortunately they suffer from the gimbal lock problem.

为了进行比较，可以使用三个数字 ${\displaystyle x}$、${\displaystyle y}$ 和 ${\displaystyle z}$ 来描述所有平移，作为沿三个垂直方向的三个连续线性运动的连续 坐标轴 ${\displaystyle X}$、${\displaystyle Y}$ 和 ${\displaystyle Z}$ 坐标轴。 旋转也是如此：所有的旋转都可以用三个数字 ${\displaystyle \alpha }$ 、 ${\displaystyle \beta }$ 和 ${\displaystyle \gamma }$ 来描述，作为三个旋转的连续 围绕三个相互垂直的轴的运动。 线性坐标和角坐标之间的这种相似性使得欧拉角非常直观，但不幸的是它们遭受了万向节死锁问题。

## Loss of a degree of freedom with Euler angles 欧拉角的自由度损失

A rotation in 3D space can be represented numerically with matrices in several ways. One of these representations is:

3D 空间中的旋转可以通过多种方式用矩阵数字表示。 这些表示之一是：

$$
{\displaystyle {\begin{aligned}R&={\begin{bmatrix}1&0&0\\0&\cos \alpha &-\sin \alpha \\0&\sin \alpha &\cos \alpha \end{bmatrix}}{\begin{bmatrix}\cos \beta &0&\sin \beta \\0&1&0\\-\sin \beta &0&\cos \beta \end{bmatrix}}{\begin{bmatrix}\cos \gamma &-\sin \gamma &0\\\sin \gamma &\cos \gamma &0\\0&0&1\end{bmatrix}}\end{aligned}}}
$$

An example worth examining happens when ${\displaystyle \beta ={\tfrac {\pi }{2}}}$. Knowing that ${\displaystyle \cos {\tfrac {\pi }{2}}=0}$and ${\displaystyle \sin {\tfrac {\pi }{2}}=1}$, the above expression becomes equal to:

一个值得研究的例子发生在 ${\displaystyle \beta ={\tfrac {\pi }{2}}}$。 知道${\displaystyle \cos {\tfrac {\pi }{2}}=0}$和${\displaystyle \sin {\tfrac {\pi }{2}}=1}$，上述表达式变为 等于：

$$
{\displaystyle {\begin{aligned}R&={\begin{bmatrix}1&0&0\\0&\cos \alpha &-\sin \alpha \\0&\sin \alpha &\cos \alpha \end{bmatrix}}{\begin{bmatrix}0&0&1\\0&1&0\\-1&0&0\end{bmatrix}}{\begin{bmatrix}\cos \gamma &-\sin \gamma &0\\\sin \gamma &\cos \gamma &0\\0&0&1\end{bmatrix}}\end{aligned}}}
$$

Carrying out matrix multiplication:

执行矩阵乘法：

$$
{\displaystyle {\begin{aligned}R&={\begin{bmatrix}0&0&1\\\sin \alpha &\cos \alpha &0\\-\cos \alpha &\sin \alpha &0\end{bmatrix}}{\begin{bmatrix}\cos \gamma &-\sin \gamma &0\\\sin \gamma &\cos \gamma &0\\0&0&1\end{bmatrix}}&={\begin{bmatrix}0&0&1\\\sin \alpha \cos \gamma +\cos \alpha \sin \gamma &-\sin \alpha \sin \gamma +\cos \alpha \cos \gamma &0\\-\cos \alpha \cos \gamma +\sin \alpha \sin \gamma &\cos \alpha \sin \gamma +\sin \alpha \cos \gamma &0\end{bmatrix}}\end{aligned}}}
$$

And finally using the trigonometry formulas:

最后使用三角公式：

$$
{\displaystyle {\begin{aligned}R&={\begin{bmatrix}0&0&1\\\sin(\alpha +\gamma )&\cos(\alpha +\gamma )&0\\-\cos(\alpha +\gamma )&\sin(\alpha +\gamma )&0\end{bmatrix}}\end{aligned}}}
$$

Changing the values of ${\displaystyle \alpha }$ and ${\displaystyle \gamma }$  in the above matrix has the same effects: the rotation angle ${\displaystyle \alpha +\gamma }$  changes, but the rotation axis remains in the ${\displaystyle Z}$ direction: the last column and the first row in the matrix won't change. The only solution for ${\displaystyle \alpha }$  and ${\displaystyle \gamma }$ to recover different roles is to change ${\displaystyle \beta }$ .

改变上述矩阵中${\displaystyle \alpha }$和${\displaystyle \gamma }$的值具有相同的效果：旋转角度${\displaystyle \alpha +\gamma }$改变了，但是旋转轴 保持在 ${\displaystyle Z}$ 方向：矩阵中的最后一列和第一行不会改变。 ${\displaystyle \alpha }$ 和 ${\displaystyle \gamma }$ 恢复不同角色的唯一解决方案是更改 ${\displaystyle \beta }$ 。

It is possible to imagine an airplane rotated by the above-mentioned Euler angles using the X-Y-Z convention. In this case, the first angle - ${\displaystyle \alpha }$  is the pitch. Yaw is then set to ${\displaystyle {\tfrac {\pi }{2}}}$ and the final rotation - by ${\displaystyle \gamma }$  - is again the airplane's pitch. Because of gimbal lock, it has lost one of the degrees of freedom - in this case the ability to roll.

可以想象一架飞机使用 X-Y-Z 约定以上述欧拉角旋转。 在这种情况下，第一个角度 - ${\displaystyle \alpha }$ 是音高。 然后将偏航设置为 ${\displaystyle {\tfrac {\pi }{2}}}$，最后的旋转 - 通过 ${\displaystyle \gamma }$ - 再次是飞机的俯仰角。 由于万向节死锁，它失去了一个自由度——在这种情况下，它失去了滚动的能力。

It is also possible to choose another convention for representing a rotation with a matrix using Euler angles than the X-Y-Z convention above, and also choose other variation intervals for the angles, but in the end there is always at least one value for which a degree of freedom is lost.

除了上面的 X-Y-Z 约定，还可以选择使用欧拉角的矩阵表示旋转的另一种约定，也可以为角度选择其他变化区间，但最终总是至少有一个值的度数失去了自由。

The gimbal lock problem does not make Euler angles "invalid" (they always serve as a well-defined coordinate system), but it makes them unsuited for some practical applications.

万向节死锁问题不会使欧拉角“无效”（它们始终用作定义明确的坐标系），但它使它们不适合某些实际应用。

## Alternate orientation representation 交替方向表示

The cause of gimbal lock is the representation of orientation in calculations as three axial rotations based on Euler angles. A potential solution therefore is to represent the orientation in some other way. This could be as a rotation matrix, a quaternion (see quaternions and spatial rotation), or a similar orientation representation that treats the orientation as a value rather than three separate and related values. Given such a representation, the user stores the orientation as a value. To quantify angular changes produced by a transformation, the orientation change is expressed as a delta angle/axis rotation. The resulting orientation must be re-normalized to prevent the accumulation of floating-point error in successive transformations. For matrices, re-normalizing the result requires converting the matrix into its nearest orthonormal representation. For quaternions, re-normalization requires performing quaternion normalization.

万向节死锁的原因是计算中的方向表示为基于欧拉角的三个轴向旋转。 因此，一个潜在的解决方案是以其他方式表示方向。 这可以是旋转矩阵、四元数（参见四元数和空间旋转）或类似的方向表示，将方向视为一个值，而不是三个单独的相关值。 给定这样的表示，用户将方向存储为一个值。 为了量化变换产生的角度变化，方向变化表示为增量角度/轴旋转。 生成的方向必须重新归一化，以防止在连续转换中累积浮点误差。 对于矩阵，重新归一化结果需要将矩阵转换为其最接近的正交表示。 对于四元数，重新归一化需要执行四元数归一化。

# See also 参见

Charts on SO(3)

Flight dynamics

Grid north (equivalent navigational problem on polar expeditions)

Inertial navigation system

Motion planning

Quaternions and spatial rotation