# 開發專案流程

開始python專案的一些事前工作，記錄下來以方便之後操作。

## 1. 建立README.md

在專案資料夾內新增  **README.md**

## 2. 建立 .vscode/settings.json

在專案資料夾內新增: .vscode/settings.json

```
{
    "[python]": {
        "editor.defaultFormatter": "ms-python.black-formatter",
        "editor.formatOnSave": true,
        "editor.codeActionsOnSave": {
            "source.organizeImports": "explicit"
        }
    },
    "[django-html]": {
        "editor.formatOnSave": true,
        "editor.defaultFormatter": "monosans.djlint"
    },
    "[javascript]": {
        "editor.formatOnSave": true,
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    }
}
```

- 關於vscode settings的設定，可以參考以下文章:
[Vscode如何快速打开用户的 settings.json 文件](https://blog.csdn.net/weixin_45277161/article/details/131330341)


## 3. 新增poetry套件管理工具:  

使用 Poetry 來管理Python套件

可參考以下專案來操作:
[poetry套件](https://github.com/ZzKaiJun/learn_poetry)

## 4. 建立.gitignore

建立 .gitignore 防止不必要的檔案上傳至git

```
__pycache__
```