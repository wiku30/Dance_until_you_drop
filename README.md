# Dance_until_you_drop



sudo apt-get install ros-melodic-desktop-full

sudo apt-get install ros-melodic-geodesy ros-melodic-pcl-ros ros-melodic-nmea-msgs ros-melodic-libg2o

echo "source /opt/ros/melodic/setup.bash" >> ~/.bashrc

source ~/.bashrc

sudo apt install python-rosinstall python-rosinstall-generator python-wstool build-essential

sudo apt install rviz

sudo apt install ros-melodic-interactive-markers

###

git clone https://github.com/PointCloudLibrary/pcl

mkdir build && cd build

cmake .. && make -j12 && sudo make install

sudo apt install ros-melodic-interactive-markers

sudo apt install libomp-dev

sudo apt install ros-melodic-geometry


