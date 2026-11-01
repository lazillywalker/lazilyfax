# LazilyFAX

LazilyFAX is a desktop FAX sending, receiving, and answering machine application for Linux.

This repository provides official update information, documentation, known issues, and support information. The complete product is distributed separately to purchasers.

## Current Version

**LazilyFAX 2.0.0 — final release (2026-11-01)**

- Product version: `2.0.0`
- Debian package version: `2.0.0-10`
- Architecture: `amd64`
- Interface and PDF manuals: English, Japanese, Korean, and German

## Features

- Send PDF documents by FAX
- Receive FAX documents and view received PDFs
- FAX phonebook and sent/received history
- FAX preview and sender header settings
- Answering machine, greeting audio, and recorded message management
- Backup and restore
- Four-language interface and manuals

## Supported Environment

Ubuntu-based distributions using Ubuntu 24.04 or later as their base, on amd64.
The reference test environment is Linux Mint 22.3 (Ubuntu 24.04 base).

A compatible USB FAX modem and telephone line are required.
FAX and voice capabilities depend on the modem and line; operation on every configuration is not guaranteed.

## Distribution and Installation

Purchasers receive a ZIP containing the DEB installer, four-language PDF manuals, installation/removal instructions, and third-party notices and corresponding source where applicable.

Stop FAX and answering machine activity, close the application, and back up application data and voicemail recordings before installation or update. Follow the instructions included in the ZIP.

The complete product is not distributed from this public repository.

## Updates

The official release metadata is in [version.json](version.json).
Version 2.0.0 / package 2.0.0-10 is the current release baseline.

Automatic update offers are currently disabled because no delta update to this release is published. Install the final release using the purchaser distribution ZIP. Future delta updates will be announced when available.

See [CHANGELOG.md](CHANGELOG.md) for release notes.

## Validation

User hardware testing confirmed FAX sending, two-page reception, received PDF display, and answering machine stability when the remote party encounters an error. Successful reception was reported with `+FHNG:000` and `efax-wire returning 0`.

Package checks included 33 simulated tests, isolated installation/update/removal and data preservation, and reproducible package rebuilding. Clean-OS dependency installation, normal-user administrator authentication, and long-duration operation remain unverified. See the validation report included in the distribution for the full scope and limitations.

## Support

Bug reports and known issues are managed through this repository.
For purchaser support, use Settings → Support in the application or the contact facility at the point of purchase.

Support covers the application itself. Configuration assistance for third-party modems and telephone lines is outside the support scope. See the included support information for details.

---

# LazilyFAX 日本語案内

LazilyFAXは、Linux向けのFAX送受信・留守番電話アプリケーションです。

**現在の正式版は2.0.0（2026年11月1日）、DEB内部管理番号は2.0.0-10です。**
英語・日本語・韓国語・ドイツ語の画面とPDFマニュアルに対応しています。

購入者向けの販売ZIPに、DEB、4言語マニュアル、導入・削除案内、第三者ライセンス資料等を同梱しています。製品本体はこの公開リポジトリでは配布しません。

対象はUbuntu 24.04以降をベースとするUbuntu系ディストリビューションのamd64環境です。基準の実機確認環境はLinux Mint 22.3です。対応USB FAXモデムと電話回線が必要です。

送信、2ページ受信、PDF表示、相手側エラー時の留守番電話の安定性をユーザー実機で確認しています。確認範囲と未確認項目は配布ZIPの検証報告をご参照ください。

正式版への差分更新はまだ公開していないため、自動更新案内は無効です。正式版は販売ZIPから導入してください。更新前には通信・待受・アプリを終了し、アプリデータと録音をバックアップしてください。旧版からの移行で利用者データを消去する必要はありません。

購入者向けのお問い合わせは、アプリの「設定 → サポート」または購入先の問い合わせ機能をご利用ください。
