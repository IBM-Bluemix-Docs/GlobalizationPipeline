---

copyright:
  years: 2015, 2017
lastupdated: "2017-07-19"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# 修改軟體組詳細資料
{: #modifybundles}

當您開啟軟體組時，可以檢視其所有詳細資料。會列出軟體組中的所有目標語言，以及其現行翻譯狀態。

![軟體組詳細資料頁面顯示軟體組及其翻譯的相關資訊。](images/bundleDetails.png)

軟體組中每一種語言的狀態可以是「進行中」、「失敗」或「已翻譯」：

| 狀態| 說明|
|--------|-------------|
| 進行中| 仍在進行機器翻譯。|
| 失敗| 將資源檔翻譯成目標語言時發生錯誤。|
| 已翻譯| 已完成翻譯成目標語言。|

您可以更新軟體組所使用的資源檔、將目標語言新增至軟體組、刪除軟體組中的目標語言，以及下載針對目標語言所產生的翻譯。

## 更新軟體組所使用的資源檔

1. 在來源語言旁邊，按一下「動作」直欄中的**上傳資源**圖示 ![選取此圖示以上傳新的資源檔](images/uploadIcon.png)。
2. 按一下**瀏覽**，然後選取要上傳的新資源檔。
3. 選取您所上傳之資源檔的類型
 * Java Properties 檔案
 * AMD I18N
 * JSON
4. 按一下**更新**以上傳新的資源檔。

新增或已更新資源檔中的鍵值組會與已上傳的值同步。只會翻譯新增或已變更的內容。

## 將目標語言新增至軟體組

1. 按一下**新增語言**按鈕。
2. 即會顯示所有可用的目標語言。選取要新增至軟體組的語言。

將立即開始所選取語言的翻譯。

## 刪除軟體組中的目標語言

當您刪除軟體組中的目標語言時，會移除專案中的目標語言和所有關聯的翻譯。在要移除之目標語言的「動作」直欄中，按一下**移除此目標語言**圖示 ![選取「移除此目標語言」的垃圾筒圖示](images/trashIcon.png)。

## 下載目標語言的已產生翻譯

{{site.data.keyword.GlobalizationPipeline_short}} 提供數種方法，將目標語言的翻譯併入應用程式中。您可以將翻譯下載為資源檔，並將它併入應用程式建置中。您也可以使用其中一個開放程式碼 [SDK](https://github.com/IBM-Bluemix/gp-common)，從 {{site.data.keyword.GlobalizationPipeline_short}} 動態參照翻譯。 

<!-- For information on {{site.data.keyword.GlobalizationPipeline_full}} SDKs, see <link>. -->

若要將翻譯下載為資源檔，請執行下列動作： 

1. 在要下載之目標或來源語言的**動作**直欄中，按一下**下載翻譯**圖示 ![選取「下載」圖示來下載目標語言的來源索引鍵或翻譯](images/downloadIcon.png)。
2. 選取檔案格式。
3. 按一下**下載**。
