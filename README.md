# iOS-Auto-Archive

iOS自动打包脚本

```
使用方法:
 
-c NAME 工程的configuration, 默认为Release
-o PATH 生成的ipa文件输出的文件夹（必须为已存在的文件路径）默认为工程根路径下的 build/ipa-build 文件夹中"
-t NAME 需要编译的target的名称
-w      编译workspace
-s NAME 对应workspace下需要编译的scheme
-n      编译前是否先clean工程
-p      平台标识符
-u      是否上传蒲公英
```

> 例如 ``` shell
./iOSAutoBuild ./ -c Release -t target -w -s scheme -n -u
```

如果要自动上传蒲公英, 先把 "uKey=******" / _api_key=******" / "password=******" 改成自己的.



完成提醒需要安装 Terminal-notifier

```
sudo gem install terminal-notifier
```

如果要使用完成提醒, 先安装 Terminal-notifier ([参考](http://osxdaily.com/2012/08/03/send-an-alert-to-notification-center-from-the-command-line-in-os-x/))