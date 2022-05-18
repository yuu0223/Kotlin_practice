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
在Android APP開發中，最常見的架構有這三種：
1. MVC (Model View Controller)
2. MVP (Model View Presenter)
3. MVVM (Model View View-Model)
<br/>
這次的練習選擇以MVVM來練習，首先來看MVVM的架構圖：<br/>
<img src="https://github.com/yuu0223/Kotlin_practice/blob/main/Pictures/MVVM.png" width="600" alt="MVVM"/><br/>
圖片轉自https://ithelp.ithome.com.tw/articles/10248755 

- - -
> View

前端在做畫面設計、動作設計，任何與畫面有關的都屬於View。<br/>

像是下列幾項都屬於View：
1. Activity
2. Fragment
3. Adapter
4. Layout
5. XML(只有這個是屬於刻UI頁面的部分)<br/>

以上1~4都是要放置在Activities層下，用來設計畫面動作的。至於XML是另外放置在res/layout層下的，用來刻UI畫面。<br/>

<br/>

> Model

包含所有的data class、Repository，負責儲存或取得資料，可以透過api形式、本地DB形式等。

<br/>

> View-Model

負責幫忙Activity(View)及Repository(Model)進行資料交換，可以透過observe、databinding的方式來呈現。他不需要知道<br/>

<br/>

* **What is observe and databinding?**

Observe是透過觀察的方式，當前端(View)需要資料時才會去呼叫View-Model，請他跟後端(Model)拿資料。

Databinding的話，他是把data跟UI元件擺在一起，不需要手動把數據設計給UI元件。




