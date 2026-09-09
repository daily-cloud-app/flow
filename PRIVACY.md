# Privacy Policy — Daily Life Flow

- [English](#english)
- [日本語](#日本語)

---

## English

Last updated: September 5, 2026

### 1. Introduction

Daily Life Flow ("the App") is a personal schedule and task management application.

By default, the data you enter is stored only on your device. The App uses no advertising SDKs and no analytics SDKs, and does not collect your name, address, phone number, date of birth, or location.

Some features (Calendar integration and Shared Tags) are **optional and disabled by default**. They communicate externally only after you explicitly enable them.

> **Beta notice**: The Calendar integration and Shared Tags features are currently provided as a beta. Their behavior may change, and support for them may be discontinued without prior notice.

### 2. Information We Collect

#### Information Stored on Device

| Data | Purpose |
|------|---------|
| Event & task details (title, date/time, notes, all-day flag) | Core schedule management |
| Recurrence rules & reminder settings | Repeating events and notifications |
| Tags with colors and order | Organization & filtering |
| Completion status | Task tracking |
| App settings (theme, default start time, week start day, display format) | App configuration |
| Linked account display info (email address, display name) | Account identification for calendar integration |

All local data is stored in the app's private storage area on the device. Uninstalling the App removes this data from your device.

#### Information Handled by Optional Features

| Data | Feature | Destination |
|------|---------|-------------|
| Anonymous identifier (UID) | Shared Tags | Firebase (Google) |
| Shared tag name, color, and membership information | Shared Tags | Firebase (Google) |
| Shared events (title, date/time, notes, all-day flag, recurrence, reminder minutes, and completion status) | Shared Tags | Firebase (Google) |
| Invite codes, membership, creator/editor UID, and timestamps required for synchronization | Shared Tags | Firebase (Google) |
| App, device, and integrity information required for abuse prevention | Shared Tags / Firebase App Check | Firebase and Google Play Integrity |
| External calendar events (read-only) | Calendar integration | Displayed on device only |

### 3. Information We Do Not Collect

- Location (GPS)
- Contacts
- Camera or microphone
- Photos / media library
- Advertising ID
- Analytics data
- Crash reports
- Hardware identifiers such as IMEI or MAC address
- Cookies

No analytics SDK (Firebase Analytics, Google Analytics, etc.) or crash reporting SDK (Crashlytics, etc.) is included.

To protect the Shared Tags backend against abuse, Firebase App Check and Google Play Integrity may process app information, device information, and integrity tokens. These are used only for security and abuse prevention, and not for advertising, marketing, analytics, or cross-app tracking.

### 4. Reminders (Notifications)

The App uses on-device local notifications to remind you before events start. Notification content is never sent to any external server. On Android 13 and later, notification permission is required to show notifications; all other features remain available if you decline it.

### 5. Calendar Integration (Optional, disabled by default, Beta)

This feature is **disabled by default** and is currently provided as a **beta**; support may be discontinued without prior notice. It operates only after you accept the terms and explicitly enable it in settings, and link an account. When enabled, the App fetches your external calendar events in **read-only** mode and displays them on your device. Currently, Google Calendar (on Android) is supported; additional calendar providers may be added in the future.

- The integration can be enabled or disabled at any time in settings.
- Linking uses the device's account mechanism (for Google Calendar on Android, the AccountManager); the App does not store authentication tokens.
- Fetched events are used only for on-device display and are not sent or stored externally.
- The linked account's email address and display name are stored on your device for identification.
- You can unlink an account at any time, which removes the corresponding account information from your device.

### 6. Shared Tags Feature (Optional, disabled by default, Beta)

The "Shared Tags" feature, which lets multiple users share schedules, is **disabled by default** and is currently provided as a **beta**; support may be discontinued without prior notice. It operates only after you accept the terms and explicitly enable it in settings. No communication with the cloud service occurs until then.

When enabled, this feature uses Google [Firebase](https://firebase.google.com/support/privacy) (Cloud Firestore / Firebase Authentication / Firebase App Check).

- **Anonymous authentication**: A non-identifying anonymous identifier (UID) is issued. No name or email is requested.
- **Data stored in the cloud**: Shared tag names and colors, events under a shared tag, recurrence and reminder settings, occurrence-level completion status, anonymous UIDs of members, invite codes, creator/editor UIDs, and timestamps required for synchronization.
- **Data not sent to the cloud**: Your private (non-shared) events and events fetched from an external calendar.
- **Invite codes**: You share invite codes yourself through your OS share sheet (email, messaging apps, etc.). They are not sent to any analytics service or logs.

All communication is encrypted via HTTPS (TLS).

### 7. Permissions

| Permission | Purpose |
|------------|---------|
| `INTERNET` | Cloud sync when Shared Tags is enabled |
| `POST_NOTIFICATIONS` (Android 13+) | Show reminder notifications |
| `RECEIVE_BOOT_COMPLETED` | Reschedule reminders after device restart |

The App does not request access to location, contacts, camera, microphone, or photos.

### 8. Third-Party Sharing

The App does not provide, sell, or share user data with third parties for advertising or marketing.

When you use the Shared Tags feature, Google (Firebase) is used as the cloud backend, and the handling of information there is governed by Google's privacy policy.

### 9. Data Deletion

- **Local data**: Uninstalling the App removes all on-device data.
- **Unlink account**: Removes the linked calendar account information from the device.
- **Leave sharing**: A member can leave a shared tag. This removes the membership and local shared cache, while the shared group's data may remain for its owner and other members.
- **End sharing as owner**: The owner can stop synchronization and keep the events as local data. Ending sharing is not necessarily the same as immediately deleting every cloud record.
- **Delete anonymous account**: The App deletes cloud data owned by the anonymous UID, removes memberships, and then deletes the anonymous account. If the process is interrupted, the App retains the pending deletion state locally and retries when possible.

### 10. Security

- All external communication is encrypted via HTTPS (TLS)
- Firebase App Check is used to help protect backend access
- Local data is stored in the app's private storage area on the device

### 11. Children

The App is not intended for users under 13 years of age.

### 12. Disclaimer

The App may be modified or discontinued without notice for improvements or bug fixes. The Calendar integration and Shared Tags features are provided as a beta and may be changed or discontinued without prior notice. The developer is not liable for damages arising from use of the App, including data loss or sync failures.

### 13. Changes to This Policy

This policy may be updated as needed. Significant changes will be communicated through app updates.

### 14. Contact

- GitHub: https://github.com/daily-cloud-app/flow/issues

---

## 日本語

最終更新日: 2026年9月5日

### 1. はじめに

Daily Life Flow（以下「本アプリ」）は、予定とタスクを管理するためのアプリケーションです。

入力したデータは既定では端末内にのみ保存されます。本アプリは広告 SDK およびアナリティクス SDK を一切使用せず、氏名・住所・電話番号・生年月日・位置情報を収集しません。

一部の機能（カレンダー連携および共有タグ）は**任意であり、初期状態では無効**です。利用者が明示的に有効化した場合にのみ外部と通信します。

> **ベータ版に関する注意**: カレンダー連携および共有タグ機能は、現在ベータ版として提供しています。動作が変更される場合があり、また予告なくサポートを終了する場合があります。

### 2. 収集する情報

#### 端末内に保存する情報

| データ | 目的 |
|--------|------|
| 予定・タスクの内容（タイトル、日時、メモ、終日フラグ） | 予定管理の基本機能 |
| 繰り返しルール・通知（リマインダー）設定 | 繰り返し予定と通知 |
| タグおよびその色・並び順 | 整理・フィルタリング |
| 完了状態 | タスクの進捗管理 |
| アプリ設定（テーマ、既定の開始時刻、週の開始曜日、表示形式） | アプリの設定 |
| 連携アカウントの表示情報（メールアドレス、表示名） | カレンダー連携時のアカウント識別 |

これらはすべて端末内のアプリ専用領域に保存されます。アプリを削除（アンインストール）すると端末から消去されます。

#### 任意機能で扱う情報

| データ | 機能 | 送信先 |
|--------|------|--------|
| 匿名識別子（UID） | 共有タグ | Firebase（Google） |
| 共有タグの名前・色・メンバー情報 | 共有タグ | Firebase（Google） |
| 共有された予定（タイトル、日時、メモ、終日フラグ、繰り返し、通知分数、完了状態） | 共有タグ | Firebase（Google） |
| 招待コード、メンバーシップ、作成者・更新者 UID、同期に必要な更新日時 | 共有タグ | Firebase（Google） |
| 不正利用防止に必要なアプリ・端末・完全性情報 | 共有タグ／Firebase App Check | Firebase および Google Play Integrity |
| 外部カレンダーの予定（読み取り専用） | カレンダー連携 | 端末内での表示のみ |

### 3. 収集しない情報

- 位置情報（GPS）
- 連絡先
- カメラ・マイク
- 写真・メディアライブラリ
- 広告ID
- アナリティクスデータ
- クラッシュレポート
- IMEI、MACアドレス等のハードウェア識別子
- Cookie

本アプリにはアナリティクス SDK およびクラッシュレポート SDK は組み込まれていません。

共有タグ用バックエンドの不正利用防止およびセキュリティ保護のため、Firebase App Check および Google Play Integrity がアプリ情報、端末情報および完全性トークンを処理する場合があります。これらは広告、マーケティング、利用状況分析またはアプリ横断の追跡には使用しません。

### 4. 通知（リマインダー）

本アプリは端末内で完結するローカル通知を使用し、予定の開始前にリマインダーを表示します。通知の内容が外部サーバーへ送信されることはありません。Android 13 以降では通知の表示に通知権限が必要ですが、許可しなくても通知以外の機能は利用できます。

### 5. カレンダー連携（任意・初期状態は無効・ベータ版）

本機能は**初期状態では無効**であり、現在**ベータ版**として提供しています（予告なくサポートを終了する場合があります）。設定画面で利用条件に同意して明示的に有効化し、アカウントを連携した場合に限り、本アプリは連携した外部カレンダーの予定を**読み取り専用**で取得し、端末内で表示します。現時点では Google カレンダー（Android）に対応しており、今後、対応するカレンダーサービスを追加する場合があります。

- 連携は設定画面からいつでも有効・無効を切り替えられます。
- 連携は端末のアカウント機能（Google カレンダーの場合は Android の AccountManager）を通じて行われ、認証トークンをアプリ内に保存しません。
- 取得した予定は端末内での表示にのみ使用し、外部へ送信・保存しません。
- 連携アカウントのメールアドレスと表示名は、識別のために端末内に保存されます。
- 連携はいつでも解除でき、解除すると対応するアカウント情報は端末から削除されます。

### 6. 共有タグ機能（任意・初期状態は無効・ベータ版）

複数の利用者で予定を共有する「共有タグ」機能は、**初期状態では無効**であり、現在**ベータ版**として提供しています（予告なくサポートを終了する場合があります）。設定画面で利用条件に同意し、明示的に有効化した場合にのみ動作します。有効化するまで、クラウドサービスへの通信は一切行いません。

有効化した場合、本機能は Google の [Firebase](https://firebase.google.com/support/privacy)（Cloud Firestore / Firebase Authentication / Firebase App Check）を利用します。

- **匿名認証**: 個人を特定しない匿名の識別子（UID）が発行されます。氏名・メールアドレス等は要求しません。
- **クラウドへ保存される情報**: 共有タグの名前・色、タグ配下の予定、繰り返し・通知設定、発生回ごとの完了状態、共有メンバーの匿名 UID、招待コード、作成者・更新者 UID、および同期に必要な更新日時。
- **クラウドへ送信されない情報**: 共有していない個人の予定、外部カレンダーから取得した予定。
- **招待コード**: 共有への招待コードは OS の共有機能（メール、メッセージアプリ等）を通じて利用者自身が送信します。解析サービスやログへ送られることはありません。

すべての通信は HTTPS（TLS）で暗号化されます。

### 7. 権限

| 権限 | 用途 |
|------|------|
| `INTERNET` | 共有タグ機能を有効化した場合のクラウド同期 |
| `POST_NOTIFICATIONS`（Android 13以降） | リマインダー通知の表示 |
| `RECEIVE_BOOT_COMPLETED` | 端末再起動後の通知の再設定 |

本アプリは、位置情報、連絡先、カメラ、マイク、写真へのアクセス権限を要求しません。

### 8. 第三者への提供

本アプリはユーザーデータを広告・マーケティング目的で第三者に提供、販売、共有しません。

共有タグ機能を利用する場合のクラウド基盤として Google（Firebase）を利用し、そこでの情報の取り扱いは Google のプライバシーポリシーに従います。

### 9. データの削除

- **ローカルデータ**: アプリを削除すると端末内の全データが消去されます。
- **連携解除**: 連携したカレンダーアカウント情報が端末から削除されます。
- **共有からの退出**: 参加者は共有タグから退出できます。自分のメンバー情報と端末内の共有キャッシュが削除されますが、共有グループのデータは所有者や他のメンバーのために残る場合があります。
- **所有者による共有終了**: 所有者は同期を停止し、予定をローカルデータとして残すことができます。共有終了は、クラウド上のすべての記録を直ちに完全削除する操作と同一とは限りません。
- **匿名アカウントの削除**: 本アプリは匿名 UID が所有するクラウドデータを削除し、メンバー情報を削除したうえで匿名アカウントを削除します。処理が中断された場合は、未完了状態を端末内に保持し、可能になった時点で再試行します。

### 10. セキュリティ

- すべての外部通信は HTTPS（TLS）で暗号化されています
- バックエンドへのアクセス保護のため Firebase App Check を使用しています
- ローカルデータは端末内のアプリ専用領域に保存されます

### 11. 子どもの利用

本アプリは13歳未満の方を対象としておらず、13歳未満の方の利用は想定していません。

### 12. 免責事項

本アプリは機能改善や不具合修正のため、予告なく仕様変更や提供停止を行う場合があります。カレンダー連携および共有タグ機能はベータ版として提供しており、予告なく変更または提供停止する場合があります。開発者は、データの消失や同期の失敗を含め、本アプリの利用に起因する損害について責任を負いません。

### 13. 本ポリシーの変更

本ポリシーは必要に応じて更新される場合があります。重要な変更がある場合はアプリのアップデート時にお知らせします。

### 14. お問い合わせ

- GitHub: https://github.com/daily-cloud-app/flow/issues
