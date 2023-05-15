# upload
app版本更新


导入方式

将JitPack存储库添加到您的构建文件中(项目根目录下build.gradle文件)

allprojects {
    repositories {
        maven { url 'https://jitpack.io' }
    }
}

dependencies {
    implementation 'implementation 'com.github.lhjgege:upload:1.0.0''
}

本框架是基于 https://github.com/easyandroidgroup/UpdatePlugin 修改而来入
增加修改版本号来判断升级app版本。
增加setNetWork(false)为false不走请求获取app版本更新接口
需要再setUpdateParser中自定义返回app的版本号下载链接等等配置，response为null
