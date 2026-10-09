# SubsTrack 0.1.12

- Суммы ближайших платежей, списка на главной и выбранного дня пересчитываются в основную валюту. Если курса нет, показана исходная сумма с пояснением.
- Активные сессии доступны в Android и iOS. Исправлены отступы; блок сессий и удаление аккаунта свёрнуты по умолчанию.
- Дата следующего списания и период оплаты расположены рядом: ежемесячно в выбранный день, каждые 30 дней, другой интервал или ежегодно.
- Во всех выпадающих меню ровные SVG-стрелки без вращения и смещения.

Android 7.0+, прежняя подпись, APK без отладки. Устанавливайте поверх существующего приложения без удаления данных. Сайт обновлён; серверная база и пользовательские записи не заменялись.

Проверено: профильные автоматические тесты и адаптивные сценарии в обеих темах, Android lint и сборки Android/iOS; установка итогового APK поверх приложения на физическом Android, восстановление аккаунта; сессии и раскрытие меню в симуляторе iPhone. Все провайдеры входа, push, одновременное редактирование и физический iPhone повторно не проверены. iOS 0.1.12 подготовлена локально, в App Store/TestFlight не опубликована.

SHA-256: `0fe56d597f986b9725290adcd3211cd5757df8f819a801738b44ede830b8c516`

## English

Upcoming payments, Today rows and day agenda now use the selected display currency with an explicit missing-rate fallback. Android/iOS session management is available; session and account-deletion panels are collapsed by default with consistent spacing. Billing date and recurrence options are together, distinguishing monthly billing from every 30 days. Dropdown chevrons stay centered without rotating.

Same certificate, non-debuggable APK, Android 7.0+. Install over the existing app without clearing data. Website updated without replacing database records. Targeted automated checks, responsive light/dark flows, native builds, physical Android upgrade and iPhone simulator sessions/dropdowns verified. Provider login, push, concurrent edits and physical iPhone not fully re-tested. iOS 0.1.12 is local only, not published to App Store/TestFlight.

# SubsTrack 0.1.11

- Фактические расходы отделены от плана платежей; предоплата учитывается одной суммой по дате оплаты.
- Можно указать нестандартную сумму за один или несколько периодов без изменения обычного тарифа.
- Исправлено сохранение идентичности ожидающего платежа при переносе даты и учёт ранее оплаченных периодов.
- Календарь сразу показывает действия выбранного дня. Улучшены состояния ошибки оплаты и недоступной статистики.
- Исправлены формат редактируемой суммы, цвета ошибок и подложка статус-бара при прокрутке.

Android 7.0+, прежняя подпись, APK без отладки. Устанавливайте поверх существующего приложения без удаления данных. Выпуск требует обновлённого сервера SubsTrack.

Проверки: 44 браузерных сценария, 26 профильных frontend-тестов, 54 серверных теста в образе выпуска, Android lint и сборки Android/iOS. Полная повторная проверка всех провайдеров входа, push и одновременного редактирования с нескольких устройств в этот выпуск не входит. iOS в магазине не публикуется.

SHA-256: `64a699e5e86ebc26aa1dd65bc4d4658b57374ffa03b579591fa8b7c488506a3d`

## English

Actual cash expenses are separate from scheduled coverage. Custom single/multi-period payments do not reprice subscriptions. Pending payment identity survives date changes; existing paid coverage is respected. Calendar selection reveals day actions, payment failures retain the draft, and amount inputs, error styling and the native status-bar shield are corrected.

Same certificate, non-debuggable APK, Android 7.0+. Install over the existing app without clearing data. Requires the updated SubsTrack server. Automated release checks passed; all-provider login, push delivery and simultaneous cross-device editing were not fully re-tested. No iOS store publication.

# SubsTrack 0.1.10

- Исправлен откат выбранной темы при синхронизации: локальное изменение сохраняется до подтверждения сервером, в том числе при повторной загрузке.
- Сервер принимает системную тему; ранее эта настройка могла блокировать очередь следующих изменений. Исправление применено с резервными копиями, без замены данных пользователей.
- Временные сетевые ошибки повторяются ограниченно; отклонённые изменения сохраняются для диагностики, а не удаляются из очереди.
- Исправлена передача восстановленной сессии интерфейсу при недоступных cookies. Секрет продления остаётся в защищённом хранилище.
- Отключено журналирование содержимого нативных вызовов с данными сессии.

Android 7.0+. Прежняя подпись, сборка без отладки. Устанавливайте поверх приложения, не удаляя данные.

Проверено: восстановление очереди и сохранение светлой темы после подтверждения сервером и перезагрузки на физическом Android; установка итогового APK поверх приложения на телефоне и эмуляторе; профильные тесты, сборка и Android lint. Все провайдеры входа и push в этом выпуске повторно не проверены. Отображение конфликтов одновременного редактирования остаётся известным ограничением. iOS в магазин не публиковалась.

SHA-256: `3ffcba4f1aecb1fb01ce5aad318b70c1571ef05293541155e4de61059a4831ee`

## English

Fixes pending theme rollback during synchronization and reload. The server now accepts system theme without blocking later queued changes; existing data was preserved with backups. Transient network failures receive bounded retries, while rejected commands remain available for diagnostics. Native session restoration no longer depends solely on WebView cookies; refresh credentials remain in secure storage. Native bridge payload logging is disabled.

Same signing certificate, non-debuggable APK, Android 7.0+. Physical-device queue recovery and acknowledged light-theme persistence were verified; the final APK was installed over the app on a phone and emulator. Provider login and push were not all re-tested. Concurrent-edit conflict presentation remains a known limitation. No iOS store publication.

# SubsTrack 0.1.9

- Интерактивный календарь на главной: платежи выбранного дня, переход к подписке, оплата, предоплата и пропуск.
- Исправлены наложения в узком календаре, выпадающие меню, фокус форм и навигация в горизонтальном положении.
- Предпросмотр фона иконки; асинхронная загрузка иконок не затирает новые правки формы.
- Единое управление цветом системных панелей Android, включая возврат из фона.
- Светлый/тёмный брендированный экран запуска с оригинальным знаком SubsTrack.
- Экспорт JSON через системное меню сохранения/отправки файла в приложении.
- Общий интерфейс обновлён на substrack.top. Без миграций БД и замены данных пользователей.

Android 7.0+. Подпись совпадает с публичной 0.1.8; устанавливайте поверх приложения без удаления данных. Сборка без отладки.

Проверено: 30 браузерных сценариев, профильные автоматические тесты, Android lint, сборка, подпись и установка/запуск на эмуляторе. Входы провайдеров и push на реальном устройстве повторно не проверены. Известное ограничение отображения конфликтов одновременного редактирования сохраняется. iOS в магазины не публиковалась.

SHA-256: `5d5ede5f2107b090c8101675c1a463a82da7db3e291faf713d5c607923c04919`

## English

Interactive Today calendar with daily payment actions; layout, menus, draft editing and icon-background previews improved. Android system-bar theming, branded startup and native JSON export improved. Shared web UI also updated, without database migrations or user-data replacement. Same signing certificate as public 0.1.8, non-debuggable sideload APK; install without clearing data. Browser tests and emulator installation/launch passed. Real-device provider login and push delivery were not re-verified; the simultaneous-edit conflict UX limitation remains. No iOS store release.

# SubsTrack 0.1.8

- Эти же исправления опубликованы на substrack.top 5 сентября 2026 г.; обновлять APK повторно после установки 0.1.8 не нужно.
- Исправлена ошибка сохранения подписок после обновления старой установки: локальная база и идентификатор устройства теперь переносятся согласованно, без очистки данных.
- Исправлено получение изменений даты оплаты с других устройств.
- Обновление с 0.1.7, сохранение даты на сервере и сохранность результата после перезапуска проверены на физическом Android-устройстве.
- Известное ограничение: конфликт одновременных изменений между устройствами пока недостаточно явно показывается в форме; после обновления данных может потребоваться повторить изменение.

Android 7.0+. Устанавливайте поверх предыдущей версии, не удаляя приложение. Подпись прежняя; сборка без отладки.

SHA-256: `b172d93993413b42ca4ed11ba38f55e2c1c70717998b616c2b18daa72bd4513d`

## English

The same fixes were deployed to substrack.top on September 5, 2026. If 0.1.8 is already installed, no replacement APK is needed.

Fixes subscription saving after upgrading older installations by migrating the local database and recovering the matching device identity without clearing data. Billing-date changes from other devices are now accepted. Upgrade from 0.1.7, server persistence and a full app restart were verified on a physical Android device. Install over the previous version; Android 7.0+ and the existing signing certificate are retained. This is a non-debuggable build.

Known limitation: simultaneous-edit conflicts are not yet clearly surfaced in the editor; after synchronization, an edit may need to be retried.

# SubsTrack 0.1.7

- Плашки оплаты, пропуска, отмены и ошибки автоматически исчезают через 6 секунд.
- Новое уведомление получает собственный отсчёт, даже если текст повторяется.
- Скрытие плашки не изменяет платёж; отмена через историю действий остаётся доступной.
- Временная кнопка «Отменить» больше не перехватывает фокус автоматически.

Android 7.0+. Обновление поверх 0.1.4–0.1.6 с сохранением прежней подписи.

SHA-256: `2d52a42b1c764de31c626cad8cd801a0a60f2d9fce40d215eb25694f59199734`

# SubsTrack 0.1.6

- Исправлена ложная ошибка обязательных полей при сбое сохранения подписки.
- Список обновляется после принятия записи в очередь синхронизации.
- При ошибке черновик остаётся в форме для повторной попытки.
- Повторное нажатие во время сохранения не создаёт дублирующую запись.

Android 7.0+. Обновление поверх 0.1.4 и 0.1.5 с сохранением прежней подписи.

SHA-256: `95b129c463d33a148045a6bfdd1bf4d6c73fd7b5cbd41e47f4ac9f9ec52b5eaa`

# SubsTrack 0.1.5

Первый публичный APK-релиз SubsTrack в отдельном репозитории сборок.

## Что входит

- единый интерфейс веб-версии и Android-приложения;
- главный экран со статусами платежей за месяц;
- календарь, список подписок, аналитика и настройки;
- поддержка нескольких аккаунтов одного сервиса;
- категории, заметки, домены и автоматические иконки;
- основная валюта и пересчёт платежей;
- предоплата на несколько периодов с отдельной акционной суммой;
- push- и Telegram-напоминания;
- вход через Google, GitHub и Telegram;
- светлая и тёмная темы, русский и английский языки.

## Установка

Скачайте `SubsTrack-0.1.5-sideload.apk`. Требуется Android 7.0 или новее. Сборка имеет тот же сертификат, что и 0.1.4, поэтому устанавливается поверх неё без удаления приложения.

SHA-256: `aca5ab3801b8596212a2bb7fbe497b2ea58107c5169083b0ab4d653042da7040`

Скриншоты в репозитории созданы на демонстрационных данных.
