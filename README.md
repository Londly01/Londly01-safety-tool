                                   Londly 

一款红队在大量的资产中实现自动化全端口扫描、标题识别、指纹识别、爆破、漏扫的二开工具
 
	
0x00 项目概述
     
     将原理简单概述一下,把收集到的ip放到ip.txt中，进行CDN过滤，masscan全端口扫描，Fscan扫描，httpx标题识别，将整理的URL进行Finger+observer双重指纹识别，xray+nuclei漏扫。
     
0x01 使用方法
     
     将xray nuclei Finger observer fscan masscan httpx放到根目录下，实现自动化，使用xray高级版效果更佳
     执行：python3 londly.py -i ip.txt  -p 1-65535 --rate 1000 2>&1 &
     执行完上面命令，等着收成果即可，建议使用VPS，一次扫描100个ip，引入fscan是为了扫描web资产和一些弱口令，例如tomcat存在弱口令后进入系统上传war包，拿shell。
     
0x02 免责声明

     该项目仅供授权下使用，禁止使用该项目进行违法操作，否则自行承担后果，请各位遵守《中华人民共和国网络安全法》！

     
 
