# shadowsocks-qt5

#### 1.安装需要的依赖包：
  ```
  sudo apt-get install qt5-qmake qtbase5-dev libqrencode-dev libappindicator-dev libzbar-dev
  如果还少依赖包使用apt-get -f install
  ```
#### 2.直接安装五个deb包，直接省去网上说的用dpkg生成deb的包：
依次执行
```
dpkg -i libssl1.0.0_1.0.1t-1+deb8u7_amd64.deb
dpkg -i libbotan-1.10-0_1.10.8-2+deb8u1_amd64.deb
dpkg -i libqtshadowsocks_1.10.0-1_amd64.deb
dpkg -i libqtshadowsocks-dev_1.10.0-1_amd64.deb
dpkg -i shadowsocks-qt5_2.8.0-1_amd64.deb
```
#### 3.如果执行上面语句以后出现如下错误
```
dpkg: dependency problems prevent configuration of shadowsocks-qt5:
 shadowsocks-qt5 depends on libqrencode3 (>= 3.2.0); however:
  Package libqrencode3 is not installed.
```
执行下面语句
```
dpkg -i libqrencode3_3.4.4-1+b2_amd64.deb
```
