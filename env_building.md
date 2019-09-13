## binwalk：

```
	git clone https://github.com/devttys0/binwalk.git
	cd binwalk
	sudo ./deps.sh
	sudo python ./setup.py install
	sudo apt-get install python-lzma
	sudo -H pip install git+https://github.com/ahupp/python-magic
	sudo -H pip install git+https://github.com/sviehb/jefferson
```

## firmadyne：

```
  https://github.com/firmadyne/firmadyne
	sudo -u postgres createuser -P firmadyne    password: firmadyne
	 
	sudo -u postgres createdb -O firmadyne firmware
	sudo -u postgres psql -d firmware < ./firmadyne/database/schema
```
	
## qemu:

```
  wget https://download.qemu.org/qemu-2.4.0.tar.xz
	tar xvf qemu-2.4.0.tar.xz && cd qemu-2.4.0/
	./configure --target-list=arm-softmmu,mips-softmmu,mipsel-softmmu --audio-drv-list=alsa,pa
	make -j8
	sudo make install
```

## gdb-multiarch:
```
  sudo apt-get install gdb-multiarch
```
## gdbserver:
```
  https://github.com/hugsy/gdb-static
```