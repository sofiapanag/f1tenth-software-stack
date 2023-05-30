# ESE-615-Final-Project
ESE 615 Final Project repository of Team 6. For various resources and software development. <br>
Website: https://derekhanbaliq.weebly.com/f1tenth.html

## Intro to Supported Repos

**f1tenth_traj_gen**: trajectory generation repo for solving min curvature QP with F1TENTH params. The dev is based on [TUM's global traj optim repo](https://github.com/TUMFTM/global_racetrajectory_optimization). For f1tenth dev, the tuned parameter is locally stored in IL folder of Derek's OMEN-16 via Windows 11 OS.


## Wireless Visualization via Rviz2

Thanks to the [ESE 615 tips](https://docs.google.com/document/d/1PhaZvV0ZKzfTiwoJAoGcjTY9W2EPkMq2NKQgz8E-glk/edit)!
```bash
ifconfig  # check wlan0, should be same to the car's
echo "export ROS_DOMAIN_ID=6" >> ~/.bashrc
sudo ufw disable  # disable the firewall
rviz2  # on your native ubuntu and add the topics, start rviz2 before pf!
```

<!-- Bringup Instructions:
All parameter tuning should be done in launch -> real_bringup_launch.py or sim_bringup_launch.py. 
Please open the relevant file for further settings.
Open CMakeLists and switch between the commented out lines with the uncommented ones in install to determine which launch file will be used. -->
