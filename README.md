# battery_health_prediction
University project on statistics in Shanghai University
上海大学统计学课程项目

# Dataset
https://www.kaggle.com/datasets/srisyra02/ev-battery-health-prediction-dataset-20k

# How to use Git / 使用方法 Git

## 🇬🇧 English

### Git in 30 seconds

Git is a tool that keeps the history of our project and lets several people work on it without overwriting each other's work. GitHub is the website where the shared copy lives.

| Term | Meaning |
|------|---------|
| **Repository (repo)** | The project folder, tracked by Git |
| **Commit** | A saved snapshot of your changes, with a short message describing them (like "Save" with a comment) |
| **Push** | Send your local commits to GitHub |
| **Pull** | Download the latest changes from GitHub to your computer |
| **Branch** | A separate line of work. You can change things without touching the main version (`main`) |

### First time only: get the project

```bash
git clone https://github.com/<your-username>/battery_health_prediction.git
cd battery_health_prediction
```

### Daily workflow

**1. Pull** the latest version before you start working:
```bash
git checkout main
git pull
```

**2. Create your own branch** (one branch per task, e.g. `pca-analysis`):
```bash
git checkout -b pca-analysis
```

**3. Work** on your files (notebook, code, report...).

**4. Commit** your changes:
```bash
git add .
git commit -m "Add PCA on quantitative variables"
```

**5. Push** your branch to GitHub:
```bash
git push -u origin pca-analysis
```
(After the first time, `git push` is enough.)

### Good habits
- ✅ Always `git pull` before starting to work.
- ✅ Commit small and often, with clear messages.
- ✅ Never work directly on `main`: use your own branch.
- ⚠️ If Git reports a **conflict** (two people edited the same lines), do not panic: open the file, keep the right version between the `<<<<<<<` and `>>>>>>>` markers, then `git add` and `git commit`. Ask the team if unsure.
- ⚠️ Do not commit very large files (check the dataset size before adding it).

### Useful commands
```bash
git status            # What changed?
git branch            # List branches (the current one has a *)
git checkout <name>   # Switch to another branch
git log --oneline     # History of commits
```

---

## 🇨🇳 中文

### 30秒了解 Git

Git 是一个记录项目历史的工具，可以让多人同时协作而不会互相覆盖对方的修改。GitHub 是存放项目共享副本的网站。

| 术语 | 含义 |
|------|------|
| **仓库 (Repository)** | 被 Git 管理的项目文件夹 |
| **提交 (Commit)** | 保存一次修改的"快照"，并附上简短说明（类似带备注的"保存"） |
| **推送 (Push)** | 把本地的提交上传到 GitHub |
| **拉取 (Pull)** | 把 GitHub 上最新的修改下载到自己的电脑 |
| **分支 (Branch)** | 独立的工作线。你可以在不影响主版本（`main`）的情况下修改内容 |

### 第一次使用：获取项目

```bash
git clone https://github.com/<your-username>/battery_health_prediction.git
cd battery_health_prediction
```

### 日常工作流程

**1. 拉取 (Pull)**：开始工作前，先获取最新版本：
```bash
git checkout main
git pull
```

**2. 创建自己的分支**（每个任务一个分支，例如 `pca-analysis`）：
```bash
git checkout -b pca-analysis
```

**3. 开始工作**：修改文件（Notebook、代码、报告等）。

**4. 提交 (Commit)** 你的修改：
```bash
git add .
git commit -m "Add PCA on quantitative variables"
```

**5. 推送 (Push)** 你的分支到 GitHub：
```bash
git push -u origin pca-analysis
```
（第一次之后，直接使用 `git push` 即可。）

### 良好习惯
- ✅ 开始工作前，务必先 `git pull`。
- ✅ 小步快跑，经常提交，提交说明要清晰。
- ✅ 不要直接在 `main` 上修改，请使用自己的分支。
- ⚠️ 如果 Git 提示**冲突 (conflict)**（两个人修改了同一处内容），不要慌：打开文件，在 `<<<<<<<` 和 `>>>>>>>` 标记之间保留正确的版本，然后执行 `git add` 和 `git commit`。不确定时请询问队友。
- ⚠️ 不要提交过大的文件（添加数据集前请先检查文件大小）。

### 常用命令
```bash
git status            # 查看哪些文件被修改
git branch            # 查看分支（当前分支前有 *）
git checkout <name>   # 切换到其他分支
git log --oneline     # 查看提交历史
```
