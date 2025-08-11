<h1 align="center">ROS2-HUMBLE-TRAINING</h1>

# 1. TẠO PACKAGE

- Vào src: **cd ~/ros2_ws/src**

- Cú pháp để tạo package mới: **ros2 pkg create --build-type ament_cmake --license Apache-2.0 <package_name>**

- VD: **ros2 pkg create --build-type ament_cmake --license Apache-2.0 --node-name <tên Node> <tên Package>**

> **ros2 pkg create --build-type ament_cmake --license Apache-2.0 --node-name my_node my_package**

Sau khi tạo package sẽ tạo ra các thư mục sau:
<p align="center">
  <img width="444" height="294" alt="image" src="https://github.com/user-attachments/assets/ad8b4031-4a06-4f94-9242-23e2716f0e4e" />
</p>

# 2 BUILD A PACKAGE

- Trở về thư mục gốc: **cd ~/ros2_ws**
- Build package:
  * Build toàn bộ: **colcon build**
  * Build 1 package bất kỳ: **colcon build --packages-select <tên package>**
  > colcon build --packages-select my_package

# 3 Source the setup file

- Trên 1 terminal mới chuyển đến thư mục **ros2_ws** chạy: **source install/local_setup.bash**

# 4 Use the package

- Vì khi tạp package ta sử dụng đối số: **--node-name** nên khi **RUN** Chạy lệnh sau: **ros2 run my_package my_node**

