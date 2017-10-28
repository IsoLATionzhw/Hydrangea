
# デフォルト動作

default :
	C:\Users\hp\Desktop\OS11\OS\tolset\z_tools\make.exe img

# ファイル生成規則

ipl.bin : ipl.nas Makefile
	C:\Users\hp\Desktop\OS11\OS\tolset\z_tools\nask.exe ipl.nas ipl.bin ipl.lst

helloos.img : ipl.bin Makefile
	C:\Users\hp\Desktop\OS11\OS\tolset\z_tools\edimg.exe   imgin:C:\Users\hp\Desktop\OS11\OS\tolset\z_tools\fdimg0at.tek \
		wbinimg src:ipl.bin len:512 from:0 to:0   imgout:helloos.img

# コマンド

asm :
	C:\Users\hp\Desktop\OS11\OS\tolset\z_tools\make.exe -r ipl.bin

img :
	C:\Users\hp\Desktop\OS11\OS\tolset\z_tools\make.exe -r helloos.img

run :
	C:\Users\hp\Desktop\OS11\OS\tolset\z_tools\make.exe img
	copy helloos.img C:\Users\hp\Desktop\OS11\OS\tolset\z_tools\qemu\fdimage0.bin
	C:\Users\hp\Desktop\OS11\OS\tolset\z_tools\make.exe -C C:\Users\hp\Desktop\OS11\OS\tolset\z_tools\qemu

install :
	C:\Users\hp\Desktop\OS11\OS\tolset\z_tools\make.exe img
	C:\Users\hp\Desktop\OS11\OS\tolset\z_tools\imgtol.com w a: helloos.img

clean :
	-del ipl.bin
	-del ipl.lst

src_only :
	C:\Users\hp\Desktop\OS11\OS\tolset\z_tools\make.exe clean
	-del helloos.img
