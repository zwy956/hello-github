# hello-github

> 我的第一个 GitHub 仓库：从零学 Git 与 GitHub 的练手场。

## 这个项目是什么

它不解决任何问题，只解决"我不会用 GitHub"这一个问题。这里记录我从图形界面到命令行、从第一次提交到 Pull Request 的全过程，包括我踩过的每一个坑。

## 技能清单

| 技能 | 状态 | 证据 |
|---|---|---|
| GitHub Desktop 提交 + 推送 | ✅ | `bc4c6bd` |
| 命令行 add / commit / push | ✅ | `ad85c38`（提交了 hello.c） |
| .gitignore 忽略编译产物 | ✅ | `d0551cb` |
| 分支与合并 | ⬜ | 进行中 |
| Fork + Pull Request | ⬜ | 第 5 阶段 |

## 文件说明

- `hello.c` —— 第一个被 Git 跟踪的 C 程序
- `.gitignore` —— 忽略 `*.exe`、`*.o`、`build/` 这类编译垃圾
- `README.md` —— 你正在看的这一页，GitHub 会自动把它渲染成仓库主页

## 代码长这样

```c
#include <stdio.h>

int main(void)
{
    printf("Hello, GitHub!\n");
    return 0;
}
```

## 我的命令备忘

```bash
git status            # 现在什么状态
git add 文件名         # 放进待存档篮
git commit -m "说明"   # 本地存档
git push              # 上传到 GitHub
git log --oneline -5  # 翻历史账本
```

## 踩坑记录（这部分最值钱）

1. **空格是语法**：`git log--oneline-5` 会被理解成找一个叫 `log--oneline-5` 的命令。
2. **Git 从不提醒你打错字**：提交说明里的 `hell0.c`、`bulid` 都是我亲手打错的，它照单全收。
3. **Commit 不等于 Push**：只 commit 不 push，GitHub 网页上什么都不会变。
4. **从聊天窗口复制 Markdown 会被转义**：`\#`、`&#x20;`、莫名多出的空行，就是这个坑留下的痕迹。

---

作者：zwy ｜ 主页：[https://github.com/zwy956](https://github.com/zwy956)
