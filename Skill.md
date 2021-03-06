# VMware 技巧

##### BIOS 设置

方法1：菜单 虚拟机->电源->打开电源时进入固件。  
方法2：鼠标点击到虚拟机里，然后按下 F2 键即可进入 BIOS 设置。(提示：如果开机画面过快，可以设置 bios.bootDelay 来调整时间)。  

##### 导出虚拟机包 OVF 或 OVA

快速使用相同操作系统环境的方法主要有三：  
方法1：复制存放虚拟机文件夹里的所有文件（文件数最多）  
方法2：使用 OVF 虚拟机包（文件数比较少）  
方法3：使用 OVA 虚拟机包（单个文件）  
个人推荐使用第 3 种方法，OVA 单个文件比较方便。  
如何导出 OVF 或 OVA 呢？选中一个关机状态下的虚拟机，点击菜单“文件”>“导出为 OVF”，默认是导出 OVF 文件（后缀名是 .ovf ），倘若在保存时的文件名的后缀名改为 .ova 就能导出为 OVA 的单个文件（将后面的 f 改为 a ，VMware 会自动识别保存的文件格式）。  

##### 善于使用快照功能

虚拟机的快照能将你虚拟机的一些系统状态保存起来，方便各种系统状态的切换。

##### 虚拟机与物理机间文件夹的共享

步骤：
1. 虚拟机关机状态下，依次：编辑虚拟机设置->选项->共享文件夹->文件夹共享 设置 “总是启用” 并 添加物理机中的文件夹。
2. 安装 VMware Tools (已安装可忽略，但版本一定要适合)
3. 虚拟机系统里查看共享的物理机文件夹方法
- Windows 虚拟机系统：网络共享里的 vmware-host 里查看(跟查看网络共享一样)。
- Linux 虚拟机系统：/mnt/hgfs 里查看。

可能出现的问题及解决方法：
- 重新安装 VMware Tools 或 安装最新的 VMware Tools。
- 按照步骤 3 的查看方法。
