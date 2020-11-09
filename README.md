# SI

sudo qemu-system-arm -machine versatilepb -cpu arm1176 -kernel zImage-qemu -append "root=/dev/sda2 console=tty0" -drive file=2015-05-05-raspbian-wheezy-qemu.img,index=0,media=disk,format=raw -net nic,model=smc91c111,netdev=bridge -netdev bridge,br=virbr0,id=bridge -serial stdio


fastcgi.server = ( ".php" => ((
                     "bin-path" => "/usr/bin/php-cgi",
                     "socket" => "/tmp/php.socket"
                 )))
