README

author:haha
date: 2014-5-4 15:08:38



FILES

tcpdump:			arm elf file for dump the network data stream.
tcpdumpshell.sh:	capture the network data stream for analysis.
hosts:				hosts that includes "host dns of ads" to redirect 127.0.0.1
					Now, I replaced to /system/etc/hosts in android.


USAGE

in android:
1. push tcpdump and tcpdumpshell.sh to /system/bin/,chmod 777 with them.
2. run tcpdumpshell.sh to caputre the network data stream to analyse.
3. add the dns to hosts with correct ways.
4. push hosts to /system/etc/.
5. OK now, the ads cannot show again. ^_^

--------------------------------------------------------
android去广告host配置文件说明

android系统中，广告地址一般是基于域名进行广告地址链接请求和数据回传。
修改hosts文件中的域名重定向数据，让广告链接全部重定向到本地，造成访问失败。
也就不会成功获取广告，进而播放也会失败，达到去掉广告的目的。
