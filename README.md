# Notes
## Autoware Calibration:
- Launch docker
```
sudo sh run.sh kinetic /media/gary/Data/autoware_folder
```
 kinetic: ROS版本
 /media/gary/Data/autoware_folder 共享数据路径

- Launch autoware
```
～/ros$:  ./run
``` 
- Playing data
```
rosbag play *.bag /rslidar_points:=/points_raw
```
### calibration_publisher
- target_frame: rslidar
- camera_frame: camera
- calibration.yml 
- camera_info_topic_name: /camera_rgb
- image_topic_source: /px2_sekonix_port_ab_rgb/image_rgba
-projection_matrix_topic: /projection_matrix

### Rviz
1.Panels-->Add_new Panel-->ImageViewerPlugin
2. 
