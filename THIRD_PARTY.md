# Third-party components / Сторонние компоненты

## Windows 0.9.8 beta

| Component | Included version | Upstream / license |
| --- | --- | --- |
| Xray-core | 26.10.21 | [Source](https://github.com/XTLS/Xray-core/tree/v26.10.21) · MPL-2.0 |
| sing-box | 1.14.4 | [Source](https://github.com/SagerNet/sing-box/tree/v1.14.4) · GPL-3.0-or-later |
| libcronet | From the same official sing-box release | [cronet-go](https://github.com/SagerNet/cronet-go) · [Chromium notices](https://chromium.googlesource.com/chromium/src/+/main/LICENSE) |
| GeoIP / GeoSite data | From the official Xray archive | [GeoIP](https://github.com/v2fly/geoip) · [Domain list](https://github.com/v2fly/domain-list-community) |
| Flutter / Dart and packages | See bundled license registry | `data/flutter_assets/NOTICES.Z` |
| Microsoft Visual C++ Runtime | App-local x64 redistributables | Microsoft redistribution terms |

The installed `licenses` directory contains upstream license texts, source
archives for the included Xray/sing-box versions, component URLs and archive
checksums. The upstream executables are separate processes and have not been
modified. Their licenses and rights are not replaced by FICUS distribution notes.

В установленном каталоге `licenses` находятся лицензии, архивы публичных исходников
включённых версий Xray/sing-box, ссылки на компоненты и контрольные суммы архивов.
Ядра выполняются отдельными процессами и не модифицированы. Условия FICUS не
заменяют лицензии и права на сторонние компоненты.

The application also includes a readable PowerShell TUN lifecycle helper.
The public repository does not include the FICUS Flutter/C++ source tree.

Программа также содержит читаемый служебный PowerShell-скрипт управления TUN.
Полное дерево Flutter/C++-исходников FICUS в этом репозитории не публикуется.

## Android 0.9.8 beta

| Component | Included version | Source / license |
| --- | --- | --- |
| Xray protected-socket core | 26.10.31-protect2 | [SDK source, core patches and build instructions](https://github.com/XIIIFOX/flutter_vless/tree/291714fcf1964183d5d6891ff7c24a631af8e343) · [upstream core](https://github.com/XTLS/Xray-core/tree/v26.10.31) · MPL-2.0 core, MIT SDK |
| Separate sing-box IPC runtime | 1.14.4 | [Corresponding runtime source archive and build instructions](https://github.com/AnonymousFS/FICUS-Connect/releases/download/v0.9.4-beta/FICUS-Android-Runtime-Sources-0.9.4.tar.gz) · GPL-3.0-or-later |
| Cronet / Chromium | Pinned by runtime go.mod/go.sum | [cronet-go source/build provenance](https://github.com/SagerNet/cronet-go) · upstream licenses/notices retained in the runtime archive |
| Flutter / Dart and packages | See bundled registry | `assets/flutter_assets/NOTICES.Z` |

The Android runtime source archive contains the separate Go IPC executable,
vendored Go dependencies, the ARM64 Cronet static library, module source URLs,
license texts and a build script. Other architectures' prebuilt libraries are
omitted and listed. Native Cronet/Chromium build sources are referenced through
the pinned upstream modules; their complete native tree is not vendored here.
Xray's independent SDK/core sources are available at the pinned links above.
These are third-party/runtime sources; the FICUS Flutter/Kotlin/C++ application
source and signing material remain private. Component licenses retain their own rights.

Android-архив содержит исходники отдельного Go runtime, Go-зависимости, статическую
ARM64-библиотеку Cronet, ссылки на исходники модулей, лицензии и скрипт сборки.
Готовые библиотеки других архитектур исключены и перечислены отдельно. Для нативных
исходников Cronet/Chromium указаны привязанные к версиям upstream-модули; полное
дерево Chromium в архив не включено. Исходники независимого Xray SDK/ядра доступны
по указанным выше ссылкам. Код приложения FICUS и ключи подписи остаются закрытыми.
