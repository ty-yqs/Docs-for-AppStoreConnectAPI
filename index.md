## App Store Connect API 使用说明
### 上传AuthKey文件
- 登录 [App Store Conect](https://appstoreconnect.apple.com)
- 进入 [用户和访问](https://appstoreconnect.apple.com/access/users)
- 点击菜单栏密钥，选择密钥类型为'App Store Connect API'
- 点击'+'按钮
- 名称随便填写，访问一栏选取'开发者'，如下图所示

![7C5E58C4-6A11-4194-922B-07FEE281D7EF](https://raw.githubusercontent.com/ty-yqs/Docs-for-AppStoreConnectAPI/gh-pages/assets/39E24207-A8F0-42E4-BDD4-FE0883119C2B.jpeg)
- 确认无误后点击创建按钮
- 点击刚创建的证书对应的最右边'下载API密钥'按钮
- 弹出的窗口中点击'下载'按钮，妥善保管下载的文件(文件名和文件内容不能修改)
- 打开[AuthKey上传页面](https://asc.isign.ren/UploadAuthKey.html)
- 点击'选取文件'按钮，在弹出的窗口中选择下载好的p8文件
- 点击'提交'按钮
- 在跳转的页面中核对文件名是否为上传时的文件名
- 成功上传AuthKey文件

## 获取Token
- 请求地址: /v1/GetToken
- 请求方式: GET
- 请求参数:

| 参数 | 值        |
|------|-----------|
| iss  | Issuer ID |
| kid  | 密钥 ID   |

- 返回格式: json
- 返回参数:

| 参数  | 值    |
|-------|-------|
| token | token |

## 注册设备
- 请求地址: /v1/RegisterNewDevice
- 请求方式: GET
- 请求参数:

| 参数  | 值             |
|-------|----------------|
| token | token          |
| udid  | 待注册设备UDID |

- 返回格式: json
- 返回参数:

英文字面意思:)
