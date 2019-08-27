# xlsVbaRatingTool_02_2Raters_VoiceData
2 raters listen to the voice data then rate them.  
2人の評価者が、音声データを聞き、観点毎に評価を行う。

# Sample direcotry structure.

~~~
Root Directory.
│
│  RatingTool_sound.xlsm
│  
├─Data
│  └─sound_data
│      ├─class-01
│      │      C01-Q1-0001.wav
│      │      C01-Q1-0002.wav
│      │      C01-Q1-0003.wav
│      │      C01-Q1-0004.wav
│      │      C01-Q1-0005.wav
│      │      C01-Q1-0006.wav
│      │      C01-Q1-0007.wav
│      │      C01-Q1-0008.wav
│      │      C01-Q1-0009.wav
│      │      C01-Q1-0010.wav
│      │      
│      └─class-02
│              C02-Q1-0001.wav
│              C02-Q1-0002.wav
│              C02-Q1-0003.wav
│              C02-Q1-0004.wav
│              C02-Q1-0005.wav
│              C02-Q1-0006.wav
│              C02-Q1-0007.wav
│              C02-Q1-0008.wav
│              C02-Q1-0009.wav
│              C02-Q1-0010.wav
~~~

# Usage
## Step 0 : Preparatison.

The excel file contains 4 sheets like below. Two sheets "$list_rating" and "$list_content" are hidden normaly. / Excelファイルには4つのシートが含まれ、"$list_rating"と"$list_content"シートは通常非表示になっています。  
<img src="https://github.com/okagen/xlsVbaRatingTool_02_2Raters_VoiceData/blob/master/Data/02-1_ToolSheet.png"  width="400">  

## Step 1 : Input some conditions on the Tool sheet.

  1. Parent directory / 親ディレクトリ
      - Enter the directory path where the audio files are stored. If it's blank, the directory which contains the Excel file used as the parent directory, and the audio files under that directory are searched. / 音声ファイルが保存されてるディレクトリのパスを入力します。空欄の場合、Excelファイルが保存されているディレクトリを親ディレクトリとし、その下にある音声ファイルを検索します。
  1. Keyword in finename / ファイル名キーワード
      - Input "*wav". Wildcard search is available. / "*wav"を入力。ワイルドカードによる指定が可能です。
  1. Number of point of view / 観点の数
      - Input a number from 1 to 10. / 1～10を入力。
  1. Then click the "Create sheet"(シート作成) button. / 上記を入力したら【シート作成】ボタンを押します。
  
<img src="https://github.com/okagen/xlsVbaRatingTool_02_2Raters_VoiceData/blob/master/Data/02-2_ToolSheet.png"  width="400">  


## Step 2 : Start rating.

  1. "Rating Sheet"(採点シート) will appear in the excel file like below. / 以下のような「採点シート」が表示されます。
  2. Then click the "Rate without groups."(分類無視採点 開始) button.  / 【分類無視採点 開始】ボタンを押します。
  
<img src="https://github.com/okagen/xlsVbaRatingTool_02_2Raters_VoiceData/blob/master/Data/03-1_RatingSheet.png"  width="400">  

  3. The rating dialog like below will appear. / 採点用ダイアログが表示されます。
  
<img src="https://github.com/okagen/xlsVbaRatingTool_02_2Raters_VoiceData/blob/master/Data/04_RatingDialog.png"  width="400">  

### Description of the dialog usage.
  1. The sound will start automatically when the dialog opens. / ダイアログが開くと、音声が流れだします。
  2. Listen to the sound and input some value of point of view into the text box. / 音声を聞いて、観点の評価値をテキストボックスに入力します。
  <img src="https://github.com/okagen/xlsVbaRatingTool_02_2Raters_VoiceData/blob/master/Data/04-1_RatingDialog.png"  width="600"> 
  
  3. Click the arrow button after input your point of view, you will listen to the next sound. / 入力が終わったら、矢印ボタンを押すことで次の音声を聞くことができます。
  4. If you are a rater B, change the check of the radio button upper right on the dialog. / 右上のラジオボタンで、採点者A、採点者Bを切り替えます。
  
  <img src="https://github.com/okagen/xlsVbaRatingTool_02_2Raters_VoiceData/blob/master/Data/04-3_RatingDialog.png"  width="600"> 
  
  5. If you want to leave some comments, input them into the text box lower right on the dialog. / コメントを残すこともできます。
  
  <img src="https://github.com/okagen/xlsVbaRatingTool_02_2Raters_VoiceData/blob/master/Data/04-4_RatingDialog.png"  width="400"> 











