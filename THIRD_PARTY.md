# Third-party components / Сторонние компоненты

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
