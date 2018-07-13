# android 集成rn和h5

# 碰到的坑

<table>
<tr>
<th>坑</th>
<th>解决方案</th>
<th>参考资料</th>
</tr>
<tr>
<td>
You have JVM property "https.proxyHost" set to .... This may lead to incorrect behavior. Proxy should be set in Settings|HTTP Proxy
</td>
<td>
网络被设置了代理，一次检测gradle.properties文件，以及操作系统网络是否设置了代理
</td>
<td>https://blog.csdn.net/xiaochenuu/article/details/80245931</td>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
</tr>
</table>

# 打包命令
react-native bundle --platform android --dev false --entry-file index.android.js --bundle-output ./android/app/src/main/assets/index.android.bundle --assets-dest app/src/main/res/