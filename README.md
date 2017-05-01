# Pure JAVA @ Android
> 使用 Android Studio作為IDE 開發 純Java 

# AS開一個新專案觀察一下!
![N|Solid](http://i.imgur.com/Fubooy7.jpg)

# 確認開好了
![N|Solid](http://i.imgur.com/pt3O0vN.jpg)

# 切換到Project模式
```sh
 看看Android app 在Android Studio 內的資料分佈格式
```
![N|Solid](http://i.imgur.com/IYGyiVh.jpg)

# 資料分佈格式
```sh
 主要是src內包main再包java然後才是packagename
```
![N|Solid](http://i.imgur.com/p03wK9i.jpg)

# 建立一個新專案
```sh
 改造開始--給純Java用的
```
![N|Solid](http://i.imgur.com/wgBO3qd.jpg)

# 確認建好了之後關閉它
![N|Solid](http://i.imgur.com/OvllIPc.jpg)

# 砍了這些檔案與資料夾

```sh
app build  settings.gradle
```
![N|Solid](http://i.imgur.com/uv5xgoU.jpg)

# 建立src內包main再包java再包packagename
```sh
偷懶的話 直接從app裡面的拉出來也可以
```
![N|Solid](http://i.imgur.com/kv7q12O.jpg)
![N|Solid](http://i.imgur.com/u6wFpYK.jpg)

# 修正build.gradle內容
```sh
可以用第三方軟體直接開啟編輯修正
```
![N|Solid](http://i.imgur.com/nqNe87v.jpg)
```sh
這是使用AS開啟後修正
```

![N|Solid](http://i.imgur.com/XYSpiHW.jpg)
```sh
apply plugin: 'java'
version = '1.0'
sourceCompatibility = 1.8
targetCompatibility = 1.8

mainClassName = 'idv.neo.TCPServer'
jar {
    manifest {
        attributes 'Implementation-Title': 'TCPServer Examples', 'Implementation-Version': version,
                'Main-Class': mainClassName
    }
}

run {
    standardInput = System.in
}

repositories {
    mavenCentral()
    jcenter()
}

dependencies {
    compile fileTree(dir: 'libs', include: ['*.jar'])
}
```
![N|Solid](http://i.imgur.com/KhLSkNu.jpg)

# 重新命名Class name為FirstJava
```sh
因為是偷懶直接用app內的
```
![N|Solid](http://i.imgur.com/lhlRJl0.jpg)
![N|Solid](http://i.imgur.com/PQ5WfGb.jpg)

# 在FirstJava內補上正確的範例code
![N|Solid](http://i.imgur.com/2DEh5Fp.jpg)

# 修正並編輯Run組態設定檔1
```sh
加入Java的單獨支援
```
![N|Solid](http://i.imgur.com/dKE9f70.jpg)

# 修正並編輯Run組態設定檔2 : 砍了app
```sh
移除Android 相關組態
```
![N|Solid](http://i.imgur.com/hgV0E4M.jpg)

# 修正並編輯Run組態設定檔3 : 加上Java組態
```sh
加上Java組態
```
![N|Solid](http://i.imgur.com/4uexG1c.jpg)

# 修正並編輯Run組態設定檔4 : 完整packagename名稱
```sh
填入Main Class 的完整packagename名稱 
```
![N|Solid](http://i.imgur.com/HUGsFZq.jpg)
# 編輯Run組態設定檔4 : Use classpath of module
```sh
記得填入 Use classpath of module (這是要指定的)
```
![N|Solid](http://i.imgur.com/2jIy4YC.jpg)

# 使用設定檔嘗試執行看看 
![N|Solid](http://i.imgur.com/J9jIK4W.jpg)
![N|Solid](http://i.imgur.com/wWM3whY.jpg)

# 進階編輯Run組態設定檔  : 支援輸出jar
![N|Solid](http://i.imgur.com/lQYaYHB.jpg)
![N|Solid](http://i.imgur.com/dNrqde6.jpg)
![N|Solid](http://i.imgur.com/6e1Qz10.jpg)
![N|Solid](http://i.imgur.com/cwg3RDs.jpg)
![N|Solid](http://i.imgur.com/YJFwLOl.jpg)
![N|Solid](http://i.imgur.com/O3Jj3Ae.jpg)


# 目前除了classes有輸出外沒有其他資料夾跟檔案 
![N|Solid](http://i.imgur.com/FQWFiCQ.jpg)
# 使用設定檔再執行看看 
![N|Solid](http://i.imgur.com/BHcTxy0.jpg)
# 執行結果 多出了資料夾跟jar
![N|Solid](http://i.imgur.com/rrUVPbz.jpg)
# jar檔執行結果 
![N|Solid](http://i.imgur.com/i0ffW94.jpg)
