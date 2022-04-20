# 此專案已停止更新
後續將在[winw1010/tataru-helper-node-text-ver.2.0.0](https://github.com/winw1010/tataru-helper-node-text-ver.2.0.0)繼續更新

# 特別感謝
簡體翻譯: 夜北yakita

# 文件架構
### en
英翻中文件放置處
### jp
日翻中文件放置處
### /chs
簡體文件放置處
### /cht
繁體文件放置處

# 各文件說明
## 修飾日文用的文件 (日文專用，日文 => 日文)
### textSubtitle.json
此為修飾原文部分句子的文件，作用為將翻譯機無法正確翻譯的句子改寫成翻譯機看得懂的形式，取代時機為原文被B區塊取代前  
* 格式：["取代前","取代後"]

### textJp.json
此為修飾原文詞彙的文件，作用為將翻譯機無法正確翻譯的詞彙取代為翻譯機看得懂的同義詞，取代時機為原文被B區塊取代前  
* 格式：["取代前","取代後"]

### textJp2.json
此為修飾原文詞彙的文件，作用為將翻譯機無法正確翻譯的詞彙取代為翻譯機看得懂的同義詞，取代時機為原文被B區塊取代後  
* 格式：["取代前","取代後"]

## 取代詞彙用的文件 (日文、英文 => 中文)
### textForceOverwrite.json
此為強制轉換整句的文件，欲取代的句子需與此文件紀錄的原文「完全符合」取代才會生效，用途為取代翻譯機完全不會翻譯的句子，英文不需要此文件  
* 格式：["取代前","取代後"]

### textChName.json
此為產生臨時NPC名字的文件，臨時產生的名字會被儲存在textNameTemporary.json裡，英文不需要此文件  
* 格式：["取代前","取代後"]

### textMap.json
此為地圖名字的文件  
* 格式：["取代前","取代後"]

### textName.json
此為NPC名字和相關事物的文件  
* 格式：["取代前","取代後"]

### textNameTemporary.json
此為用來儲存尚未分類的臨時名字  
* 格式：["取代前","取代後"]

### textOther.json
此為通用名詞的文件  
* 格式：["取代前","取代後"]

### textAfterTranslated.json
此為翻譯後做最後修飾用的文件，也可以用來校正翻譯機不會翻譯的詞彙  
* 格式：["取代前","取代後"]

## 各項參數文件
### textException.json
此為無視名單，若原文含有在此文件內的任一句子片段皆會被略過不顯示  
* 格式："欲無視的句子片段"

### player.json
此為存放玩家名字的文件，不需要上傳  
* 格式：["取代前","取代後"]

## 各項參數文件 (日文專用)
### textKana.json
此為日文假名文件，平常沒有更動的必要  
* 格式：["平假名","片假名"]

### listForHira.json
此為說話會夾雜片假名或是全都片假名的NPC名單  
在此名單內的NPC對話都會先轉換成平假名再翻譯  
* 格式："NPC名字"

### listOfCrystalium.json
此為隸屬水晶城的NPC名單  
因為在這裡的NPC都稱呼「水晶公」為「公」  
但「公」在日文有公共、公眾的意思  
翻譯機也都如此翻譯，導致無法翻譯出正確的意思  
因此在此名單的NPC說的「公」都會被取代成「水晶公」  
* 格式："NPC名字"
