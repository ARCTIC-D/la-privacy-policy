# 百变谱面 隐私政策

**生效日期：** 2026-07-14

---

## 1. 概述

一款在 **您的设备本地** 完成人脸检测与换脸处理的应用。我们高度重视您的隐私，本政策说明我们如何处理与您相关的信息。

**核心原则：您的所有照片、视频与人脸数据均在设备本地处理，我们不会将其上传到任何服务器，也不会存储或转发给任何第三方。**

---

## 2. 我们收集的信息

### 2.1 我们「不」收集的信息

- **照片与视频**：您选择的源脸、目标照片仅在本机内存中用于换脸计算，处理完成后即释放，**不会被上传、不会被我们保存**。
- **人脸与生物特征数据**：应用使用设备端机器学习模型（ONNX Runtime + Core ML）进行人脸检测与对齐，相关特征数据**仅在本地临时使用，不上传、不持久化、不与任何身份绑定**。
- **账号信息**：本应用**不要求注册账号**，不收集姓名、手机号、邮箱等个人身份信息（购买相关身份由 Apple 代管，见 2.3）。
- **位置信息**：不收集。
- **设备标识符**：不主动收集用于追踪的设备 ID。

### 2.2 我们分析、广告与第三方 SDK

本应用**不集成任何第三方广告 SDK、不集成任何用户行为分析/追踪 SDK**。我们不基于您的个人数据进行画像或定向广告。

### 2.3 购买与支付信息

应用内购买（如「Pro 永久版」）由 **Apple App Store** 直接处理。我们**无法获取您的信用卡号、Apple ID 密码等支付凭据**。与该购买相关的订单与收据信息由 Apple 按其隐私政策管理。我们仅在本地记录「是否已解锁 Pro」这一布尔状态，用于功能解锁。

### 2.4 崩溃与诊断数据

为改进稳定性，系统可能会通过 Apple 的崩溃报告机制收集**匿名的崩溃日志**。这类日志由 Apple 汇总后提供给我们，不含您的照片或人脸内容。您可在 iOS「设置 → 隐私与安全性 → 分析与改进」中关闭共享。

### 2.5 人脸数据与生物特征信息专项说明（Face Data）

本应用核心处理对象即为**人脸图像与生物特征信息**，本小节对此作专项、完整的说明：

- **收集的人脸数据**：您在使用中主动从本机「照片」选取的「源脸」与「目标」照片；以及为完成换脸，设备端模型在内存中临时生成的**人脸关键点（landmarks）、人脸特征向量（embeddings）等中间特征**。我们**不采集**任何与您身份绑的生物识别 ID（如 Face ID 模板）。
- **使用目的**：上述数据**仅用于**在您的设备本地完成人脸检测、对齐与换脸这一项您主动触发的功能，绝不作任何其他用途。
- **是否共享第三方**：**否**。人脸数据**不会**以任何形式上传至服务器，也**不会**与任何第三方（包括任何 AI 云服务商）共享、出售或交换。
- **存储位置**：源脸/目标原图仅驻留于设备内存，处理结束即释放，**不被写入磁盘**；换脸**结果图**及 320px 的源/目标**缩略图**仅保存在**您设备本地的应用沙盒目录**（`Documents/History/`）中，不离开设备。
- **留存期限**：源脸/目标原图与临时特征在处理完成后立即丢弃；结果图与缩略图会保留在设备沙盒中，**直至您主动删除**（在 App 内「历史」页可逐条或清空删除）。卸载 App 会一并清除沙盒内所有历史数据。
- **删除方式**：您在「历史」页删除某条记录时，App 会同步删除其对应的结果图与缩略图文件；您也可通过卸载 App 彻底清除。我们不保存任何可远程删除的人脸数据，因为相关数据本就只存在于您的设备。

> **可直接引用的核心声明（Quotable summary）：**
> "所有照片、人脸与生物特征数据均在用户设备本地处理，不会上传到任何服务器，不会与任何第三方共享，也不会被用于任何与换脸功能无关的用途。源脸与目标原图仅在内存中临时使用、处理完成后立即释放；仅换脸结果图及缩略图保存在设备本地应用沙盒，可由用户随时删除。"

---

## 3. 信息的使用目的

我们仅在本地使用您的数据以：

- 在您的设备上完成换脸、画质增强等您主动触发的功能；
- 将处理结果保存到您的「照片」图库（需您授权）；
- 验证内购状态以解锁对应功能。

我们**不会**将您的数据用于广告、营销或任何与产品功能无关的用途。

---

## 4. 数据共享与披露

我们**不与任何第三方共享、出售或交换**您的照片、人脸数据或个人身份信息。

仅在以下极少数情况下，我们可能依法披露信息：

- 应国家法律、法规或有权机关的合法要求；
- 为保护本应用及其用户的合法权益所必需。

---

## 5. 数据存储与安全

- 所有图像与换脸推理均在**设备本地**完成，**不调用任何云端 AI 服务、不向任何外部服务器发送人脸或图像数据**。本应用不依赖任何第三方 AI 服务商。
- 源脸/目标原图仅在设备内存中临时使用，**处理完毕即释放，不写入磁盘**。
- 换脸**结果图**及缩略图保存在**设备本地应用沙盒**（`Documents/History/`）中，由「历史」功能管理；您可随时在 App 内删除，或卸载 App 彻底清除。您也可将结果保存到本机「照片」图库（需授权），保存后的文件由您与系统权限控制。
- 我们**不维护任何位于服务器端的用户照片或人脸数据库**。
- 我们采用 Apple 平台标准的安全机制（如应用沙盒隔离）保护应用数据。

---

## 6. 儿童隐私

本应用为娱乐用途的图像处理工具。我们**不故意收集**未满 13 周岁（或适用司法辖区规定年龄）儿童的任何个人信息。由于我们不上传、不存储任何用户数据，儿童使用本应用时同样不会产生被我们收集的数据。若您是监护人并对此有疑问，可通过下方邮箱联系我们。

---

## 7. 您的权利

由于我们不存储您的照片或人脸数据，您无需发起"删除账户/数据"请求——这类数据本就不存在于我们的系统中。

关于内购：您可通过 App Store 的「购买记录」与「恢复购买」管理您的订阅/购买状态；如需退款，请遵循 Apple 的退款政策。

---

## 8. 本政策的变更

如本政策发生变更，我们将在应用更新说明或本页面发布更新版本，并更新「生效日期」。重大变更会以合理方式通知您。

---

## 9. 联系我们

如对本隐私政策有任何疑问，请通过以下方式联系：

- **邮箱：** 【请填写支持邮箱】
- **应用内：** 设置 → 关于 → 联系支持

---

## 附录：英文摘要（Face Data Summary / EN）

For the convenience of App Review, the following is an English summary of how this app handles face data. The binding version is the Chinese text above.

- **What face data we collect:** The "source face" and "target" photos you voluntarily pick from your device Photos, plus temporary in-memory face landmarks/embeddings generated on-device by local ML models to perform the face swap. We do **not** collect any identity-bound biometric ID (e.g., Face ID template).
- **Use:** Solely to perform on-device face detection, alignment, and face swapping that you explicitly trigger. No other use.
- **Sharing with third parties:** **None.** Face data is **never** uploaded to any server and **never** shared, sold, or exchanged with any third party — including any cloud AI provider.
- **Storage location:** Source/target originals live only in device memory and are released after processing (never written to disk). The resulting swapped image and 320px thumbnails are stored only in the app's local sandbox (`Documents/History/`) on the device.
- **Retention:** Source/target originals and temporary features are discarded immediately after processing. Result images/thumbnails remain in the device sandbox **until you delete them** (via the in-app "History" screen, or by uninstalling the app).
- **Deletion:** Deleting a record in "History" removes its result image and thumbnails; uninstalling the app clears all sandbox data. We hold no server-side copy to delete because no face data ever leaves the device.
- **AI service provider:** **There is no third-party AI service provider.** All face processing runs 100% on-device using on-device machine learning (ONNX Runtime Mobile running open-source FaceFusion-derived models). No data is sent to any AI service or cloud.

*本政策为中文版本，如与其他语言版本存在歧义，以中文版本为准。*
