# 物理机配置  
  
**开启虚拟化**：一般是在BIOS里设置`Intel Virtualazation Technology`为Enabled即可（该设置项一般在Configuration选项里）	
	
# VMware配置  
  
**设置进入BIOS前停顿时间**	 
编辑虚拟机文件夹下的.vmx文件，一般在最后添加一行：  
`bios.bootDelay = "5000"`  
单位是毫秒，上面设置结果是等待时间为5秒  
  
**VMware Tools的安装**  
VMware Tools具有很多功能，能改善鼠标移动性，视频和性能。  
  
**修改MAC物理地址**  
针对复制相同环境虚拟机后可能产生MAC地址相同，导致无法联网。  
虚拟机关机状态下，依次：编辑虚拟机设置->网络适配器->高级->MAC地址，点击“生成”即可。(记得可能也要修改操作系统里的MAC地址配置)。  