# Rosrot

problem:
sudo rosdep init fail!!
rosdep update

方法1
sudo gedit /etc/hosts
199.232.28.133 raw.githubusercontent.com
151.101.228.133 raw.github.com


方法2：
1.更新rosdep相关文件，增加代理地址

 wget https://gitee.com/ncnynl/rosdep/raw/master/rosdep_update.sh ; sudo chmod +x ./rosdep_update.sh; sudo ./rosdep_update.sh

完成之后，运行rosdep update即不会出现错误提示 脚本只能运行一次，多次运行，会提示重复运行信息

2.恢复rosdep相关文件，去掉代理地址

wget https://gitee.com/ncnynl/rosdep/raw/master/rosdep_recover.sh ; sudo chmod +x ./rosdep_recover.sh; sudo ./rosdep_recover.sh


方法3：
sudo pip3 install rosdepc
sudo rosdepc init
rosdepc update
