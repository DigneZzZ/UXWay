# Публикация релиза

1. Откройте [новый релиз](https://github.com/DigneZzZ/UXWay/releases/new).
2. Создайте тег версии, например `v1.2.1`, и укажите название `UXWay 1.2.1`.
3. Прикрепите APK и остальные файлы. Имена файлов могут быть любыми.
4. Добавьте описание изменений, отметьте **Set as the latest release** и нажмите **Publish release**.

Ссылка **Download latest release** на главной странице всегда открывает последний релиз. README обновлять не нужно. Черновики и предварительные версии эту ссылку не меняют.

Публикация через GitHub CLI:

```bash
gh release create v1.2.1 \
  "/path/to/UXWay-1.2.1.apk" \
  --repo DigneZzZ/UXWay \
  --title "UXWay 1.2.1" \
  --notes "UXWay 1.2.1 for Android." \
  --latest
```

Для публикации нужен доступ **Write** к репозиторию. Разработчик: [FireWookie](https://github.com/FireWookie).
