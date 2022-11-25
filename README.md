# Cài windows lên Linux ở Oracle Cloud (không dùng cho chip Amphere A1, áp dụng chip AMD, Intel)


Ubuntu
1. Lệnh cài

- apt-get update
- apt-get install -y xz-utils openssl gawk file wget

A. Windows 2012 Server (TK: Administrator MK: nat.ee)

wget --no-check-certificate -qO InstallNET.sh 'https://raw.githubusercontent.com/vumail159951/oracle-windows-img/main/InstallNET.sh' && bash InstallNET.sh -dd 'http://63.210.148.61/Oracle_Win_Server2012R2_64_Administrator_nat.ee.gz'

B. Windows 7 Enterprise (TK: Administrator MK: nat.ee)

wget --no-check-certificate -qO InstallNET.sh 'https://raw.githubusercontent.com/vumail159951/oracle-windows-img/main/InstallNET.sh' && bash InstallNET.sh -dd 'http://63.210.148.61/Oracle_Win7_sp1_64_Administrator_nat.ee.gz'


Sau khi chạy lệnh chờ nó tự ngắt putty, chờ thêm 10 phút và lên Oracle cloud reboot lại instance. sau đó chờ 20 - 40 phút cho đến khi máy ở trạng thái Running.
