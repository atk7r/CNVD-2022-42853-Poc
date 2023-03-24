# 简介
CNVD-2022-42853禅道16.5 SQL注入Poc

# 声明
此工具仅限授权安全测试使用,禁止非法攻击未授权站点

# 漏洞信息
禅道是一款国产的开源项目管理软件。禅道V16.5未对输入的`account`参数内容作过滤校验，导致攻击者拼接恶意SQL语句执行。

# 使用教程

参数

```
python3 CNVD-2022-42853.py -h
CNVD-2022-42853 Poc by atk7r

options:
  -h, --help            show this help message and exit
  -rh remote_host, --rhost remote_host
                        Please input host to scan.
  -f file_path, --file file_path
                        Please input file path to scan.
  -o outfile_path, --outfile outfile_path
                        Please input path and filename for output file.

```

单个扫描（一定要是ip或者域名，后面可以加端口）

```
python3 CNVD-2022-42853.py.py -rh 192.168.0.1
python3 CNVD-2022-42853.py -rh 192.168.0.1:8088

python3 CNVD-2022-42853.py -rh www.abc.com
python3 CNVD-2022-42853.py -rh www.abc.com:8088
```

批量扫描（url.txt的内容一定要是ip或者域名，后面可以加端口）

```
python3 CNVD-2022-42853.py -f url.txt -o outfile.txt
```
