# 通用应用配置页面

这个目录包含可复用的隐私政策、技术支持和EULA(最终用户许可协议)页面,适用于所有应用。

## 使用方法

所有页面都支持通过URL参数 `app` 来动态设置应用名称。

### 隐私政策页面

```
https://your-domain.com/privacy.html?app=应用名称
```

### 技术支持页面

```
https://your-domain.com/support.html?app=应用名称
```

### EULA页面

```
https://your-domain.com/eula.html?app=应用名称
```

## 示例

- **超级小孩**: `privacy.html?app=超级小孩`
- **健康习惯**: `privacy.html?app=健康习惯`
- **AI开发助手**: `privacy.html?app=AI开发助手`

## 页面特点

### 设计风格
- 采用极简黑白配色方案
- 使用系统原生字体(-apple-system)
- 响应式设计,适配各种屏幕尺寸
- 符合iOS和Web设计规范

### 隐私政策内容
- 强调本地数据存储
- 说明iCloud备份机制
- 明确无服务器上传
- 涵盖儿童隐私保护
- 列出第三方服务使用情况

### 技术支持内容
- 常见问题解答(7个通用问题)
- iCloud备份和恢复说明
- 数据安全性说明
- 功能建议提交入口
- 联系方式和响应时间

### EULA内容
- 许可授予和使用限制
- 知识产权保护
- 数据和隐私条款
- 免责声明和责任限制
- 终止条款和适用法律
- 完整的法律保护条款(15个章节)

## 文件说明

- `privacy.html` - 隐私政策页面
- `support.html` - 技术支持页面
- `eula.html` - 最终用户许可协议页面
- `*.html.bak` - 备份文件(旧版本)

## 在Flutter应用中使用

在iOS `Info.plist` 中配置:

```xml
<key>PRIVACY_POLICY_URL</key>
<string>https://your-domain.com/privacy.html?app=YourAppName</string>

<key>SUPPORT_URL</key>
<string>https://your-domain.com/support.html?app=YourAppName</string>

<key>EULA_URL</key>
<string>https://your-domain.com/eula.html?app=YourAppName</string>
```

## 更新说明

当需要更新隐私政策或支持信息时:
1. 直接编辑对应的HTML文件
2. 修改"最后更新日期"
3. 所有使用这些页面的应用会自动获得更新

## 联系邮箱

aigrowth@163.com
