# netgear_wax206

## telnet enable

git clone https://github.com/bkerler/netgear_telnet
cd netgear_telnet

# 再起動しないと有効にならないことがある
./telnet-enable2.py 192.168.XX.XX 34:XX:XX:XX:XX:XX admin XXXX
telnet 192.168.XX.XX

# region を変更できる US EU JP
/usr/bin/fw_setenv fenv_region XX

# openwrt の管理画面 は事前にtelnetでログインしてroot passwordを変更すると見れる
passwd root
https://192.168.XX.XX/cgi-bin/luci/
