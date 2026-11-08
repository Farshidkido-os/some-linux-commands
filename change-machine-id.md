قدم اول حذف مورد machine-id حال حاظر بعد از کلون کردن هستش
```bash
sudo rm -f /etc/machine-id
```
بعد ساخت یه مورد جدید توسط dbus-uuidget
```bash 
sudo dbus-uuidget --unsure=/etc/machine-id
sudo dbus-uuidget --unsure=
```
و تست مجدد 
```bash
cat /etc/machine-id
```
