![image](https://github.com/SpitFire-666/Toshiba-T3200/assets/38451588/28225772-d040-46ea-84e1-062690178733)


# ℹ Gotchas / Things Worth Knowing

- Early models have a 720KB floppy drive - NOT 1.44MB. Later models included a 1.44MB drive
- Additional memory is on a proprietary expansion card - there are no SIMM slots etc
- External monitor is connected via a CGA connector - NOT VGA
- Accessing the internals involves disassembling the screen (removing the LED stickers)
- Keyboard layout is non-standard. For example, no F11, F12. Alt key is ABOVE Ctrl key. Esc key is where Num Lock would usually be

# 🔢 Model numbers

PA7039U

PA7039E

# Hardware

## Hard Disk Drive (HDD)

![image](https://github.com/SpitFire-666/Toshiba-T3200/assets/38451588/2bd76dbf-bf01-4ace-9560-40b2da76f9c9)

Known models:
- Fujitsu M2227DT

### Alternatives
- XT-IDE CF works fine for me, even with a working HDD. It boots off the original HDD and mounts the CF card as D:\
- To boot from an XT-IDE card, you need to access the BIOS and set HDD to ```None```
- Installing an unsupported HDD via a SCSI card: https://www.youtube.com/watch?v=bdotvenfClw

## Switches/Buttons/Ports

- A/B/PRT should be set to PRT. This switch controls what the parallel port functions as.

With switch set to "A", external FDD port is accessed as drive A; internal 3.5" FDD as drive B.
With switch set to "B", external FDD port is accessed as drive B; internal 3.5" FDD as drive A.
Switch is set to "PRT" for parallel printer output.
Computer must be re-booted for switch change to take effect.

### DIP Switches

![image](https://github.com/SpitFire-666/Toshiba-T3200/assets/38451588/e634b0d1-955c-4d50-9c72-75b82917fd3c)


### Soft Switches

![image](https://github.com/SpitFire-666/Toshiba-T3200/assets/38451588/52430930-67ba-4a8d-a16f-36bd57008271)

## 🖥 Display

Panel: Matsushita MD400F720PD1 (PCB: M400F720BDT52)

- Pics of display panel (PDP): https://imgur.com/a/PFSZChy

### How to disassemble/replace the display

https://www.youtube.com/watch?v=bdotvenfClw


## ⌨️ Keyboard

https://deskthority.net/viewtopic.php?f=62&t=603&start=

## Memory / RAM

### Built-in

[Info about DOS/XMS/EMS](https://forum.vcfed.org/index.php?threads/himem-sys-not-finding-xms-on-a-toshiba-t3200.53833/page-2)

### Optional 3MB RAM/Memory Module

Plugs into motherboard

Known models
- kingston ktt-3200 3b
- Cubig T3M7137
- F32MEM 36P711476G01
- PA7137U

![image](https://user-images.githubusercontent.com/38451588/155870440-f8ff2c20-6b7f-4a02-b392-b47d59b2946e.png)

![image](https://github.com/SpitFire-666/Toshiba-T3200/assets/38451588/cb65bce6-f0b2-47b2-8f09-263055b5bcbf)

![image](https://github.com/SpitFire-666/Toshiba-T3200/assets/38451588/8bd7a584-7f37-4200-8b7d-5edc0644f4f5)

https://forum.vcfed.org/index.php?threads/himem-sys-not-finding-xms-on-a-toshiba-t3200.53833/page-2

## 💾 Floppy Disk Drive (FDD)

- 26-pin 

![image](https://github.com/SpitFire-666/Toshiba-T3200/assets/38451588/b23b0648-bc03-4332-a030-894b7d51b496)

![image](https://github.com/SpitFire-666/Toshiba-T3200/assets/38451588/88ad08e3-b431-482a-a11b-b07c8e6ebdf4)


Known model numbers
Toshiba ND-356S-A (1.44MB)


# BIOS / CMOS

- Use ```TEST3.EXE``` to access the BIOS
- Can also use Shift + Control + F10 at startup

## 🔋 CMOS Battery

- Mine has a Tadiran 3.6v battery with a 3.3k resistor (orange, orange, purple, gold)

# 🔌 Power Supply (PSU)

# 💾 Software

Machine came with MS-DOS 3.3 from the factory

## XCHAD

Use XCHAD to adjust colours

Ctrl + SysReq brings up the UI

## Apps and Games

Stuff I've seen running on these beasts

- Space Quest III
- XTree GOld
- Fire Hawk
- 8088 Domination: https://www.youtube.com/watch?v=6vTPqO2sgrU
- ModPlayPlus
- Sound Blaster Pro Intelligent Organ 
- Creative Talking Parrot
- PC Paint
- Planet X3
- Arkanoid
- Commander Keen 1
- CD-MAN 
- Zaxxon
- Tower Toppler
- Accolade Grand Prix Circuit
- Double Dragon
- prince of persia
- space racer
- prehistorik
- Falcon
- Striker

| Software | Yay/Nay/Other | Comment |
| -------- | -------- | -------- |
| stars.com    | Yay   |    |
| LXPic | Yay | | 
| PictVIEW | Nay | Requires a 386+ | |
| MS Flight Simulator 4 | Other | Did not work in EGA mono. More testing req'd | 
| Norton Commander 4 | Yay | |
| Doom / FastDoom | Nay | Requires a 386+ | |
| Aquanoid | Nay | Illegal function call? | | 
| BioMenace | Other | Out of memory error with 1MB. Might require more memory, or HIMEM.SYS? | 
| Chip's Challenge (DOS) | Yay | | 
| Ford Simulator | | |
| UGH | | | 
| MS Word 5.5 | | | 

# Troubleshooting

## 🔋 Flat CMOS battery

![image](https://github.com/SpitFire-666/Toshiba-T3200/assets/38451588/c2bf91bf-22d0-4140-9991-6a4ec4aa365a)

## Lines down the screen

https://retropaq.com/repairing-gas-plasma-displays/

## 💾 Floppy drive issues

- Check/replace the 16V 10uF filter caps near the motor driver. They're SMTs

## Connecting an external floppy via the parallel port

https://forum.vcfed.org/index.php?threads/toshiba-t3200-with-no-floppy.29617/

# ℹ️ Info

https://oldcomputer.info/portables/t3200/index.htm

[Retro Swim ]https://www.youtube.com/watch?v=bdotvenfClw

[VWestlife's YouTube tour](https://www.youtube.com/watch?v=hrJgjmAPzmE)

https://www.1000bit.it/scheda.asp?id=1636

https://www.clous.cz/toshiba-t3200/

https://d1rytvr7gmk1sx.cloudfront.net/wp-content/uploads/2017/07/screen-shot-2017-07-11-at-1-32-47-pm.pngz

https://www.youtube.com/watch?v=49SNshVOyxU

https://gtello.pagesperso-orange.fr/t3200_e.htm

https://www.youtube.com/watch?v=gChpa0_5S3Q


## 📚 User manuals

https://usermanual.wiki/Collections/Product-Manuals/Toshiba/Other/Toshiba%20T3200%20-%20Owners%20Manual.pdf

Info: https://minuszerodegrees.net/manuals/Toshiba/Other/Toshiba%20T3200%20-%20Information.pdf


# Media

![image](https://github.com/SpitFire-666/Toshiba-T3200/assets/38451588/7f3a5016-34c5-47f8-9b94-e0ec099bce2e)

https://notebookblog.cz/blog/wp-content/uploads/2022/06/T3200-ad.jpg

![image](https://github.com/SpitFire-666/Toshiba-T3200/assets/38451588/861e9ef8-1253-4b7b-9e7c-1e8dccd96800)

https://www.techrepublic.com/wp-content/uploads/2017/07/screen-shot-2017-07-11-at-1-32-47-pm.png

# 🪛 Disassembly

https://www.youtube.com/watch?v=VU8P75qtYr4
