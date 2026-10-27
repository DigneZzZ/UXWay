# Публикация релиза

1. Откройте [новый релиз](https://github.com/DigneZzZ/UXWay/releases/new).
2. Создайте тег версии, например `v1.2.1`, и укажите название `UXWay 1.2.1`.
3. Прикрепите один APK и остальные файлы. Имя APK может быть любым.
4. Добавьте описание изменений, отметьте **Set as the latest release** и нажмите **Publish release**.

После публикации GitHub Actions автоматически переименует APK в `UXWay.apk`. Ссылка **Download for Android** на главной странице скачивает этот файл из последнего релиза напрямую. README обновлять не нужно. Черновики и предварительные версии эту ссылку не меняют.

Проверьте успешное выполнение [Keep the APK download link current](https://github.com/DigneZzZ/UXWay/actions/workflows/stable-apk.yml): переименование обычно занимает несколько секунд. Если в релизе несколько APK, универсальную сборку назовите `UXWay.apk` перед загрузкой.

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
