# HttpServer

基于 **Go + Gin + Socket.IO** 的 HTTP / 实时通信服务端试验项目。

## 结构

代码在 `httpserver/`：

- `app.go`：入口（Gin 中间件、路由、Socket.IO）
- `metadb/`、`metaredis/`：数据库 / Redis 封装
- `sio/`、`logs/`、`idv/`、`src/`：Socket、日志等模块

模块名：`httpserver`（见 `go.mod`，Go 1.16+）。

## 运行

```bash
cd httpserver
go mod download
go run .
```

需自行配置本机 Redis / DB 等依赖（代码中有对应包引用）。
