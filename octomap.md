# Octomap

Installation:

Download the source code from [https://github.com/OctoMap/octomap\_mapping](https://github.com/OctoMap/octomap_mapping) and build it.

For now we will be installing it directly using apt

```bash
sudo apt-get install ros-melodic-octomap ros-melodic-octomap-mapping
```

Open a new terminal and run it using the following command:

```bash
rosrun octomap_server octomap_server_node /cloud_in:=/orb_slam2_rgbd/map_points
```

Note that we are remapping the `cloud_in` topic to `orb_slam2_rgbd/map_points`

Later on we will directly add this change to the launch file.

