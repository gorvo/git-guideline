# Git Guideline

Git 準則。

## 目錄
* [Default gitignore Template](#default-gitignore-template)
* [Initial commit](#initial-commit)
* [Commit Message Format](#commit-message-format)

## Default gitignore Template

範本 `.gitignore` 文件。

詳見 `Default.gitignore` 。

## Initial commit

初始 Commit 如下：

```
git commit -m "Initial commit"
```

## Commit Message Format

Commit Message 之格式，標準如下：

```
<header>
<BLANK LINE>
<body>
<BLANK LINE>
<BLANK LINE>
<footer>
```

### Commit Message Header

標題， `header` 格式如下：

```
<type>(<scope>) <subject>
```

- **type**: 必要欄位。
- **scope**: 必要欄位。
- **subject**: 必要欄位。

範例如下：

```
[Feat](HisotryModal) Add history modal
```

#### Type

類別，須為下列其一：

- **Feat**: 新增 / 修改功能。
- **Chore**: 次要內容變動。
- **Refactor**: 內容重構。
- **Fix**: 修正錯誤。
- **Docs**: 新增 / 修改文件。
- **Style**: 程式碼格式，例如：換行、空白。
- **Perf**: 改善效能。
- **Test**: 新增 / 修改測試。

#### Scope

影響範圍， `scope` 依專案而不同，例如： `Index` 、 `boilerplate` ，不需加入副檔名。

若為描述性單字則為小寫，例如： `all`。

範例如下：

```
[Feat](all) Add outline none mixin
```

#### Subject

主旨，首字大寫，結尾不需加句號。

不可超過 50 個字元，若內容即將超過 50 個字元，則以 `...` 省略，並於 `body` 中詳細說明。

範例如下：

```
[Refactor](VideoModal) Rename VideoModal action...
```

### Commit Message Body

條列式內容， `body` 範例如下：

```
Add toolbox and image panel open close function.
Add menu slice.
```

### Commit Message Footer

與其他事件相關之註記， `footer` 範例如下：

```
PR #<pull request number>
```