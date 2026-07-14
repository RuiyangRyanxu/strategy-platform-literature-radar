# 战略与平台文献雷达

GitHub Pages 静态发布仓库。公开页面位于 `site/`，内容由上级工作区的日报生成器同步。

公开网站：https://ruiyangryanxu.github.io/strategy-platform-literature-radar/

公开归档从 `2026-07-14` 开始，只包含通过现行期刊白名单和日期核验规则的报告。

## 更新公开文件

```bash
cd ..
python3 scripts/build_literature_portal.py \
  --outputs outputs \
  --output outputs/index.html \
  --minimum-date 2026-07-14 \
  --site-dir literature-portal-site \
  --github-pages-dir literature-portal-pages
```

推送 `main` 后，GitHub Actions 会把 `site/` 部署到 GitHub Pages。
