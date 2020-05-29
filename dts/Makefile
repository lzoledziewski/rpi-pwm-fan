all: rpi-pwm-fan.dtbo

rpi-pwm-fan.dtbo: rpi-pwm-fan-overlay.dts
	dtc -@ -Hepapr -I dts -O dtb -o rpi-pwm-fan.dtbo rpi-pwm-fan-overlay.dts
install: rpi-pwm-fan.dtbo
	sudo cp rpi-pwm-fan.dtbo /boot/overlays/
