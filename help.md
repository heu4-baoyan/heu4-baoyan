# 1 到你的仓库根目录（有 .git 的那层）
PS D:\> cd D:\heu4_baoyan\<你的仓库根>

# 2 看看有哪些改动
git status

# 3 全部加入暂存区
git add -A

# 4 正确提交（注意是 git 空格 commit，再用 -m）
git commit -m "feat: 更新文档与配置"

# 5 若需要先同步远程再推送（避免冲突） 也可以不用
git pull --rebase origin main

# 6 推送到 GitHub
git push origin main

# 7 同步github pages更新
mkdocs gh-deploy --force