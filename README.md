# 小米笔记本air安装原版Windows7系统

小米笔记本air安装Windows7,以下过程在SN前5位是17245的机型测试通过

### 准备工作
#### 文件
* Windows7原版镜像
cn_windows_7_ultimate_with_sp1_x64_dvd_u_677408.iso
下载地址:在[msdn.itellyou.cn](http://msdn.itellyou.cn/)或者您信任的渠道下载
* 优启通 
下载地址:在[IT天空](https://www.itsk.com/)下载
优启通是一个可以在U盘安装PE系统的安装器
* 万能驱动
在[IT天空](https://www.itsk.com/)下载
* [**重要** **关键**]用于Windows7的NVME硬盘驱动和USB3.0驱动
在本仓库下载zip包
#### 硬件
* U盘1个

### 步骤
1. 双击优启通,在U盘安装PE系统,过程略(注意:此过程会格式化U盘,请提前备份U盘中的文件)
2. 将下载好的Windows7镜像复制到U盘
3. 将驱动zip包解压后得到的文件夹复制到U盘
4. 重启小米笔记本,在开机时按F2进BIOS.选择Security，再选择Set Supervisor Password，这是设置管理员和密码，只有设置了这个，我们下一步才能操作。设置好后，按F10，点Yes。
5. 重启后，继续按F2，就会出现要你输入管理员密码的提示。输入密码进BIOS，选择Security，往下找，选择Secure Boot，选择Disabled，关闭微软安全认证，不然安装win7会蓝屏的。
6. 选择boot，选择硬盘启动模式UEFI改为Legacy。USB Boot改为Enabled，然后选择Boot Devices Order，看有没有Generic Flash Disk也就是U盘。确认后按F10，点Yes重启。
7. 选择进入Win10PE系统
8. 进入PE系统后，打开桌面上的“傲梅硬盘分区”程序。在左侧的“硬盘操作”菜单选择“快速分区”。然后选择分区的数目，建议2个分区就好。在“硬盘的类型”中，选中“MBR”类型，勾选“重建MBR”和“分区对齐到4KB对齐”。然后调整按喜好或需求调整分区的大小，建议C盘100G，剩下的全部D盘。配置好后点击开始执行进行硬盘的格式化。
9. 重启PE，刚刚格式化好的硬盘将成为C盘和D盘。
10. 打开桌面上的“Win系统安装”程序。
11. 在“选择Windows安装源”选择U盘中的Windows7镜像文件。在“选择引导驱动器”选择C盘。在“选择安装驱动器”选择C盘。
12. 在“选项”中选择你要安装的Windows版本(建议选择旗舰版)
13. [**重要** **关键**]勾选“添加驱动”，将选择文件夹指向到U盘中的驱动文件夹
14. 点击开始安装。过程略。
15. 进入Windows7桌面后。打开万能驱动进行驱动的安装。中间可能会要求重启电脑。驱动安装完成后，打开Windows设备管理器，查看是否安装了大部分需要的驱动。
16. 完成


keyword:
xiaomi 小米 笔记本 air 安装 重装 Windows7 win7 Windows10 win10 驱动 nvme 原版
