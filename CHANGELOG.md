# LazilyFAX Changelog

## v2.0.0 — 2026-11-01

Final release baseline. Product version: `2.0.0`; Debian package version: `2.0.0-10` (amd64).

### Included

- FAX sending and receiving, with received PDF viewing
- Phonebook, sent/received history, FAX preview, and sender header settings
- Answering machine, greeting audio, and recorded message management
- Backup and restore
- English, Japanese, Korean, and German interfaces and PDF manuals

### Final Packaging

- Preserved application files, modem binary, audio, public verification keys, and manuals from the hardware-tested final-test package; no new application features were introduced during final packaging.
- Normalized package file permissions and updated release documentation.
- Set Debian package revision to 2.0.0-10 so pre-sale revisions 2.0.0-1 through 2.0.0-9 can update normally.
- Included installation/removal guidance, third-party notices, credits, and the corresponding efax source.
- Removal and purge retain user settings and data; no data purge is required to migrate to the final release.

### Validation

- User hardware testing: FAX sending, two-page reception, received PDF display, and answering machine stability when the remote party encounters an error.
- Successful reception reported with `+FHNG:000` and `efax-wire returning 0`.
- 33 existing simulated tests passed.
- Isolated installation, update, removal, purge, reinstallation, and synthetic data preservation checks passed.
- Repeated DEB builds matched; the included efax source also rebuilt to the packaged binary hash.
- Clean-OS dependency installation, normal-user administrator authentication, long-duration operation, and all modem/line combinations remain unverified. See the distribution validation report for further limitations.

### Distribution and Updates

- Purchaser distribution: ZIP containing the DEB and four-language manuals.
- Reference test environment: Linux Mint 22.3 / Ubuntu 24.04 base, amd64.
- This public repository provides update information and documentation, not the complete product.
- Version 2.0.0 / package 2.0.0-10 is the official release baseline.
- Automatic update offers are disabled until a compatible delta update is published. Install this release from the purchaser ZIP.
- Earlier duplicated roadmap entries for v1.2.0 have been retired; GitHub update checking is included in the current product.

### 日本語

LazilyFAX 2.0.0の正式販売版です。DEB内部管理番号は2.0.0-10です。

FAX送受信、PDF表示、電話帳、送受信履歴、送信ヘッダー、留守番電話、バックアップ・復元を収録し、英日韓独の画面とマニュアルに対応しています。販売用の最終梱包では実機確認済みテスト版のアプリ処理を変更していません。

ユーザー実機で送信・2ページ受信・PDF表示・相手側エラー時の留守番電話の安定性を確認しています。クリーンOSでの導入や長時間運用などの未確認項目は、販売ZIP内の検証報告に記載しています。

正式版を今後の更新の基準とします。正式版への差分更新は未公開のため自動更新案内は無効です。販売ZIPから導入してください。移行のために利用者の設定・送受信データを消去する必要はありません。

---

## Earlier Release History

The entries below preserve the previously published release history.

## v1.1.0

### Added

- Korean language support
- Korean interface for FAX Phonebook
- Korean interface for FAX Transmission History

### Changed

- Added Korean language selection support

## v1.0.0

Initial release.

### Features

- PDF FAX sending
- FAX phonebook
- FAX transmission history
- FAX preview
- Header settings
- Language settings
- Japanese interface
- English interface
- Setup check
- Multi-user installation support

### Platform

- Linux
- Developed and tested primarily on Linux Mint

### Notes

- A compatible USB FAX modem is required for FAX transmission.
- Product files are not distributed from this public repository.
- This repository is used for update information, documentation, known issues, and support.
