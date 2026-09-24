# 服务器 · 整合包分发

本仓库用于分发**我们自己开的服务器上用到的整合包**。

原作者大多把整合包放在网盘上，下载慢、要会员、还容易断；我们把这些文件**原封不动**搬一份到 GitHub，给服务器玩家做一个更快的下载点。

以后还会陆续分发更多整合包 —— **一个整合包对应一个 Release**，往下翻即可看到全部。

---

## ⚠️ 免责声明（请逐条读完）

1. **整合包都不是我们做的。** 本仓库分发的所有整合包，均由**各自的原作者 / 整合者**制作，**版权与著作权全部归各自的作者所有**。我们不是作者，也不主张任何权利。
2. **本仓库只做「搬运 + 加速」。** 这些文件原本发布在网盘等渠道，下载速度慢；我们只是把**同一个文件原封不动**搬到这里，**仅为服务器玩家下载方便**。
3. **未做任何修改。** 所有文件与原作者发布的原始版本**完全一致**，未增删、未二次打包、未植入任何额外内容。每个文件都给出 SHA-256，可自行比对。
4. **请优先支持原作者。** 每个整合包下方都标注了**原作者的原始发布地址**（网盘 / 视频 / 帖子），提取码也一并给出。喜欢的话请走原作者渠道。
5. **完全免费、非商业。** 本仓库不售卖整合包、不设付费墙、不接广告、不以此盈利。请勿将本仓库内容用于任何商业用途。
6. **侵权即删。** 原作者或权利方认为本仓库的搬运行为不妥的，请通过下方联系方式告知，我们会在**第一时间删除相关内容**，不需要任何额外流程。
7. **风险自负。** 使用整合包产生的任何后果（存档损坏、模组冲突、账号问题、与服务器规则冲突等）由使用者自行承担，**建议先备份存档**。
8. **无隶属关系。** 本仓库与任何原作者、Mojang Studios、Microsoft 及任何第三方平台均无隶属、赞助或合作关系。

> 一句话：**整合包都是别人做的，我们只是给服务器玩家搭了个更快的下载点。仅用于自己开的服务器，非商业用途。**

---

## 📦 已分发的整合包

| 整合包 | 版本 | 大小 | 原版出处 | 下载 |
| --- | --- | --- | --- | --- |
| **Chapter of Yuusha Ⅲ**（勇者之章Ⅲ）<br>客户端导入包 · 绝望纪元版本 | v3.13.13 | 1.07 GiB | [原作者网盘](https://pan.baidu.com/share/init?surl=ALWC3NIeXsvfiu6zEHwaTA)（提取码 `yzzz`）<br>[原作者视频（B站）](https://www.bilibili.com/video/BV1nYN2evEug/) | [前往下载](../../releases/tag/v3.13.13) |

> 表格会随新整合包发布持续更新；也可以直接进 **[Releases 总页面](../../releases)** 看全部。

---

## 📥 下载

👉 **[Releases 页面](https://github.com/NovaX322/zhb/releases)** —— 一个整合包一个 Release，在 **Assets** 里点 zip 即可。

---

## ✅ 校验文件完整性（建议）

下载完成后核对 SHA-256，与下表及对应 Release 说明里的值一致即可。

**Windows PowerShell：**

```powershell
Get-FileHash -Algorithm SHA256 "下载的文件.zip"
```

**Linux / macOS：**

```bash
sha256sum "下载的文件.zip"
```

| 整合包 | 下载文件名 | SHA-256 |
| --- | --- | --- |
| 勇者之章Ⅲ v3.13.13 | `Chapter-of-Yuusha-III-v3.13.13-Client-Pack-Despaired-Era.zip` | `29BD7F4265DDD216419D18589AE1EEE4DB7CAB5FB9DE59B77BFD2E8584B269AD` |

> 📌 **关于文件名**：GitHub 的 Release 附件名会剔除中文与全角符号，所以上传时文件名会被转写成纯 ASCII（例如 `Chapter.of.Yuusha.III.v3.13.13.zip`）。**文件内容与原版完全一致**，只是名字变了。

---

## 🛠️ 安装（客户端导入包类）

> 这类是**客户端导入包**，不是需要手动解压到 `.minecraft` 的普通压缩包，请用启动器的「导入整合包」功能加载。

1. 准备一个支持整合包导入的启动器（HMCL / PCL2 等）。
2. 启动器里选 **导入整合包 / 安装整合包**。
3. 选中刚下载的 zip，等待自动解压与安装依赖。
4. 装完后在版本列表里选择对应版本启动。
5. 首次启动较慢（要解压和初始化模组），耐心等待。

**注意：**

- 磁盘建议预留 **3 GB 以上**。
- 启动器提示内存不足的话，把最大内存调到 **4 GB 以上**。
- 联机地址请以服务器公告为准，本仓库不提供服务器连接信息。

---

## 📮 联系 / 删除请求

- 原作者或权利方如需下架，请在 [Issues](https://github.com/NovaX322/zhb/issues) 提出，或直接联系仓库所有者。
- 服务器玩家遇到整合包相关问题，请先在服务器群内反馈。

---

## 📜 版权声明

本仓库的说明文字以 CC0 释出；**分发的整合包本体版权归各自原作者所有**，本仓库不主张任何权利。

---

<details>
<summary><b>给维护者：新增一个整合包怎么发（点开）</b></summary>

### 约定

- **一个整合包 = 一个 Release**，不要覆盖旧的附件。
- **Tag**：整合包简称 + 版本，例如 `yuusha3-v3.13.13`（首个包用的 tag 是 `v3.13.13`）。简称要能区分不同整合包，避免版本号撞车。
- **附件名**：纯 ASCII。空格用 `-` 代替，**中文和全角符号会被 GitHub 剔除**，别指望它保留。
- **Release 说明必须包含**：原作者原始链接（网盘 + 提取码 + 视频/帖子）、大小、SHA-256、免责声明。
- 发完记得更新本 README 的「已分发的整合包」和校验值两张表。

### 步骤

```bash
# 0. 国内网络建议挂代理
export HTTPS_PROXY=http://127.0.0.1:10808

# 1. 算哈希与大小
sha256sum "整合包.zip"
stat -c %s "整合包.zip"

# 2. 建 Release（target_commitish 用 main）
curl -X POST \
  -H "Authorization: Bearer $GITHUB_TOKEN" \
  -H "Accept: application/vnd.github+json" \
  https://api.github.com/repos/NovaX322/zhb/releases \
  -d '{"tag_name":"yuusha3-v3.13.13","target_commitish":"main","name":"整合包标题","body":"说明…"}'

# 3. 上传附件（从返回 JSON 里取 id 填到 <RELEASE_ID>）
#    用 -T 走流式上传，别用 --data-binary @，1 GB 文件会吃满内存
curl -X POST \
  -H "Authorization: Bearer $GITHUB_TOKEN" \
  -H "Content-Type: application/zip" \
  -H "Expect:" \
  -T "整合包.zip" \
  "https://uploads.github.com/repos/NovaX322/zhb/releases/<RELEASE_ID>/assets?name=ASCII-Filename.zip"

# 4. 附件名被 GitHub 洗过的话，改名
curl -X PATCH \
  -H "Authorization: Bearer $GITHUB_TOKEN" \
  -H "Accept: application/vnd.github+json" \
  https://api.github.com/repos/NovaX322/zhb/releases/assets/<ASSET_ID> \
  -d '{"name":"ASCII-Filename.zip"}'

# 5. 确认 digest 与本地哈希一致，再更新 README
```

### 上限提醒

- 仓库单文件 **100 MB**、Release 附件单文件 **2 GB**、Release 说明正文 **125 KB**。
- 整合包超过 2 GB 就得**分卷压缩**，在 Release 说明里写清分卷顺序与合并方法。

</details>
