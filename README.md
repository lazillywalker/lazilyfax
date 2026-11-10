# LazilyFAX

LazilyFAX is a desktop FAX sending, receiving, and answering machine application for Linux.

This repository provides official update information, documentation, known issues, and support information. The complete product is distributed separately to purchasers.

## Current Version

**LazilyFAX 2.0.0 — Gumroad edition (2026-11-10)**

- Product version: `2.0.0`
- Debian package version: `2.0.0-19`
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

The complete product is available from [Gumroad](https://lazilywalker.gumroad.com/l/lazilyfax-linux) and is not distributed from this public repository.

## Updates

The official release metadata is in [version.json](version.json).
The current package is `2.0.0-19`. Updates are enabled from `2.0.0-18` and the development build `2.0.0-19~gumroad1`. Earlier packages require the complete DEB from the purchaser distribution ZIP.

Register your purchase email and Gumroad license key in Settings → License registration. Updates in the Gumroad edition verify purchase status online; invalid, revoked or refunded purchases cannot authorize updates. FAX and answering machine functions remain available without this update registration. Save registration separately using Backup and Restore.

The initial migration from package 2.0.0-18 uses its existing updater; purchase verification applies to subsequent updates in the Gumroad edition.

See [CHANGELOG.md](CHANGELOG.md) for release notes.

## Validation

User hardware testing confirmed FAX sending, two-page reception, received PDF display, and answering machine stability when the remote party encounters an error. Successful reception was reported with `+FHNG:000` and `efax-wire returning 0`.

The Gumroad license checks passed 45 automated tests. Test-purchase verification, license disabling and re-enabling were also confirmed against the live API. Delta rebuilding was checked from both supported base versions. Isolated installation/update checks and user-reported FAX and answering machine operation were also completed.

## Support

Bug reports and known issues are managed through this repository.
For purchaser support, use Settings → Support in the application or the contact facility at the point of purchase.

Support covers the application itself. Configuration assistance for third-party modems and telephone lines is outside the support scope. See the included support information for details.

---

# LazilyFAX 日本語案内

LazilyFAXは、Linux向けのFAX送受信・留守番電話アプリケーションです。

**現在の製品版は2.0.0 Gumroad版（2026年11月10日）、DEB内部管理番号は2.0.0-19です。**
英語・日本語・韓国語・ドイツ語の画面とPDFマニュアルに対応しています。

購入者向けの販売ZIPに、DEB、4言語マニュアル、導入・削除案内、第三者ライセンス資料等を同梱しています。製品本体は[Gumroad](https://lazilywalker.gumroad.com/l/lazilyfax-linux)で販売し、この公開リポジトリでは配布しません。

対象はUbuntu 24.04以降をベースとするUbuntu系ディストリビューションのamd64環境です。基準の実機確認環境はLinux Mint 22.3です。対応USB FAXモデムと電話回線が必要です。

送信、2ページ受信、PDF表示、相手側エラー時の留守番電話の安定性をユーザー実機で確認しています。確認範囲と未確認項目は配布ZIPの検証報告をご参照ください。

2.0.0-18および開発版2.0.0-19~gumroad1から、2.0.0-19への更新を有効にしています。それ以前の版は販売ZIP内の完全DEBから導入してください。更新前には通信・待受・アプリを終了し、アプリデータと録音をバックアップしてください。旧版からの移行で利用者データを消去する必要はありません。

Gumroad版で更新を利用するには「設定 → ライセンス登録」で購入メールとライセンスキーを登録します。更新時に購入状態を照合し、無効・取消・返金済みの購入は更新できません。FAX送受信・留守番電話には、この更新用の登録判定を適用していません。登録情報はFAXデータとは別にバックアップしてください。旧版18からの初回移行は従来の更新処理を使い、移行後の更新に購入照合が適用されます。

購入者向けのお問い合わせは、アプリの「設定 → サポート」または購入先の問い合わせ機能をご利用ください。
