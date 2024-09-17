# 项目说明

## 运行代码的需要执行的步骤为：  

打开终端
cd Swarm-Formation
catkin_make -j1
source devel/setup.bash
roslaunch ego_planner rviz.launch

然后另起一个终端运行  

source devel/setup.bash
roslaunch ego_planner fly_SYSU.launch

## 默认模式为点一次目标点飞SYSU编队，可通过修改配置文件SYSU.yaml中的playmode控制飞行模式。playmode值为1代表点一次目标点，即可自动变队形SYSU；值为2代表需要分别点3个目标点使其按次序变换队形SYSU。

## demo02显示playmode=1的效果，demo01显示playmode=2的效果

## 若编译后报错，请尝试将src/planner/plan_manage 中的文件内容，以及traj_utils的文件内容，逐一进行复制。

## playmode=1时，请只点击一个目标点，最好点击在地图左侧如demo02所示