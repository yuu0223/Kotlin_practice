# Kotlin_practice
### **About**
* 主要是想紀錄自己初學APP所遇到的各種大小事！
* 使用工具：Android Studio、Kotlin
* 架構：MVVM

## **Outlines**
* [Android Studio & JDK - Prepare The Enviroments](#android-studio--jdk---prepare-the-enviroments)
* [Architetural Pattern - MVVM](#introduce-architetural-pattern---mvvm)
* * * *

## **Android Studio & JDK - Prepare The Enviroments**
> **1. Download JDK from Oracle**
* [Oracle下載網站](https://www.oracle.com/java/technologies/downloads/#jdk18-mac)
* **下載符合自己系統的dmg檔 (ARM:M1晶片 / x64:Intel晶片)** <br/>
<img src="https://github.com/yuu0223/Kotlin_practice/blob/main/Pictures/jdk_download.png" width="1000" alt="jdk_download"/><br/>

> **2. Download Android Studio**
* [Android Studio下載網站](https://developer.android.com/studio) <br/>
<img src="https://github.com/yuu0223/Kotlin_practice/blob/main/Pictures/android_download.png" width="600" alt="android_download"/><br/>

> **3. Install Android Studio**
* **Complete Installation** > Do not import settings. <br/>
(在這邊的話，如果沒有要導入以前的版本就可以直接選取Do not import settings.)

* **Android SDK相關套件下載** > 會自動導入要下載哪些套件，只要按Accept就可。
* * * *
## **Introduce Architetural Pattern - MVVM**
* 在Android APP開發中，最常見的架構有這三種：
1. MVC (Model View Controller)
2. MVP (Model View Presenter)
3. MVVM (Model View View-Model)
