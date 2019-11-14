# Dance_until_you_drop

http://math.stanford.edu/~vakil/216blog/FOAGjun1113public.pdf

********************************************************************

sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'

sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654

sudo apt update

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
