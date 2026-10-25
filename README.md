# 微生物菌落形态图谱在线平台

食源性致病菌菌落形态交互式在线平台。核心为**致病菌 × 培养基的生长交互热图**，并提供菌落形态照片检索、账号 / 角色 / 审核流、照片上传与统计分析等协同能力。

## 技术栈

- 前端：单文件 `index.html`（原生 HTML / CSS / JS，无需构建）
- 本地缓存：`localStorage`
- 后端：[Supabase](https://supabase.com/)（auth 登录 / storage 存储 / database 数据）

## 目录结构

| 路径 | 说明 |
| --- | --- |
| `index.html` | 主程序（单文件应用） |
| `菌落使用照片/` | 菌落形态照片资源 |
| `交互式检索细菌图片/` | 细菌图片交互检索模块 |
| `LICENSE` | 许可证 |

## 本地预览

直接用浏览器打开 `index.html` 即可；需要登录 / 上传等后端能力时，依赖 Supabase 项目配置。

## 部署

线上部署于 **GitHub Pages**（`guitarmancoder.github.io/microbial_atlas`）。当前采用**手工更新**：将最新 `index.html` 上传覆盖即可。

> ⚠️ 历史教训：手工更新时**不要「先删再传」**，否则可能把线上仓库清空成只剩 README。请直接覆盖上传。

## Git 规范

- 仓库已忽略 `.DS_Store`、编辑器临时文件等（见本文件）；
- 菌落照片等二进制资源当前随仓库提交管理（后续可迁移至 Supabase storage 以减小仓库体积）。

---

作者：王欣（Wang Xin）
