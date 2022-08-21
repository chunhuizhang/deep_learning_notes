
## 0. 系统硬件及服务配置

- bios
    - 开机 f2，进入bios，boot configuration
        - 禁用BIOS中的安全启动模式secure boot
- grub
    - sudo gedit /etc/default/grub

- 开机启动项禁止
    - `/etc/modprobe.d/blacklist`
        - `blacklist driver-name`
            - `blacklist nouveau`
        - modprobe是linux的一个命令，可载入指定的个别模块，或是载入一组相依的模块。modprobe会根据depmod所产生的相依关系，决定要载入哪些模块。若在载入过程中发生错误，在modprobe会卸载整组的模块。
        
- 命令行及图形界面
    - drm：direct rendering manager
    - `ctrl + alt + f4：纯命令行界面` 

## 1. 显卡相关

- `lspci | grep -i nvidia`

## 2. 文件系统

- `/dev/null`


## 3. softwares

- pycharm
    - `snap find pycharm`
    - `sudo snap install pycharm** --classic`

