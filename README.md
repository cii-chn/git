# git

Git 练习仓库。用来熟悉日常的提交、分支、推送流程。

## 常用命令速查

```bash
# 初始化
git init -b main

# 查看状态
git status

# 提交
git add .
git commit -m "说明这次改了什么"

# 关联远程仓库
git remote add origin https://github.com/cii-chn/git.git

# 推送（第一次加 -u，之后直接 git push）
git push -u origin main

# 拉取
git pull

# 分支
git branch              # 看分支
git checkout -b dev     # 新建并切到 dev
git checkout main       # 切回 main
git merge dev           # 把 dev 合进当前分支

# 历史
git log --oneline
git diff
```

## 提交信息怎么写

简单说清楚「做了什么」，别写「修改」「更新」这种废话：

- `feat: 新增登录功能`
- `fix: 修复数组越界`
- `docs: 补充 README`

## .gitignore

已经配好了常见忽略项（编译产物、IDE 配置、Python 虚拟环境等），
临时文件不会混进提交记录。
