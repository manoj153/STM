Sucessfull make and flash with openocd

*/ #1 Open ocd script*/
openocd -f /usr/share/openocd/scripts/board/st_nucleo_f401re.cfg

*/ #2 Telnet to connect to openocd*/
telnet localhost 4444

*/ #3 Telnet session with openocd commands to flash */
> reset halt
> flash write_image erase main.hex
> reset run

Refrences Link : 

http://regalis.com.pl/en/arm-cortex-stm32-gnulinux/



