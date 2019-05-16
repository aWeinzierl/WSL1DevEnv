# WSL1DevEnv

- WSL Activation (PS Admin): `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux`

- X-server installation: //TODO

- X-server auto start: //TODO

- CLion (ssh port: 2222): `cd && sudo apt-get install cmake gcc clang gdb build-essential && wget https://raw.githubusercontent.com/JetBrains/clion-wsl/master/ubuntu_setup_env.sh && bash ubuntu_setup_env.sh && rm ubuntu_setup_env.sh`
Source: https://www.jetbrains.com/help/clion/how-to-use-wsl-development-environment-in-clion.html

- X11-Forwarding: `export DISPLAY=localhost:0.0" >> ~/.bashrc`

- ROS (Melodic: Full): `sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list' && sudo apt-key adv --keyserver hkp://ha.pool.sks-keyservers.net:80 --recv-key 421C365BD9FF1F717815A3895523BAEEB01FA116 && sudo apt update && sudo apt install ros-melodic-desktop-full && sudo rosdep init && rosdep update && echo "source /opt/ros/melodic/setup.bash" >> ~/.bashrc && source ~/.bashrc && sudo apt install python-rosinstall python-rosinstall-generator python-wstool build-essential`
Source: http://wiki.ros.org/melodic/Installation/Ubuntu
