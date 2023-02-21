<!--
 * @Author: 15868707168@163.com 15868707168@163.com
 * @Date: 2023-02-20 10:19:20
 * @LastEditors: 15868707168@163.com 15868707168@163.com
 * @LastEditTime: 2023-02-20 15:24:20
 * @FilePath: \UnityStudyNote\Animator And  Animation Clip.md
 * @Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
-->
##### 动画编辑器 和 动画片段

**方式一**： Window => Animation 

**方式二**：Add Component => Animator

Animator Controller 动画控制器，Animation 动画片段，一个Animator Controller 可以控制多个 Animation 动画片段之间切换的逻辑

![example](/Images/animator-exaple.png)

![Animator](/Images/animator.png)  Animator

![Animator](/Images/animation.png) Animation

![Animator](/Images/AnimatorView.png) Animator View


+ Animator => Parameters => " + " 
+ Inspector => Has Exsit Time 
+ 点击动画的某一帧，右键添加事件
+ 可以通过绑定 Animation Clip 的 【开始帧动画】 和 【结束帧动画】 事件，触发我们自定义方法，在自定义方法中设置我们需要设置变量，代码中可以通过判定状态开始和结束，来进行逻辑处理

