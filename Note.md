# 记录

#### 发布到JCenter

1. ##### 项目所有库整体发布

   gradlew clean build bintrayUpload -PbintrayUser=你的用户名 -PbintrayKey=你的密钥 -PdryRun=false

2. ##### 分库发布

   gradlew :VerifyCodeView:bintrayUpload -PbintrayUser=你的用户名 -PbintrayKey=你的密钥 -PdryRun=false（如果本地库已存在，可直接发布）

   gradlew :VerifyCodeView:clean build bintrayUpload -PbintrayUser=你的用户名 -PbintrayKey=你的密钥 -PdryRun=false（本地库不存在，先编译后发布）
