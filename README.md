---
# 🚫 404 – 文件未找到（但这里是我存放错误代码的地方）

> **说明**：这个页面并不是真正的 404 错误，而是我特意设计的一个“伪 404”页面。  
> **用途**：用来集中存放和管理我在开发过程中遇到的各种错误代码、报错信息以及解决方案。  
> **方便**：遇到问题可以快速翻查，不用到处找日志。

---

<div style="font-family: 'Courier New', monospace; background: #0d1117; color: #c9d1d9; padding: 30px; border-radius: 12px; border: 1px solid #30363d; max-width: 800px; margin: 0 auto;">

## ⚠️ 404 – 此页面仅为错误代码仓库

您所请求的页面并不存在（这本来就是假的），但您正好来到了我的“错误代码集散地”。

---

### 📋 最近收录的错误（按时间倒序）

#### 1. `GitHub API: Resource not accessible by personal access token`
- **时间**：2026-07-27 14:23
- **原因**：Token 权限不足，未勾选 `repo` 范围。
- **解决**：重新生成 Token，确保勾选 `repo` 权限。

#### 2. `Python: ModuleNotFoundError: No module named 'playwright'`
- **时间**：2026-07-26 22:15
- **原因**：未安装 Playwright 依赖。
- **解决**：执行 `pip install playwright` 并运行 `playwright install`。

#### 3. `GitHub: Couldn't check availability`
- **时间**：2026-07-26 20:05
- **原因**：网络波动导致前端检查超时，但后端仍可正常创建。
- **解决**：忽略提示，直接点击“Create repository”即可。

#### 4. `HTML: CORS policy blocked request`
- **时间**：2026-07-26 19:30
- **原因**：在浏览器中直接请求第三方 API 被跨域策略拦截。
- **解决**：使用后端代理（如 Node.js/ Python）或启用 CORS 插件（仅开发时）。

---

### 🧰 常用错误代码速查

| 错误码 | 含义 | 常见场景 |
| :---: | :--- | :--- |
| 401 | Unauthorized | Token 无效或未提供 |
| 403 | Forbidden | 权限不足 |
| 404 | Not Found | 资源不存在 |
| 422 | Unprocessable Entity | 请求参数非法（如仓库名重复） |
| 500 | Internal Server Error | 服务器内部异常 |
| 502 | Bad Gateway | 代理/网关错误 |