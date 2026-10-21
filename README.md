# friends

[吐槽大王部落格](https://www.tcdw.net) 的友情链接页面生成器。

## 提交友情链接

欢迎通过 GitHub Pull Request 提交友情链接申请：

1. Fork 本仓库
2. 编辑 `friends.toml`，在 `[[blogs]]` 或 `[[nonBlogs]]` 部分添加你的站点信息：
   ```toml
   [[blogs]]
   name = "你的站点名称"
   url = "https://your-site.com"
   avatar = "https://secure.gravatar.com/avatar/xxx"
   description = "站点简介（可选）"
   ```
3. 提交 Pull Request

### 要求

- 只能提交你自己的链接
- 必须开启全站 HTTPS，且没有混入 HTTP 资源
- 需要提供一个能够保证稳定的头像图片 URL。建议使用 Gravatar 或 GitHub 头像 URL
  - 重要提醒！！！请勿使用包含构建哈希、版本号等可能随网站重新构建或部署而变化的图片 URL（例如 Next.js 等框架生成的构建产物地址）
  - 如果不想提供 Gravatar 或 GitHub 的头像 URL，请至少使用固定路径的静态资源或独立图床，并确保图片尺寸不超过 200x200
- **跟我的电波能对上**
- 拒绝采集站、内容农场、完全以 AI 生成内容为主的站点

## 开发

安装依赖：

```bash
bun install
```

检查友情链接的健康度：

```bash
bun run healthcheck
```
