# 绿茶白底 · Gitea Theme

高对比黑 / 绿 / 白 / 浅绿 / 浅灰。白底绿茶，线条清晰，布局克制，过渡丝滑。
![效果演示图]([https://static.jyshare.com/images/runoob-logo.png)](https://github.com/kaka77/green-tea-gitea/blob/main/demo.png?raw=true)

## 安装

1. 将 `theme-green-tea.css` 放到：

   ```
   $GITEA_CUSTOM/public/assets/css/theme-green-tea.css
   ```

   `$GITEA_CUSTOM` 可用 `gitea help` 查看 CustomPath。  
   旧版（Gitea < 1.21）路径为 `$GITEA_CUSTOM/public/css/`。

2. 编辑 `app.ini`：

   ```ini
   [ui]
   THEMES = gitea-auto,gitea-light,gitea-dark,green-tea
   DEFAULT_THEME = green-tea
   ```

   不写 `THEMES` 时，Gitea 会加载 `public/assets/css/theme-*.css` 下全部主题。

3. 重启 Gitea。用户可在 **设置 → 外观** 选择「绿茶白底」。

## 色板

| 角色 | 色值 | 用途 |
| --- | --- | --- |
| 墨黑 | `#141816` | 正文、标题 |
| 龙井绿 | `#2d6a4b` | 主色、链接、主按钮 |
| 纯白 | `#ffffff` | 页面底、卡片 |
| 浅绿 | `#e3f6ea` / `#d8f3dc` | 高亮、成功、hover |
| 浅灰绿 | `#f3f6f4` / `#c9d4cc` | 导航、边框 |

对比：正文对白底约 16:1，主色按钮白字满足 AA。

## 文件

- `theme-green-tea.css` — 可直接部署的主题
- `demo.html` — 独立预览（不依赖 Gitea）
