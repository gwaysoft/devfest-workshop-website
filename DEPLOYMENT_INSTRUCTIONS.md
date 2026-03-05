# 部署说明

## 已完成的修改

文件：`styles.css`

修改内容：移动端按钮居中
- 在 `.hero-buttons` 中添加了 `align-items: center;`
- 在 `.btn` 中添加了 `text-align: center;`

## 部署步骤

### 方法 1：通过 GitHub 网页界面上传

1. 访问：https://github.com/gwaysoft/devfest-workshop-website/upload/main
2. 登录账号：gwaysoft@outlook.com
3. 点击 "choose your files" 或拖拽文件
4. 选择本地的 `styles.css` 文件
5. 提交信息填写：`Center buttons on mobile`
6. 点击 "Commit changes"
7. GitHub Actions 会自动部署到 GitHub Pages

### 方法 2：通过 Git 命令行（如果 SSH 问题解决）

```bash
git add styles.css
git commit -m "Center buttons on mobile"
git push origin main
```

## 验证部署

部署完成后，访问 https://gwaysoft.github.io/devfest-workshop-website/ 并在移动端视图下检查按钮是否居中。

## 修改详情

在 `styles.css` 文件的第 338-348 行（移动端媒体查询部分）：

```css
.hero-buttons {
    justify-content: center;
    flex-direction: column;
    gap: 12px;
    align-items: center;  /* 新增 */
}

.btn {
    width: 100%;
    max-width: 300px;
    padding: 12px 24px;
    font-size: 15px;
    text-align: center;  /* 新增 */
}
```
