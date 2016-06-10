# VMware配置  
  
**设置进入BIOS前停顿时间**	 
编辑虚拟机文件夹下的.vmx文件，一般在最后添加一行：  
`bios.bootDelay = "5000"`  
单位是毫秒，上面设置结果是等待时间为5秒  
  
**VMware Tools的安装**  
VMware Tools具有很多功能，能改善鼠标移动性，视频和性能。  