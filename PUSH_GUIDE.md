# 推送说明

当前文件夹已关联到你提供的仓库：

```text
git@github.com:VincentZJW/VincentZJW.git
```

## 手动推送

如果自动推送失败，请在当前项目根目录执行：

```bash
cd profile
git add README.md .github/workflows/snake.yml assets/README.md PUSH_GUIDE.md
git commit -m "创建双语科技风个人介绍 README"
git push -u origin main
```

## 推送前替换占位内容

打开根目录 `README.md`，搜索并替换：

```text
REPLACE_WITH_YOUR_LINKEDIN_SLUG
REPLACE_WITH_YOUR_EMAIL
```

## 蛇形图动画

推送成功后，打开仓库的 `Actions` 页面，手动运行一次 `生成贡献蛇形图`。

工作流会把 SVG 文件发布到 `output` 分支。蛇形图 URL 已按 GitHub Profile 特殊仓库 `VincentZJW/VincentZJW` 配置。

## 安全说明

- 不要把 API Key、token、真实邮箱密码或其他私密凭据写入 README。
- `snake.yml` 使用 GitHub Actions 自动提供的 `GITHUB_TOKEN`，无需手动填写 token。
