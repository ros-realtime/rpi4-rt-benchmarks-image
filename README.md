# rpi4-rt-benchmarks-image

This repository includes the scripts required to generate a
ROS 2 RPI4 image including the tools used for the ROS 2 real-time benchmarks.

## How to build the image

### Humble

```bash
# Clone this repository
git clone https://github.com/ros-realtime/rpi4-rt-benchmarks-image
# Clone the `ros-realtime-rpi4-image` repository
git clone https://github.com/ros-realtime/ros-realtime-rpi4-image
# copy the customized layer to the image_builder directory
cp -r rpi4-rt-benchmarks-image/ros2-rt-benchmark-tools ros-realtime-rpi4-image/image_builder/data
# Build the image
cd rpi4-rt-benchmarks-image
sudo ./ros-rt-img build jammy-rt jammy-rt-humble ros2-rt-benchmark-tools
```