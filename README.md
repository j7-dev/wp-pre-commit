# wp-pre-commit

一句話說明 `wp-pre-commit`

> 讓你每次 commit 時，自動幫你的 plugin.php (你的套件入口文件) 裡的 patch 版本號 +1

> 也會把 package.json 裡的版本號與你套件版本號同步

```php
/**
 * Plugin Name: Another WordPress Plugin
 * Description: Lorem ipsum dolor sit amet
 * Author: j7.dev
 * Author URI: https://github.com/j7-dev
 * License: GPLv2
 * Version: 1.0.4
 */
```

> 例如當前版本號是 Version: 1.0.4，commit 後會變成 Version: 1.0.5

<br><br><br>

## 如何使用

在你的專案上 `.git` 目錄下的 `hooks` 目錄裡，放入 `pre-commit` 這個檔案，並且給予執行權限。

```sh
chmod +x pre-commit
```

這樣就完成了，每當你 `commit` 時，會自動把你的 patch 版本號 +1

至於 major 版本(第一個數字，代表大版本更新，可能API不兼容)

以及 minor 版本(第二個數字，代表小版本更新，可能釋放新的功能)

我都建議手動改就好

<br><br><br>

## RoadMap

✅ 同時也修改 package.json 的版本號
