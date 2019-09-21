# Dance_until_you_drop



sudo apt-get install ros-melodic-desktop-full

sudo apt-get install ros-melodic-geodesy ros-melodic-pcl-ros ros-melodic-nmea-msgs ros-melodic-libg2o

echo "source /opt/ros/melodic/setup.bash" >> ~/.bashrc

source ~/.bashrc

sudo apt install python-rosinstall python-rosinstall-generator python-wstool build-essential rviz ros-melodic-interactive-markers ros-melodic-interactive-markers libomp-dev ros-melodic-geometry ros-melodic-nav-msgs libsuitesparse-dev


###

git clone https://github.com/PointCloudLibrary/pcl

mkdir build && cd build

cmake .. && make -j12 && sudo make install

git clone https://github.com/RainerKuemmerle/g2o.git

cd g2o

mkdir build && cd build

cmake .. -DCMAKE_BUILD_TYPE=RELEASE

make -j12 && sudo make install

###

mkdir catkin_ws && mkdir catkin_ws/src && cd catkin_ws/src
git clone https://github.com/koide3/ndt_omp.git
