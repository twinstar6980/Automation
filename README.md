# Automatic

为个人项目编写的自动化构建流程。

## 构建列表

* [`Twinning`](https://github.com/twinstar6980/Automation/actions/workflows/diliver.Twinning.yml)

  * [latest](https://github.com/twinstar6980/Automation/releases/tag/Twinning-latest)

* [`KairosoftGameManager`](https://github.com/twinstar6980/Automation/actions/workflows/diliver.KairosoftGameManager.yml)

  * [latest](https://github.com/twinstar6980/Automation/releases/tag/KairosoftGameManager-latest)

## 构建参数

* `repository_url`

  需要构建的代码仓库 URL 。

* `enable_signing`

  对构建产物进行签名。

  > 未签名的文件在一些系统中可能不便于安装或使用。
  >
  > 如果启用签名，必须在 Secrets 中设置 `keystore_file`（ Base64 编码的 p12 密钥库文件数据）与 `keystore_password`（密钥库的密码）。

* `build_<platform>`

  是否为指定平台进行构建。

* `publish_release`

  是否将构建产物发布到 Releases 中。

* `publish_release_tag_suffix`

  将构建产物发布到 Releases 时的 tag 后缀。
