---
title: "Livox ROS 2 Driver for Lidar Sensors"
date: 2025-03-19T12:00:00+00:00
weight: 2
description: "AGV Lidar sensor (GOIMEK pilot)"
license: "https://img.shields.io/badge/License-Apache%202.0-yellowgreen"
trl: "https://img.shields.io/badge/TRL-9-green"
link: "https://github.com/COGNIMANEU/pilot02-physical-livox-lidar"
github: "https://github.com/COGNIMANEU/pilot02-physical-livox-lidar"
---

## Name
Livox ROS 2 Driver for Lidar Sensors

## Description

This project provides an easy-to-use setup for integrating Livox Lidar devices into ROS 2. The `livox_ros_driver2` node supports configuration via JSON and RViz files, and the system can be run inside a Docker container for ease of use.

The repository includes the following components:
- Configuration files for the Livox Lidar device
- Launch files for running the ROS 2 node
- Docker setup for easy containerization
- A docker-compose based test environment to verify the topics published by the Livox driver (lidar hardware required)

## Guidelines for build and test the component 

### 1. **Build the Main Docker Image:**

In this step, we build the Docker image using the provided `Dockerfile`. The image is named `pilot02-physical-livox-lidar`.

```bash
docker build -t pilot02-physical-livox-lidar .
```

Make sure the path to your configuration and launch files is correctly mapped to the Docker container.

### 2. **Run the ROS 2 Container:**

After building the Docker image, you can run the container using the following command:

```bash
docker run -e LAUNCH_FILE=your_custom_launch_file.py pilot02-physical-livox-lidar
```

This will start the container and launch the ROS 2 node with the configured launch file.

### 3. **Build and Run the test automation:**

Test automation is integrated by docker-compose file:

Run: 
```bash
docker-compose up --build
```

In case lidar hardware is ready, you should see:
```python
✅ PointCloud2 message received!
```

In case of errors, you should see:
```python
❌ No PointCloud2 message was received
```

## Example for cogniman pilot02

Build component: 
```bash
docker build  -t pilot02-physical-livox-lidar .
```

Rebuild component (no cache):
```bash
docker build --no-cache -t pilot02-physical-livox-lidar .
```

Run component : 
```bash
docker run -e LAUNCH_FILE=livox_hub_launch.py pilot02-physical-livox-lidar
```

Build test: 
```bash
docker build -t test-pilot02-physical-livox-lidar ./test
```

Rebuild test (no cache):
```bash
docker build --no-cache -t test-pilot02-physical-livox-lidar ./test
```
Run test: 
```bash
docker run -it --rm test-pilot02-physical-livox-lidar
```

## Contributing

Feel free to open issues or submit pull requests. Contributions are welcome!

## License

This project is licensed under the Apache 2 Licences, but includes MIT License and 3-Clause BSD License components - see the [LICENSE](https://github.com/COGNIMANEU/pilot02-physical-livox-lidar/blob/main/LICENSE) file for details.