# GifPlayer
> 英日文說明都是亂寫的，看不懂請完全不要在意
> English details is for fun, don't care about it.
> 日本語説明は趣味で書いただけ、読み難いなら気にしないて。

一個簡單的 Gif 播放器，適用於 uGUI，基於將 Gif 轉成 SpriteSheet 的功能。

A simple unity Gifs player for uGUI base on gif to png spritesheet feature.

uGUI に使うシンプルな GIF プレーヤ。自動的に GIF イメージを PNG スプライトシートに変換するこどが可能です。

## Install
下載[套件包](https://github.com/wix3000/GifPlayer/raw/master/GifPlayer.unitypackage)匯入專案當中，確保 csc.rsp 檔案置於 Assets 資料夾下的根層級，重新啟動編輯器後即可使用。
如果專案中已經使用 csc.rps，用文字編輯器開啟並合併兩個檔案的內容即可。

Download and import [package](https://github.com/wix3000/GifPlayer/raw/master/GifPlayer.unitypackage) to your project, make sure 'csc.rsp' file is putting in root of Assets folder. Then restart Unity editor, everything should be done.
If there is already a csc.rsp file, open two files using IDE and merge contents.

[パッケージ](https://github.com/wix3000/GifPlayer/raw/master/GifPlayer.unitypackage)をダウンロードしてインポードする、その中の‘csc.rsp’ファイルを Assets フォルダーのルートに移動してください。
もし既に csc.rsp が存在した場合は、IDE で二つを開けて、中に書いた内容を一つに併合してください。

### Using 2017 below
如果使用 2017 之前的版本，需要將 csc.rsp 更名為 msc.rsp。

If using unity 2017 below, csc.rsp file must rename to 'msc.rps'.

エディタが 2017 以前のを使いたければ、csc.rsp を msc.rps にリネームが必要です。

### On macOS
在 macOS 環境底下 Unity 不會自動指向 Mono 的安裝路徑，要在應用程式中找到對應版本的 Unity，按右鍵顯示套件內容，用文字編輯器打開 content/MonoBleedingEdge/etc/mono/config。
找到 dll=gdiplus 及 dll=gdiplus.dll 的項目後將項目的 target 改成本機安裝的 Mono 函式庫路徑。
預設為：/Library/Frameworks/Mono.framework/Versions/6.6.0/lib/libgdiplus.dylib
注意： 路徑中的 6.6.0 可能會隨著安裝的版本不同而有所改變。

## Quick Start
- 將 Gif 圖檔放進專案目錄當中，在專案視窗裡對圖片按右鍵選擇 Create>GifSheet
<img src="https://raw.githubusercontent.com/wix3000/GifPlayer/master/picture1.png"></img>

- Gif 圖片將自動被轉成 PNG 圖片儲存，並切割好 Sptires
<img src="https://raw.githubusercontent.com/wix3000/GifPlayer/master/picture2.png"></img>

- 場景上會自動生成一個 GifPlayer 用於顯示。現在按下執行，你應該就會看到動畫播放了。
<img src="https://raw.githubusercontent.com/wix3000/GifPlayer/master/picture3.png"></img>
