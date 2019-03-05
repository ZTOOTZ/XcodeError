# XcodeError
Xcode错误记录及解决办法

# You don’t have permission
#### 方法一
* Xcode->File->Projects Setting->Build System->设置成Legacy Build System  (推荐)


#### 方法二
* 清除DeviceData 并clean工程


#### 方法三
* 将info.plist的文件中的Executable.file中的文件修改为:$(PRODUCT_NAME) 改完后记得clear下

# has denied the launch request
1. Xcode->Targets->Build->更新下build版本号
2. Xcode->Edit Scheme->取消勾选Debug executable
3. 将钥匙串中的证书设置为`有效`而非`始终信任`
4. 重启手机(🤦‍♀️) 

# The executable was signed with invalid entitlements.

* 重启xcode 
* 重启电脑
* 证书从自动切手动来回倒腾


# Xcode 10: A valid provisioning profile for this executable was not found
* Xcode->File->Projects Setting->Build System->设置成Legacy Build System

