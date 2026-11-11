# Echo Voice — загрузки для Windows

Это **официальный публичный репозиторий с установщиками Echo Voice**, опубликованный автором проекта. Здесь размещаются только готовые сборки приложения, контрольные суммы и инструкции. Основной репозиторий с кодом сервиса остаётся отдельным и приватным.

**Сайт:** https://echo-voice-production.up.railway.app/

**Актуальный Windows-релиз: 1.5.0.** Номер версии также показывается рядом со скачиванием на сайте. После следующей публикации обновляйте эту строку вместе с номером на сайте.

## Скачать приложение

Перейдите в [последний релиз](https://github.com/artemisfox112/echo-voice-downloads/releases/latest) и выберите один из файлов:

- **EchoVoice-Setup.exe** — установка для Windows 10/11 x64 с выбором папки; в обычную пользовательскую папку права администратора не нужны.
- **EchoVoice-Windows-Portable.zip** — портативная версия. Распакуйте архив целиком и запустите `EchoVoice.exe`.
- **SHA256SUMS.txt** — контрольные суммы опубликованных файлов для проверки целостности.

Для Windows-клиента требуется **Microsoft Edge WebView2 Runtime**. Echo Voice позволяет создавать голосовые комнаты без регистрации, общаться в чате и сворачивать приложение в системный трей.

**Как проверить обновление:** откройте Параметры Windows → Приложения → Echo Voice и сравните установленную версию с номером на сайте. Автообновления пока нет: если версия устарела, скачайте актуальный установщик с этой страницы и запустите его поверх старой версии. Папка установки и локальный профиль WebView2 сохраняются.

> **Внимание:** установщик пока **не имеет цифровой подписи издателя**. Windows SmartScreen может показать предупреждение о неизвестном приложении. Проверяйте адрес официального репозитория и SHA-256 файла перед запуском. Предупреждение само по себе не доказывает ни безопасность, ни вредоносность файла.

### Проверка скачанного файла

В PowerShell:

```powershell
Get-FileHash .\EchoVoice-Setup.exe -Algorithm SHA256
```

Сравните полученное значение с записью в `SHA256SUMS.txt` соответствующего релиза.

## English

Official Echo Voice desktop downloads for **Windows 10/11 (64-bit)**. The setup lets you choose a destination folder; the portable ZIP runs after extraction without installation. See [latest releases](https://github.com/artemisfox112/echo-voice-downloads/releases/latest). The app is **currently unsigned**; verify SHA-256 checksums before running. Microsoft Edge WebView2 Runtime is required.

The private main application repository is separate from this public downloads-only repository.
