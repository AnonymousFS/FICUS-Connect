# Privacy / Конфиденциальность

## English

This describes the current Windows and Android betas' behavior, not a claim that every network path has passed an independent security audit.

- The installer does not copy the developer's user vault, subscription URLs, server credentials, session files or logs. Published screenshots use synthetic demo data.
- Windows protects saved subscriptions and settings with DPAPI for the current Windows user. An encrypted backup is intended for that same user context. Do not publish or share it casually.
- Android stores private subscription/settings data in platform secure storage. Android cloud backup is disabled. The APK contains no preconfigured subscription or developer account. Android diagnostics use fixed error codes; redact any additional connection details before sharing a report.
- Adding/refreshing a subscription contacts the provider URL you chose. If enabled, the HWID option includes a locally generated installation identifier in subscription requests; it is not the Windows MachineGuid. DNS, latency tests and proxy connections contact their configured endpoints. Public routing-profile import may contact GitHub.
- Copying a link, displaying a QR and saving its PNG are local actions. The person receiving the resulting data receives the associated connection access.
- TV transfers start only when you press **Send to TV**. INCY uses `check.incytv.com` with client-side CPace / ChaCha20-Poly1305 encryption. HAPP Web Import uses `check.happ.su` and can read the Base64-encoded subscription/server link. Base64 is not encryption. The selected destination is displayed before sending.
- Donation and support actions open external pages in your browser. Their operators' privacy practices apply there.
- Core logs may contain endpoint names or other connection metadata. Review and redact them before reporting a bug.
- TUN / Kill Switch are experimental. This beta does not promise complete leak protection.

## Русский

Здесь описано поведение текущих бет для Windows и Android. Это не заявление о независимом аудите всех сетевых сценариев.

- Установщик не копирует пользовательское хранилище разработчика, ссылки подписок, реквизиты серверов, файлы сеансов и логи. В публичных скриншотах используются вымышленные демонстрационные данные.
- Сохранённые подписки и настройки защищены Windows DPAPI для текущего пользователя. Зашифрованная резервная копия рассчитана на тот же контекст Windows. Не публикуйте её и не передавайте без необходимости.
- На Android приватные данные подписок/настроек сохраняются в защищённом хранилище платформы. Облачное резервное копирование Android отключено. APK не содержит готовой подписки или учётной записи разработчика. Диагностика Android использует фиксированные коды ошибок; очищайте дополнительные сведения о подключении перед отправкой отчёта.
- Добавление/обновление подписки обращается к выбранному вами провайдеру. При включённом HWID в запрос добавляется случайно созданный идентификатор установки, а не Windows MachineGuid. DNS, тесты задержки и прокси-подключения обращаются к своим настроенным адресам. Импорт публичного профиля маршрутизации может обращаться к GitHub.
- Копирование ссылки, показ QR и сохранение PNG выполняются локально. Получатель этих данных получает соответствующий доступ к подключению.
- Передача на ТВ начинается только после нажатия **«Отправить на ТВ»**. INCY использует `check.incytv.com` с шифрованием CPace / ChaCha20-Poly1305 на клиенте. HAPP Web Import использует `check.happ.su` и может прочитать ссылку подписки/сервера в Base64. Base64 — не шифрование. Получатель указан до отправки.
- Донат и поддержка открывают внешние страницы в браузере. Там действуют правила соответствующих сервисов.
- Логи ядер могут содержать имена узлов и другие сведения о соединении. Проверяйте и очищайте их перед публикацией отчётов.
- TUN / Kill Switch экспериментальны. Бета не гарантирует полную защиту от утечек.
