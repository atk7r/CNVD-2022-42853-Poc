# 声明
本工具仅限授权安全测试使用,禁止非法攻击未授权站点

# 漏洞信息
漏洞编号：CNVD-2022-42853
漏洞等级: 高危
公开日期：2022-06-14
影响产品:
青岛易软天创网络科技有限公司 禅道企业版 6.5
青岛易软天创网络科技有限公司 禅道旗舰版 3.0
青岛易软天创网络科技有限公司 禅道开源版 16.5
青岛易软天创网络科技有限公司 禅道开源版 16.5.beta1

# 使用教程

参数

```
python3 CNVD-2022-42853.py -h                                                                               
usage: CNVD-2022-42853.py [-h] [-ip] [-f] [-o]

CNVD-2022-42853 Poc by atk7r

options:
  -h, --help          show this help message and exit
  -ip , --ipaddress   Please input url to scan.
  -f , --file         Please input file path to scan.
  -o , --outfile      Please input path for output file.
```

单个扫描（一定要是ip或者域名，后面可以加端口）

```
python3 CNVD-2022-42853.py -ip 192.168.0.1
python3 CNVD-2022-42853.py -ip 192.168.0.1:8088

python3 CNVD-2022-42853.py -ip www.abc.com
python3 CNVD-2022-42853.py -ip www.abc.com:8088
```

批量扫描（url.txt的内容一定要是ip或者域名，后面可以加端口）

```
python3 CNVD-2022-42853.py -f url.txt -o outfile.txt
```

