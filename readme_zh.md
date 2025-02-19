# mad

[English](README.md)

[🗣 News](https://t.me/s/txthinking_news)
[🩸 Youtube](https://www.youtube.com/txthinking) 

为任何域名和IP签发证书

❤️ A project by [txthinking.com](https://www.txthinking.com)

### 安装 via [Nami](https://github.com/txthinking/nami)

    nami install mad

### 使用

```
NAME:
   Mad - Generate root CA and derivative certificate for any domains and any IPs

USAGE:
   mad [global options] command [command options] [arguments...]

VERSION:
   20210401

AUTHOR:
   Cloud <cloud@txthinking.com>

COMMANDS:
   ca       Generate CA
   cert     Generate certificate
   install  Install ROOT CA
   help, h  Shows a list of commands or help for one command

GLOBAL OPTIONS:
   --help, -h     show help (default: false)
   --version, -v  print the version (default: false)
```

### 举例

生成 root CA

```
mad ca --ca ./ca.pem --key ./ca_key.pem
```

为`localhost`生成证书

```
mad cert --ca ./ca.pem --ca_key ./ca_key.pem --cert ./localhost_cert.pem --key ./localhost_cert_key.pem --domain localhost
```

## 开源协议

基于 MIT 协议开源
