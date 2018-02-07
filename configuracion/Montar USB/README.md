Para montar una unidad usb:
1. Crear el punto de montage:
	sudo mkdir ./<punto de montage>
2. Montar la unidad
	sudo mount -t vfat <unidad> <punto de montage> -o uid=1000,gid=1000,utf8,dmask=027,fmask=137
Automatizar el montage:
Editar el fichero /etc/fstab, y añadir:
	<unidad> <punto de montage>  vfat auto,uid=1001,gid=1001,utf8,dmask=027,fmask=137
