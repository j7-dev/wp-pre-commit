# wp-pre-commit

一句話說明 `wp-pre-commit`

> 讓你每次 commit 時，自動幫你的 plugin.php 裡的 patch 版本號 +1

> 例如當前版本號是 Version: 1.0.4，commit 後會變成 Version: 1.0.5

<br><br><br>

## 如何使用

在你的專案上 `.git` 目錄下的 `hooks` 目錄裡，放入 `pre-commit` 這個檔案，並且給予執行權限。

```sh
chmod +x pre-commit
```

這樣就完成了，每當你 `commit` 時，會自動把你的 patch 版本號 +1

<br><br><br>

## RoadMap

- 與同時也修改 package.json 的版本號
