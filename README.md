# SyncTV Synology Build

使用群晖官方 DSM 7.2 交叉工具链，自动构建并发布 SyncTV 服务端二进制文件。

## 兼容性

- Synology DSM 7.2+
- amd64 / x86_64
- armv8 / aarch64

## 下载

请从 Releases 下载对应架构的未压缩二进制文件：

- amd64：`synctv-dsm72-amd64`
- armv8：`synctv-dsm72-armv8`

同时提供 SHA-256 校验文件。下载后执行 `chmod +x synctv-dsm72-*` 添加执行权限。

## 自动更新

GitHub Actions 每天检查 `synctv-org/synctv` 的最新正式 Release。发现尚未发布的新版本时，会自动使用 DSM 7.2 工具链构建两个架构，并创建同版本 Release。草稿版和预发布版不会触发自动构建。

上游项目：https://github.com/synctv-org/synctv
