# BLEAKFATE for Android — security policy

## Supported versions

Only the latest release is supported, and security fixes come out as a new release. If you use an older version, update to the [latest release](https://github.com/MostViable/bleakfate-android/releases/latest) and check whether the problem is still there.

## Reporting a vulnerability

Report security problems privately in our support bot, [@BleakFateSupportBot](https://t.me/BleakFateSupportBot), not in public issues. We reply in the bot.

Please include:

- the app version;
- your Android version and phone model;
- the steps to reproduce the problem;
- the impact: what an attacker could do and whose data is at risk.

Do not put other people's data, subscription links or keys in the report. If the problem involves them, describe where they show up instead.

## Scope

In scope:

- the BLEAKFATE app for Android from the releases of this repository;
- the BLEAKFATE account and subscription services the app uses on `bleakfate.com` and `sub.bleakfate.com`.

Out of scope:

- denial of service, spam and social engineering;
- other apps you may use with a BLEAKFATE subscription, such as Happ or INCY: report problems in them to their developers;
- bugs in the open-source components the app is built on: report Xray-core and libXray bugs to [XTLS](https://github.com/XTLS), and hev-socks5-tunnel bugs to [its repository](https://github.com/heiher/hev-socks5-tunnel). If such a bug affects the BLEAKFATE app, you can tell us about it too.

## Testing rules

- Test only with your own account and subscription.
- Do not open, change or delete other people's data. If you come across it by accident, stop, tell us, and do not keep or share it.
- Do not put load on the service: load tests, mass scanning and brute-forcing passwords or codes against our servers are not allowed.

## Verifying a release

Every release has `BLEAKFATE.apk.sha256` next to the APK. Put both files in one folder and check the download:

```
sha256sum -c BLEAKFATE.apk.sha256
```

All releases are signed with the same key. With the Android SDK, `apksigner verify --print-certs BLEAKFATE.apk` must show this SHA-256 certificate digest:

```
b6fa737b90b114ed4144ee2f0c7d00559fcbc81fbe890f59636d3142e93c51f8
```

A file signed with any other key is not ours: do not install it, and tell us in the support bot where you found it.

---

# BLEAKFATE для Android — политика безопасности

## Поддерживаемые версии

Поддерживается только последний выпуск, исправления безопасности выходят новым выпуском. Если у вас старая версия, обновитесь до [последнего выпуска](https://github.com/MostViable/bleakfate-android/releases/latest) и проверьте, осталась ли проблема.

## Как сообщить об уязвимости

О проблемах безопасности пишите напрямую в бот поддержки [@BleakFateSupportBot](https://t.me/BleakFateSupportBot), а не в открытые issues. Отвечаем в боте.

Укажите:

- версию приложения;
- версию Android и модель телефона;
- шаги, по которым проблему можно повторить;
- последствия: что может сделать злоумышленник и чьи данные под угрозой.

Не присылайте чужие данные, ссылки подписки и ключи. Если проблема их касается, опишите, где они появляются.

## Что входит

Входит:

- приложение BLEAKFATE для Android из выпусков этого репозитория;
- сервисы аккаунта и подписки BLEAKFATE на `bleakfate.com` и `sub.bleakfate.com`, к которым обращается приложение.

Не входит:

- отказ в обслуживании (DoS), спам и социальная инженерия;
- другие приложения, которыми можно пользоваться с подпиской BLEAKFATE, например Happ или INCY: о проблемах в них пишите их разработчикам;
- ошибки в открытых компонентах, на которых построено приложение: об ошибках Xray-core и libXray сообщайте [XTLS](https://github.com/XTLS), об ошибках hev-socks5-tunnel — в [его репозиторий](https://github.com/heiher/hev-socks5-tunnel). Если такая ошибка задевает приложение BLEAKFATE, можно написать и нам.

## Правила проверки

- Проверяйте только на своём аккаунте и своей подписке.
- Чужие данные не открывайте, не меняйте и не удаляйте. Если наткнулись на них случайно, остановитесь и напишите нам; сохранять и передавать их нельзя.
- Не нагружайте сервис: нагрузочные тесты, массовое сканирование и перебор паролей или кодов на наших серверах запрещены.

## Проверка выпуска

В каждом выпуске рядом с APK лежит `BLEAKFATE.apk.sha256`. Положите оба файла в одну папку и проверьте скачанный файл:

```
sha256sum -c BLEAKFATE.apk.sha256
```

Все выпуски подписаны одним ключом. С Android SDK `apksigner verify --print-certs BLEAKFATE.apk` должен показать этот отпечаток SHA-256 сертификата:

```
b6fa737b90b114ed4144ee2f0c7d00559fcbc81fbe890f59636d3142e93c51f8
```

Файл, подписанный другим ключом, — не наш: не устанавливайте его и напишите в бот поддержки, где вы его нашли.
