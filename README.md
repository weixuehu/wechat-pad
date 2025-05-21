# WeChat API（Pad Protocol）

![Golang](https://img.shields.io/badge/language-Golang-blue.svg)
![Beego](https://img.shields.io/badge/framework-Beego-green.svg)

## 微信Pad协议，GO语言源码，使用教学，学会为止，限时低价出售

#### 非常稳定，长期不掉线，功能接口丰富，可多开
#### 最新版微信协议859
#### 防封，永久更新，送内网穿透教程，告别收费代理IP

## 联系QQ：1010331559
## 支持多平台运行（windows，mac，linux）
## 后期统一发送更新内容

## 项目结构

```
wechat-pad/
│
├── Cilent/                 # 客户端相关逻辑处理
│   ├── HybridEcdh.go      # 混合ECDH算法实现
│   ├── NewSpamData.go     # 新Spam数据处理
│   ├── common.go          # 公共数据处理
│   ├── device/            # 设备相关数据和操作
│   ├── mm/                # 微信相关原型定义
│   └── ...
│
├── Mmtls/                  # MMTLS协议实现
│   ├── GenNewHttpClient.go# 生成新的HTTP客户端
│   ├── InitMmtlsShake.go  # 初始化MMTLS握手
│   └── ...
│
├── controllers/            # MVC 控制器
│   ├── Favor.go           # 收藏相关操作
│   ├── Finder.go          # 发现页相关操作
│   └── ...
│
├── models/                 # 数据模型和业务逻辑
│   ├── Favor/             # 收藏相关模型
│   ├── Finder/            # 发现页相关模型
│   └── ...
│
├── conf/                   # 配置文件夹
│   └── app.conf
│
├── main.go                 # 程序入口文件
└── go.mod                  # Go模块定义
```


## 开始使用

### 1. 安装依赖

- 环境要求：Go 1.15+，Redis 5.0+
- 安装依赖：`go mod tidy`
- 配置文件：`conf/app.conf`
```go
go env
go env -w GOPROXY=https://goproxy.cn

go mod tidy

go run main.go
```
### 2. 修改 [app.conf](conf%2Fapp.conf) 数据库配置

### 3. 编译打包
#### Window打包
SET CGO_ENABLED=1
SET GOOS=windows
SET GOARCH=amd64
go build main.go
go build -o vera.exe main.go

#### Mac打包
export GOOS=darwin
export GOARCH=amd64 
go build -o vera_darwin main.go

#### Linux打包
export GOOS=linux
export GOARCH=amd64
go build -o vera main.go


## 联系QQ：1010331559
