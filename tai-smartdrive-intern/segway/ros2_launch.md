# ROS2 控制流程與 Launch 架構筆記

## 架構理解
- 該 ROS2 節點由前輩從 ROS1 改寫，透過 serial 接口控制 Segway RMP 底盤
- 節點包含參數：serial_port、baud_rate、frame_id

## 我的測試方式
- 自寫 Python 腳本發送 `/cmd_vel` topic
- 觀察底盤是否有動作反應（實際尚未完全成功）

## 啟動流程樣板
```bash
ros2 launch segway_ros2 drive_segway.launch.py
```
