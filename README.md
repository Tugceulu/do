# do
for gem5
sudo apt update
sudo apt upgrade -y

sudo apt update
sudo apt install -y libxcb-cursor0 libxcb-cursor-dev libx11-xcb-dev libxrender-dev libxext-dev libxfixes-dev


sudo apt update
sudo apt upgrade -y
sudo apt install -y build-essential cmake python3 python3-pip git libgl1-mesa-dev libxcb-xinerama0

chmod +x qt-online-installer-linux-x64-4.10.0.run
./qt-online-installer-linux-x64-4.10.0.run


cd ~
git clone https://github.com/cad-polito-it/ase_riscv_gem5_sim.git
cd ase_riscv_gem5_sim

export QT_INSTALLATION_DIR=~/Qt/6.8.3
export Qt6_DIR=$QT_INSTALLATION_DIR/gcc_64/lib/cmake/Qt6
export CMAKE_PREFIX_PATH=$Qt6_DIR:$CMAKE_PREFIX_PATH

./utils/installation.sh
