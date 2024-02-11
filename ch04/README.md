# 004 在 U 盘启动

* 没有分区表不能启动 

## 主引导扇区的结构

* 代码: 446B
* 分区表: 64B + 4 * 16B
* 魔数: 0xaa55

```console
dd if=boot.bin of=usb.bin bs=446 count=1 conv=notrunc
```