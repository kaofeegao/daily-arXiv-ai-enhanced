# GitHub Secrets 配置

要使邮件发送功能正常工作，需要添加以下 GitHub Secrets：

## SMTP 凭据

1. **SMTP_USER**: 您的 SMTP 用户名（例如邮箱地址）
2. **SMTP_PASS**: 您的 SMTP 密码或授权码

## 配置步骤

1. 登录 GitHub，进入仓库页面
2. 点击 **Settings** 标签
3. 在左侧边栏中点击 **Secrets and variables**
4. 点击 **Actions** 标签
5. 点击 **New repository secret**
6. 添加以下 secrets：

| Secret Name | 说明 | 示例 |
|-------------|------|------|
| SMTP_USER | SMTP 用户名（邮箱地址）| your-email@example.com |
| SMTP_PASS | SMTP 密码或授权码 | your-smtp-password |

## SMTP 服务器配置

当前配置使用的是 yeah.net 的 SMTP 服务器：
- 服务器：smtp.yeah.net
- 端口：587
- 加密：STARTTLS

如果您使用其他邮箱服务，需要修改工作流文件中的 SMTP 服务器配置。
