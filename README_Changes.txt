AozoraEpub3 更新履歴と更新予定
===========

TODO
------------
Milestone1.0.7
　- リリース済 (バグは適宜修正)
Milestone1.1.0
　- 英数字2文字の縦中横設定
　- 目次抽出条件追加（次が空行 前が空白等）

優先度高
　- 外字
　　　対応しない端末の調査と文字除去設定
　- ファイル毎の変換履歴(表紙と目次)の保存

他
　- 確認ダイアログでメタデータの詳細設定
　- 表紙テンプレート(中央と横書き)
　- 未対応の青空注記への対応 (左ルビ、行内の地付き)
　- 禁則文字が続く場合のword-break設定
　- Web小説取得(優先度低)

Changes
------------
[1.1.0]
1.0.7→1.1.0bでの主な変更点 (2015/02)
　- ルビ処理調整 (開始位置判別 注記や画像を間に含むルビ)
　- 割り注注記、窓見出し注記に対応
　- 空行除去 (見出しの後以外)
　- 行頭強制字下げ
　- Web小説取り込み
　- 画像関連調整
　　　余白除去 (ノンブル除去)
　　　挿絵なし (表紙・外字画像以外の画像注記)
　　　画像自動回転
　　　画像回り込み設定
　　　画像キャプション
　　　画像倍率
　- 確認画面でタイトル再取得
　- 確認画面で目次の一覧表示 (選択、名称変更)
　- 前回の表紙設定を利用 (※再起動で履歴は消える)
　- 端末プリセット選択
　- プロファイル設定(追加、削除、名称変更、並び替え)
　- 全画面表示(画像のみ 固定レイアウト+SVG画像タグ)
　- Rarファイル読み込み
　- 文字出力関連
　　　IVS文字のチェックと出力設定
　　　外字用１文字フォントの利用

----
1.1.1b22Q (2024/02/18)
　- ライブラリの管理をgradleに移行
　- 濁点の改修
　- junrar、urlなど
1.1.1b21Q (2024/02/08)
　- ページネーションの対応
　- 非日本語環境での日本語フォントの使用
　- finalize()を使わないように書き換え
1.1.1b20Q (2024/01/26)
　- issue8「nav.xhtml のXML構造が壊れます」の対応
　- GitHub Actionsでビルドに変更
　- antの内容をgradleから実行
1.1.1b19Q (2023/12/31)
　- カクヨム目次変更の対応の修正
　- ビルドをgradleに変更
　- Javaの推奨バージョンを21に
1.1.1b18Q (2023/12/10)
　- カクヨム目次変更の対応
1.1.1b17Q (2023/05/14)
　- コマンドライン時のスタイルシートのマージンの単位が数字になっていたのを修正
　- Javaアプレットが非推奨になっていたので除去した
1.1.1b16Q (2023/05/14)
　- zip/rar固定レイアウトEPUBの出力ができなかったのを修正
　- 使用しているライブラリの更新
　- Javaの推奨バージョンを17以降に
　- フォント追加を可能に
1.1.1b15Q (2023/04/19)
　- 脚注の追加
　- 電書協EPUBのテストデータの追加
　- Java 17に変更
1.1.1b14Q (2022/08/19)
　- 文字コード判別失敗の修正
1.1.1b13Q (2022/04/04)
　- JAVAをAdoptiumに変更。
　- カクヨムの章の取得ができていなかったのを修正
1.1.1b12Q (2022/01/09)
　- 文字コードを自動判別する機能がGUIで動いていなかったのを修正。
1.1.1b11Q (2021/12/17)
　- Log4jを含むcommons-logging-1.2.jarを除去
1.1.1b10Q (2021/10/23)
　- 各種jarライブラリのアップデート
　- 文字コードを自動判別する機能の追加
1.1.1b9Q (2021/5/06)
　- 外字画像、縦長外字画像、横長外字画像を切り分けるようにした。
　- README.txtの追加
1.1.1b8Q (2021/2/27)
　- なろう改稿時のレイアウト修正
　- Windwos 64bit実行ファイルの配布
1.1.1b7Q (2021/1/30)
　- 外字フォント読み込み時のOPFの修正
　- ノベルアップレイアウト変更への追随
1.1.1b6Q (2020/11/09)
　- 左右中央の書き方の変更
　- 画像単ページの書き方の変更
　- middle.cssとimage.cssを電書協に置き換え
　- 言語情報がnullの場合は"ja"として例外回避
1.1.1b5Q (2020/10/01)
　- 電書協サンプルの再現のための機能追加
　- 色文字機能の追加
　- 背景の色指定機能の追加
　- nav.xhtmlの階層化がオフの場合に</li>が足りないのを修正。
1.1.1b4Q (2020/09/02)
　- toc.ncxをもとに戻した
　- 言語設定を追加した
　- 動作環境の説明をJAVAのOpenJDKにした
　- nav.xhtmlの階層化がオフの場合に</li>が足りないのを修正。
1.1.1b3Q (2020/08/01)
　- 画像をfitクラスに指定した
　- iBooks用のprefixを追加
　- ナビゲーション文章をitemフォルダーに移した。
1.1.1b2Q (2020/07/08)
　- 電書協ガイド1.1.3をもとに書き換え
　- ディレクトリ構造を電書協に合わせる
　- toc.ncx、guideタグの削除
1.1.1b1Q (2020/06/25)
　- CSSを電書協CSSに入れ替え
　- 表紙をSVGラッピングに変更
　- 縦書き横書きテンプレートを統一
　- 画像の読み込みをimageIOに一本化
1.1.0b55Q (2020/03/03)
　- 英語版のreadmeを追加
　- ノベルアップ＋とハーメルンに対応
1.1.0b54Q (2020/01/20)
　- 画像zipのEPUBを修正
　- 表紙をsvgかimg fitかを選べるようにした。
　- スタイルシートをfixed-layout-jp.cssに書き換え
1.1.0b53Q (2020/01/14)
　- 超縦書での画像表示に対応
　- カバー画像と単ページ画像のスタイルシートの書き換え
　- prefix="ebpaj: http://www.ebpaj.jp/　に書き換え
1.1.0b52Q (2019/12/10)
　- 電書協の038a 「ぶら下がりインデントでの折り返し行頭字下げ」のスタイル位シートに近づけた
　- 左右中央表示のテーブルに設定を戻した。
1.1.0b51Q (2019/12/10)
　- kakuyomu.jp対応
　- 端末設定にkidle fireを追加
1.1.0b50Q (2019/05/06)
　- AdoptOpenJDKでビルドに変更
　- 左右中央表示のスタイルシートの変更
　- nav.xhtmlのテンプレートの変更
1.1.0b49Q (2018/11/17)
　- 「ファイル選択」からショートカットファイルの読み込みエラーの修正
1.1.0b48Q (2018/11/17)
　- なろうとノクターンで改行が増えていたのを修正
1.1.0b47Q (2018/11/16)
　- みてみん画像対応
　- 目次エラーの修正
　- openjdk-support
　- linux対応
1.1.0b46 (2016/06/17)
　- 「ノカケヵヶ」を漢字扱いしないように修正
　- nav.xmlのtitlepageを修正
　- Web小説取得時にCOOKIEを送信
　- Web小説のhttpsのURLに対応
1.1.0b45 (2015/04/20)
　- 割り注内に注記やルビがある場合の改行位置の調整
　- 割り注内に半角文字がある場合の改行位置の調整
　- 横書き時は縦書き向けの文字変換をしない
　- Webからの変換時に表紙指定が無視されるバグを修正
　- Webからの変換時にショートカットファイルと同名の画像ファイルを表紙に利用できるように修正
　- IVS外字注記リストを調整
1.1.0b44 (2015/03/05)
　- ルビの前が外字画像でルビ開始記号がなければ前にルビ｜を追加（1文字分のみ）
　- 横組みの位置を調整
　- 画像リサイズが多い時にメモリが肥大化するバグ修正(ImageWriterを毎回生成しない)
　- Rarで画像情報読み込みできないバグを修正
1.1.0b43 (2015/02/20)
　- 前方参照注記(複数)で後ろルビの位置を修正する処理のバグ修正
　- 前方参照注記の「」内に「」がある場合の処理修正
　　［＃「○○」に「××」の注記］の××側に「」がある場合は変換されない
　- ［＃注記付き］○○［＃「××」の注記付き終わり］の処理調整
1.1.0b42 (2015/02/17)
　- b34以降で、前方参照注記が複数あるとルビ位置がずれるバグ修正
　　※「[WARN]ルビが注記の後ろにあります」のログが出た場合のみ
　- chuki_ivs.txtでIVS指定になっているJIS漢字を置き換えてchuki_utf.txtに追加
　　※外字注記にJISコード指定が無い場合だけIVSで出力されてしまう
1.1.0b41 (2015/02/15)
　- 外字注記一覧を更新 ( http://kanji-database.sourceforge.net/aozora/gaiji.html 利用)
　- 濁点半濁点を１文字フォントで出力
　　ベースの文字は〓ではなく元の文字 (あ゛→<span class="glyph u3042-u3099">あ</span>)
　　フォントはglyphwikiから取得し、fontforgeで崩れ修正とウェイト調整
　　フォントファイルは gaiji/dakuten に配置
　- 「ばつ傍点」「×傍点」「左に～傍点」の注記に対応 → ※ばつ傍点があるとDigitalEditions3は強制終了する
　- 目次の <～> は img a タグのみ除去
　- 目次ページに正立のスタイル追加漏れ修正
　- ※［＃米印］のエスケープ処理を調整
1.1.0b40 (2015/02/08)
　- 濁点半濁点文字出力設定 (スタイルタブに追加)
　- IVSの出力設定 (スタイルタブに追加)
　　　IVS出力時は正立指定 (-epub-text-orientation:upright;)
　　　IVS文字用の青空外字注記変換表を追加(chuki_ivs.txt)＋UTF変換表との重複を調整
　　　IVSの出力または除外をログに出力
　- 外字１文字フォント( http://glyphwiki.org/wiki/ )をePubに組み込み
　　　本文内の文字に対応する1文字フォントファイル(u?????.ttf)が gaiji/ 以下にある場合
　　　　文字を〓にしてフォント指定のspanタグを出力 ( <span class="glyph u2496d">〓</span> )
　　　IVS付きの文字の1文字フォントも対応 (u?????-ue01??.ttf)
　　　※１文字フォントによっては上下に空白ができる場合有り → Fontforgeで調整が必要？
　- 4バイト文字の出力設定を削除(Koboの表示問題が解消したため)
　- Readerで正立しない文字を縦中横指定していた部分を正立指定に変更
　　　※Readerのファームアップで直ったがDigitalEditions向けに処理は行う (÷±∞∴∵ は正立指定のまま)
　- 拡張ラテン文字Aの定義をchuki_latin.txtに追加＋CID無しでもエラー出力しない
　- 青空特殊文字のエスケープ処理を調整（特殊文字の前後で自動縦中横されないバグを修正）
　- ルビの終了と開始が連続する場合は </ruby><ruby> タグは追加しない
　- 表紙画像が無い場合に入力ファイルパスに cover.png|jpg|jpeg のファイルがあれば確認画面で表紙に設定
　- JIS変換調整後に一部半角になってしまっていたバグを修正(1.1.0b39のみ)
1.1.0b39 (2015/02/01)
　- 濁点の結合文字は全角文字に変換
　- ひらカナ＋濁点半濁点で通常の濁点付き文字がある場合（がパ等）はその文字に置換
　- 割り注の先頭と末尾が〔〕と（）の場合は外に出す
　- 外字未変換時の小書き表示のずれを修正(letter-spaceing:-2px;を削除)
　- Webタブ追加
　　　取得間隔設定
　　　キャッシュ保存パス指定
　　　未更新時は変換スキップ
　　　変換対象の指定 指定話数+更新分
　- テキストエリアの右クリックメニューに「コピー」を追加
　- ファイルパス文字列の貼り付けでファイルの変換を実行
　- キャッシュパスのtxtファイル変換時はエンコードを一時的にUTF-8にする
　- ファイルとURL混在時に出力先が入力と同じ場合は先頭のファイルのパスに出力（キャッシュパスは除く）
1.1.0b38 (2015/01/25)
　- LICENSE.txt追加 (GPLv3)
　- 前方参照注記内の注記を除外
　　（［＃「～」は「第32［＃「32」は縦中横］図」を指す。］ → ［＃「～」は「第32図」を指す。］）
　- 画像キャプションを画像の下に表示
　　　キャプションがある場合は画像単ページ化は無効
　　　キャプションがある場合は高さは90%以下に調整
　　　キャプションが長い場合は画像倍率指定を有効にする必要あり
　- 画像倍率 画像ピクセルと画面ピクセルの比率で幅を％指定 (単ページ化時は無効)
　　　64px以下の画像は倍率は変更しない
　　　画面回転で縦横比が変わった場合は下にはみ出る場合あり
　- 画像単ページの「拡大表示」指定時にmobiで拡大されない不具合修正
　- 画像注記のキャプションに（）がある場合のファイル名取得を修正（後ろから）
　- 回り込み以外の画像のfloat指定 (Readerで画像前ページの空行が埋まる)
　- 回り込み時の画像の左右余白を0.5文字に設定
　- 回り込み画像が見出しをまたがないように調整
　　　見出し注記にclear:both追加＋１行の見出し注記をspanからdivに変更
1.1.0b37 (2015/01/23)
　- 出力先選択処理を調整 (空欄時のチェック等)
　- スタイルタブ追加
　　　vertical_text.css、horizontall_text.css を設定された内容で出力
　　　余白設定 (ReaderとKobo全画面(上下のみ)はhtmlのmarginを指定)
　　　行間設定
　　　文字サイズ調整
　　　太字注記、ゴシック体注記を太字ゴシックで表示する設定
　- 拡張子に .fxl.kepub.epub を追加
　- Kobo全画面用の拡張子と余白設定のプリセットを追加（左右余白は効かない）
　- Readerの目次で字下げ注記の見出しに移動できないバグを修正
　　（先頭の<span id="～"></span>の空タグに飛べなかった）
　- iniファイルのWebInterval指定が整数のみだったバグ修正
　- ペースト用の「貼り付け」右クリックメニュー追加
1.1.0b36 (2015/01/18)
　- ひらがな＋濁点/半濁点の表示を修正（縦中横ではなくpositionで重ねる）
　- 回り込み画像が重ならないようにスタイルのclearを有効化
　- 前方参照注記内の［＃「○○」に「××」の注記］の変換処理を修正
　- 出力先指定を「入力と同じ」はチェックボックスに変更
　- 拡張子「.mobi+.epub」でmobi変換前のepubも出力する
　- ブラウザからのzipのドロップはキャッシュパスではなく出力先のパスに保存
1.1.0b35 (2015/01/14)
　- b34のバグ修正
1.1.0b34 (2015/01/13)
　- ひらがな＋濁点/半濁点を縦中横表示(ずれ対策で半角文字を利用)
　- 罫囲みではみ出ないようにスタイル調整(display:inline-block;を削除)
　- ルビの文字種判別で漢字の間の「ノカケヵヶ」は漢字扱い
　- 前方参照型の後ろにルビがあったら前に移動
　- Rarファイル読み込み
　- 全画面表示(画像のみ 固定レイアウト+SVG画像タグ出力)
　- mobi変換は一時ファイルに出力してからリネーム(日本語ファイル名の対策 一時ファイルのepubは削除)
　- ファイルとWebの変換処理のSwingWorkerスレッドを1つに統合
　- ReaderT3のプリセットを追加
　- Web小説
　　　URL文字列(複数)のペーストまたは選択ドロップでの変換
　　　URL末尾の"/"漏れのチェックを修正
　　　キャッシュ内でフォルダが作れない場合は同名ファイルを削除
1.1.0b33 (2015/01/06)
　- epubcheck向けのePub定義のテンプレート修正
　- BOM文字除去
　- 異体字選択符号文字を除去(U+FE00～U+FE0F ※漢字以外)
　- Web小説周りの調整
　　　Web小説定義の追加と修正(なろう、暁)
　　　Web小説変換時は強制コメント出力
　　　本文が複数タグの場合は間に改行とセパレータを追加
　　　底本リンクの&を&amp;に変更
　　　個別ページ変換時も底本と変換日時を出力
1.1.0b32
　- 自動縦中横対象の前後の半角文字チェックをタグを無視するように修正
　- 見出し前方参照注記はブロック注記ではなくインライン注記に変換
　- 空行除去最大行設定のプロファイル保存修正
1.1.0b31
　- 目次階層していない場合にdtb:depthが設定されないバグ修正
　- Readerで字下げ時に自動改行されないバグ修正
　- 画像単ページと表紙のサイズ指定なし設定 (KindleとKobo用)
　- 表題の連続記号(―など)は短縮しない
　- 表題の前に発行者に対応
　- 確認ダイアログでメタデータにフリガナと発行者設定
　- 同行見出しも目次抽出対象にするチェック追加
　- Web小説定義フォルダ名変更 syosetu.org→novel.syosetu.org
1.1.0b30 (2013/03/12)
　- package.opfのguideを調整
　- package.opfのkindle画像metaを修正(画像解像度はコメント)
　- kindle目次はtoc.ncxを使うようにnavタグのepub:type="toc"指定を無くす
　- nav.xhtml内のlandmarksのずれ修正
　- kindle左右中央の行間が詰まっていたのを調整
　- kindleのテキストページはbodyタグにclass="kindle"追加
　- kindleのみ行間を0.5文字に (他は0.75文字)
　- 字下げ複合注記の横書きに対応
　- 連続する見出しを除外されなくなっていたのを修正
1.1.0b29 (2013/03/07)
　- nav.xhtmlの階層タグを調整＋landmark出力(Kindleのみ)
　　※KindlePreviewer2.8のNCX表示はKindle側の動作にバグ有り？
　- nav.xhtmlのスタイルと行間調整
　- toc.ncx内のタグ除去
　- 表題の有無でtoc.ncxの中見出しレベルがずれていたのを修正
　- コメント開始が10行目以降にあったらWARN出力
　- 左右中央の上paddingを0に修正(下がはみ出すため)
　- 「http」で始まるaタグはリンクで出力する
　- Web小説の最後のページに底本URLと変換日時を表示
1.1.0b28 (2013/02/18)
　- package.opf内表題ページのIDを title-page に変更 (metadataのtitleとID重複バグ)
　- ショートカットの拡張子の大文字に対応
　- kindle左右中央のはみ出し調整 (height:95%)
　- 目次の階層化設定
　　「目次ページ階層化」指定時は nav.xhtmlを1.0.7と同様に階層化
　　「目次(ncx)階層化」指定時はtoc.ncxを階層化 (Reader,Kindleのみ有効)
　　(※見出し以外のレベルは、数字は中見出し、他は大見出しと同じ)
　- ページ余白の上 0.5文字→0文字に変更 (右余白は0.5文字のまま)
　- コンソールからの表紙指定のパス調整
　- Web小説取得間隔指定 (現状ini編集のみ)
1.1.0b27 (2013/02/09)
　- 画像回転後に画面より横長の画像のアスペクトずれを修正
　- mobiでルビ内の縦中横で改行される対策でルビタグ内は改行しない
　- 長いルビは警告 (タグを1文字扱いで30文字以上）
　- KindlePWのプリセットの画面サイズを修正
　- 前後に改ページのある画像が単ページ化処理されていなかったバグ修正
1.1.0b26 (2013/02/07)
　- 確認画面の目次一覧で表題行の非表示設置が効かなかったバグ修正 (表題ページ出力時のみ)
　- 画像の自動単ページ化処置の後に改行が出力されていた
　- b25で表紙画像のitemを2つ追加していたバグ修正
　- kindleの［＃ページの左右中央］［＃ページの左］に対応 (横書きのページの左は未対応)
1.1.0b25 (2013/01/25)
　- zip内txtの場合に表紙の先頭の挿絵指定でエラーになるバグ修正 (b24のバグ)
　- 画像zipの場合に先頭画像が表紙にならないバグ修正 (b23-24のバグ)
　- 確認画面で挿絵以外の表紙画像が設定された場合、画像前後切り替えの先頭で選択できるようにした
　- 拡張子間違いの画像ファイルが確認画面でも表示されるように修正
　- Web小説取得
　　　表紙画像指定は本文に入れずにconverted.pngで保存 (表紙置き換え時に出力しない)
1.1.0b24 (2013/01/24)
　- 表紙の外部ファイル指定後の再変換で指定した挿絵と入れ替わるバグ修正
　- 64x64以下の画像は先頭の挿絵で表紙にしない (外字画像対策)
　- 表題が7行以上連続は6行の場合と同様の処理をする
　- 表題のみの取得で注記タグ除去忘れ修正
　- 表題+著者のみ(2行)の選択追加
　- Web小説関連
　　　タグが取得できない場合のエラーログ表示
　　　htmlファイル取得時のRefererに一覧ページのURLを設定
　　　本文にタイトルがない場合は一覧のタイトルを利用 (SUBTITLE_LISTで設定) → Hameln定義修正
　　　novelist.jp (http://novelist.jp/) 対応 (※2.novelist.jpも対応 ログインが必要なものは不可)
　　　dNoVeLs (http://www.dnovels.net/) 対応
1.1.0b23 (2013/01/21)
　- b22の地付き注記の修正は間違いなので元に戻す
　- 先頭の挿絵の有効な行数を指定
　- 横書きの表紙はKindle向けに位置を若干調整
　- ページ出力の表題のチェックなしなら表題文字は出力しない (「本文内」が以前のチェックなしと同等)
　　※プロファイルの表題ページの設定が変わる場合あり
1.1.0b22 (2013/01/19)
　- 地付き注記のタグが閉じないバグ修正 → 修正間違い
1.1.0b21 (2013/01/19)
　- b20で字下げ複合注記が変換されなくなっていた修正
　- 目次の表題チェックが効いていなかったのを修正
1.1.0b20 (2013/01/19)
　- 表題前の画像が出力されないバグ修正
　- 表題テンプレートでの外字画像、縦中横、訓点・返り点の注記は変換
　- 行頭10文字以前全角スペースは行末非表示処理しない
　- Web小説
　　文字取得時のinnerHTMLはparse後に文字列取得＋rtタグは除外
　　半角スペースのみの行が空行にならないのを修正
1.1.0b19 (2013/01/18)
　- 字上げの文字数が2倍になっていたバグ修正
　- タイトルが目次文字数で短縮されていたバグ修正
　- 確認画面の見出し種別で小が中になっていたバグ修正
　- 目次抽出時に記号の連続は1文字に短縮
　- 目次抽出で表題の出力選択
　- 表題をテンプレートで出力 中央寄せと横書き (template/OPS/xhtml/title_middle.vm , title_horizontal.vm)
　- kindle出力フラグが2回目以降の変換時に解除されないのを修正
　- タグの中で単ページ化しない場合はログにWARN出力
　- Web小説の文字取得処理を変更 (タグ内のinnerHTMLに対して置換処理後にタグを除去)
　　→ タグ前までの文字列取得だったのがすべての文字列の取得に変更 → 小説を読もうの定義修正
1.1.0b18 (2013/01/11)
　- 表題の前に改ページ注記があるとxhtmlエラーになるバグ修正
1.1.0b17 (2013/01/10)
　- 表題が改行されないバグ修正
　- 著者名の下の余白が出なくなっていたのを修正
　- 画像注記以外のzip内画像を表紙にした場合のバグ修正 (opfにitemが追加されない、画像に余白ができる)
　- urlショートカット内のURL文字列のtrim
　- プロファイルが1つの時に変更ボタンが押せないバグ修正
1.1.0b16 (2012/12/31)
　- Web小説取得時の改ページ注記前の改行漏れ修正
1.1.0b15 (2012/12/30)
　- 画像注記以外のzip内画像を表紙にした場合にepub側に入っていなかったバグ修正
　- 縮小サイズより大きい外部画像を表紙で編集したときに黒い余白ができるバグ修正
　- プロファイル
　　　タブの上に移動、順序変更、名称変更
1.1.0b14 (2012/12/28)
　- 窓見出し注記対応 (行頭のみ 見出し下は0.5文字の余白追加)
　- 「○○」に「××」のルビ 注記が行内に複数ある場合にずれるバグ修正
　- 「○○」に「××」の注記の出力設定(非表示orルビor小書き)
　- ルビ位置によって画面下にはみ出していたのを修正(ルビのnowrapをルビ内縦中横spanのnowrapに変更)
　- タイトルと目次の前後の記号除去を廃止
　- 端末プリセット選択
　- プロファイルの追加削除
　- UI調整 (アイコン追加他)
1.1.0b13 (2012/12/26)
　- ルビ内の特殊文字(《》｜等)のエスケープ処理修正
　- 見出しID設定用spanをinline-blockのdivに変更
　- 表紙設定の再利用(仮)
　　　確認ダイアログで変換orスキップした表紙の設定を利用(ファイル毎)
　　　※DB未実装のため再起動で履歴がリセットされるので注意
1.1.0b12 (2012/12/24)
　- 画像回り込みが効いていなかったのを修正＋横はみ出しに対応
　- 画像ガンマ補正追加
　- 表紙プレビューのキー操作追加＋「元画像出力」の選択状態を記憶
　- Web小説取得のルビ内の特殊文字エスケープ漏れ修正
　- コマンドラインで設定が反映されないバグ修正
　　　(表題のファイル名利用、表紙ページ追加、外字変換、自動縦中横)
1.1.0b11 (2012/12/21)
　- ルビの開始記号｜がある場合に間に注記を含んでもいてもルビがつくように修正
　- 目次の見出し内に特殊文字を含む場合のエスケープ処理修正
　- Kobo,Kindleの外字画像の位置ずれを調整
1.1.0b10 (2012/12/20)
　- 割り注注記に対応
　- cssの調整 (字上げと字下げのクラス名変更 画像単ページスタイル調整)
　- Web小説取得
　　　説明文が全文取得されないのを修正
　　　前書き後書きの開始終了位置指定できるようにした
　　　説明、前書き、後書きのhrは出力しない
1.1.0b9 (2012/12/16)
　- 確認画面目次一覧で非選択行はグレー表示
　- 確認画面目次一覧の一括設定がマウスオーバーで反応しないように調整
　- 目次の全角スペースが0x2000に置換されていたのを修正(Reader用設定時)
　- 画像単ページのスタイルを横書き中央寄せに変更
　- Koboで画面より小さい画像が拡大されるように修正
　- 余白除去 (ノンブルのサイズ指定 縦横比変更時の余白調整部分修正)
1.1.0b8 (2012/12/14)
　- 行頭字下げ時に画像の次に空白ページがでるバグ修正
　- フォントファイルがあれば一緒にePubに圧縮
　　　template/OPS/fonts/ 以下のファイルすべて
　- スタイルのカスタム設定ファイルがあればそちらを利用
　　　template/OPS/css_custom/ 以下の同じファイル名
1.1.0b7 (2012/12/13)
　- ルビ内の自動縦中横、縦中横注記内のルビに対応
　　　※縦中横のみの行＋ルビはReaderでルビ位置が左にずれる
　- ルビ開始記号省略の判別文字種調整 (漢字、半角英数字空白、全角英数字、ひらがな、カタカナ)
　- Web小説の本文開始終了タグ指定の修正
　　　http://syosetu.org/ 定義修正 (更新日時チェック、前書きなし、後書あり)
1.1.0b6 (2012/12/12)
　- 改ページ後の目次はアンカーのIDをつけない
　- 確認画面で目次種別一括選択
　- Web小説の一覧側の公開日を出力
　　　(不要ならextract.txtからCONTENT_UPDATE_LISTを削除(更新時の上書注意))
　- Web小説の文字列取得処理を修正
1.1.0b5 (2012/12/09)
　- 行頭字下げ調整 (例外文字に 〔【 追加)
　- 余白除去調整 (ノンブル誤認識調整)
　- Web小説取得時に改行が空白にならないように修正
　- 画像zipファイル名並び替えで大文字小文字を区別しない
1.1.0b4 (2012/12/08)
　- ブラウザからのDnDで出力先選択にならず2回変換されていたのを修正
　- 空行除去の場合は半角全角空白のみの行も空行扱いする
　- 余白除去調整 (ゴミ除外処理修正と縦横比が変わらないように下／左余白調整)
　- 前後改ページの画像が常に幅100%になっていたのを修正(縦横比で合わせる)
　- Web小説定義追加 (Arcadia http://www.mai-net.net/bbs/sst/sst.php)
　- バージョン番号を起動時にログ画面へ出力
　- 行頭字下げ機能
　　　行頭が全角空白,「,『,―,”,（,〈 以外なら全角空白を追加
　　　行頭の半角1～2文字は全角空白に置き換え
　- 画像回り込み設定UI修正
1.1.0b3 (2012/12/04)
　- 画像回り込み設定
　　※Readerでclearが正常に動作しないため未設定→連続すると重なる
　　※画面サイズより大きい場合ははみ出す
　- 画像自動回転
　- 画像設定画面調整 (縮小の画素数指定欄は無くした)
　- 余白除去修正(左右の下側の無視領域が広くなっていた)
　- Web小説取得時にリダイレクト後のURLを取得
1.1.0b2 (2012/12/02)
　- 画像zipの変換時のエラー修正
　- コマンドライン変換時のエラー修正
1.1.0b1 (2012/12/02)
　- 挿絵なしの設定追加 (表紙と外字以外の画像はePubに追加しない)
　- !? 1文字の縦中横の設定追加
　- 空行除去 (見出し後3行以内開始の空行は1行は残す)
　- GIF画像変更時に出力されないバグ修正
1.1.0a7 (2012/12/01)
　- 目次見出し内のタグはaとimg以外は消さない (<1>等は消さない)
　- 目次見出し内の《》が消えないようにエスケープ
　- Web小説対応
　　　ページ数からURL生成
　　　抽出置換パターン設定
　　　本文ノード内の開始終了タグ指定
　　　http://novel.fc2.com/ 対応
　　　http://syosetu.org/ 対応
1.1.0a6 (2012/11/30)
　- タイトル・目次に &<> がある場合エラーにならないようにエスケープ
　- 目次を階層化しない
　- 縦書き目次の自動縦中横
　- コマンドラインでのフルパス指定で実行対応
　- Web小説取り込み(仮)調整
　　　web定義修正(Elementの位置指定 表紙ID追加)
　　　http://www.newvel.jp/library/ 対応
1.1.0a4-5 (2012/11/29)
　- ［＃ここから○字上げ］独自注記対応 (地付きにせずに余白開ける margin-bottom)
　- Web小説取り込み(仮)調整
　　　DnDとファイル選択で複数のショートカット(.url)に対応
　　　ショートカット(.url)のDnDで出力先が同じ場所に対応
　　　リンクに対応する更新日時タグの比較で追加更新された物のみ取得
　　　変換済ファイル名変更 (index.txt → converted.txt)
　　　抽出的ファイルを利用 (web/ドメイン/extract.txt)
　　　挿絵対応 (外部ファイルのみ確認 キャッシュ更新チェック無し)
　　　短編に対応 (本文クラスが最初のページにある場合)
　　　Chapterの表示を調整
1.1.0a3 (2012/11/28)
　- 余白除去調整 (ノンブル側制限緩和 ゴミ除外処理修正)
　　　※大きなゴミのない縦書き小説なら概ね問題なさそう
　- 前方参照注記の対象の注記タグとルビ等の除外
　　　※動作確認中
　- 目次に特殊文字があると正しく文字が取れないバグ修正
　- Web小説取り込み(仮)
　　　※試験中 パラメータファイルは未使用 画像非対応
　- ［＃区切り線］独自注記対応 上下0.5文字空きのhrタグ表示
1.1.0a2 (2012/11/26)
　- 前方参照注記の対象に ［ が文字としてある場合のエラー対処（ ］は未対応）
　- 目次一覧で種別表示
　- 目次の次の行を繋げる処理に見出しは使わない[1.1.0a1]
　- 表題が目次に入っていなかった[1.1.0a1]
　- xhmlt内のIDを常に1～
　- 余白除去(仮)調整 （ノンブル除去 ゴミ除外(0.5%)）
1.1.0a1 (2012/11/25)
　- 半角と漢字連続時のルビ開始位置バグ修正
　- 目次取得処理を初回の読み込み時に行う
　- 確認画面でタイトル再取得
　- 確認画面で目次の一覧表示、選択、名称変更
　- 確認画面のプレビューを少し大きく

----
[1.0.7]
1.0.7u1
　- 表紙関連
　　　サイズが3:4でない場合に実サイズに合わせてプレビューとダイアログ幅を可変
　　　幅調整で位置がずれるバグ修正
　　　Ctrl左右で幅調整 Ctrl+Wheelでズーム倍率を小さく
　　　表紙プレビュー2倍表示(仮)
　- 縮小時にjpeg圧縮率の指定が効いていなかった
　- 縮小時のpng保存修正
　　　2値縮小時の4bitインデックスの値修正
　　　jai-imageioがインストールされている場合にCLibPNGImageReader/Writerは使わない
　- UbuntuとMacのDnD操作に対応
　- ログ削除時にクリップボードにコピー
　- ログの行番号を1～開始に修正
　- 画面調整 (上下をSplitでサイズ変更可能に テキスト幅をフォントサイズで調整)
　- Kindle関連
　　　kindlegen.exe(またはkindlegen)がjarと同じパスにあれば変換後実行
　　　※画像のみのZipではKindle全画面用のepubを出力するので変換後要削除
　　　kindlegen.exeがある場合表紙はjpegで保存

1.0.6→1.0.7での主な変更点 (2012/11/19)
　- 画像サイズに応じて単ページ化＋画像の縮小
　- 表紙プレビューと編集
　- Readerで横倒しになる文字の強制縦中横追加 (Koboの正立参考 黒丸文字等は除く)
　- 目次の抽出 (見出し注記＋パターン)
　- 強制改ページ設定
　- コメントフロック出力
　- 縦書き時の横組み注記対応 (Koboのみ)
　- 縦書き時の横書き注記対応 (Kobo,Kindleのみ)
　- zip内複数ファイル対応
　- プログレスバーと変換中の中断
　- Windows以外はJavaの標準Look&Feel(Metal)に
　　(Ubuntu12はDnDできない以外はOK  Macは動くらしいが詳細不明)
　- コマンドラインオプション追加 (細かい設定はiniから取得)

----
Release (2012/11/19)
　- 表紙プレビュー周りの修正
　- タイトル左右中央時に前後のブロック注記でxhtmlエラーを修正
　- タイトルや目次に｜が残るバグ修正
　- 上付き下付文字のサイズを50%→66%に変更
　- ファイル名からタイトル取得時の()内の除去を特定文字に限定
　- 目次抽出の章見出し対象を調整
　- プログレスバーの値ずれ修正
b29-30 (2012/11/18)
　- プログレスバー修正(zipのtxtで重複画像がある場合に100%にならない)
　- 表紙幅調整機能のバグ修正 (縦が指定表紙サイズと同じ場合に幅調整が効かない)
　- Zipテキストで画像注記にないzip内の画像も選択可能に
　- 余白除去後の余白量設定
　- txtzはzipと同様に処理 (txtzの詳細仕様不明なのでとりあえず)
b27-28 (2012/11/17)
　- プログレスバー (テキスト10行毎に+1 ,画像出力毎に+10)
　- 変換中の処理注意
　- 余白除去機能（仮）テスト中
b26 (2012/11/16)
　- 画像ePubのnav.xhtmlのリンクにページ番号のアンカーがついていたのを修正
　- 自動改ページのサイズ指定を、各行、空行、見出し毎に指定
　- zip内の複数のテキストファイルをすべて変換
　- コマンドライン修正 (オプション指定, iniファイル指定, 画像zip変換対応, zip内複数テキスト)
　　※コマンドラインオプション以外の設定はiniファイルから読み込み
b25 (2012/11/15)
　- 改ページ前の［＃ここで字下げ終わり］注記の省略でエラーにならないようにした
　- ［＃ページ左］［＃ページ左寄せ］［＃ページ左下］(表記揺らぎ含む)注記に対応
　- 折り返し字下げ内の縦中横の表示不具合対応
b24 (2012/11/15)
　- Windows以外のLook&FeelはMetal+Plainフォントにした
　- 見出しの次の行も繋げて目次に出力
　- 目次抽出でのその他パターン(正規表現)指定
b23 (2012/11/14)
　- 表題に<img>タグが残るバグ修正
b22 (2012/11/14)
　- 外字画像を文字サイズにあわせた (class="gaiji")
　- 目次設定タブ追加と設定項目追加
b21 (2012/11/13)
　- 見出し自動抽出処理調整 （ローマ数字に対応 数字前後の条件を調整)
　- 連続した見出しの除外処理で消えすぎていたバグ修正
b19-20 (2012/11/10)
　- nav.xhtmlのidに番号がついていなかったバグ修正
　- 連続した見出しは目次に入れない (目次ページ等の自動抽出対策) (抽出見出しが３つ以上連続(１行空き含む)の場合）
　- 目次の階層化 (nav.xhtmlのみ) → Kobo目次機能では効果なし？
　- ブロック見出し注記の強制改ページ対応（その前の行にブロック字下げ等あると効かない）
b18 (2012/11/09)
　- 表紙画像拡大時にキーで移動
　- Readerで横倒しになる文字の強制縦中横追加 (Koboの正立参考 黒丸文字等は除く)
　　(©®⁑⁂◐◑◒◓▷▶◁◀':♤♠♢♦♡♥♧♣☖☗☎☁☂☃♨▱⊿✓␣⏎♩♮♫♬ℓ№℡ℵℏ℧)
　- 目次に表紙を入れる設定(詳細設定の目次出力) ※表紙画像がある場合のみ
b17 (2012/11/08)
　- 割り注があると末尾に1が表示されるバグ修正 (chuki_tag.txtのタブ位置ずれてた)
　- Readerで横倒しになる他の文字も強制縦中横 (数学記号は一部のみ)
　　(☆★♂♀♪♭§†‡÷±∀∞∴∵‼⁇⁉⁈)
　- 縦書き時の横組み注記対応 (Koboのみ)
　- 縦書き時の横書き注記対応 (Kobo,Kindleのみ)
　- 「表紙」は目次に入れない
　- 小さい文字の倍率調整
　- ６段階の文字の倍率調整
b16 (2012/11/07)
　- 強制改ページのバイト数取得修正(UTF-8指定漏れ)
b15 (2012/11/07)
　- 目次出力設定 (数字+章名)
　- 強制改ページ設定 (分割バイト数調整中)
　- △▽▲▼を強制縦中横
　- ブラウザからのzipのリンクDnDで変換 (キャッシュファイル(.cache以下)は終了時に削除)
　- ［６段階大きな文字］［６段階小さな文字］注記に対応（大きさは５段と同じ）
　- 画面に入りきらないので最小幅を広げた
b14 (2012/11/03)
　- Java7で動かなかったのを修正
b13 (2012/11/02)
　- gitHubでGebner氏の修正をマージ (mimetypeはSTOREDで圧縮 他)
　- 表紙サイズ設定が使われていなかったのを修正
　- 表紙幅調整周りを修正(強制的に縦に合わせる、幅に合わせたら幅調整なし)
　- 3文字の!?も自動縦中横
　- 3文字の半角数字も自動縦中横
　- 目次出力設定 (改ページ後、各見出し注記) 仮(第～、その～、数字のみ)
　- 目次最大文字数設定
b12 (2012/10/05)
　- コメントブロックの出力とブロック内注記変換設定
　　(注記変換しない場合も < > & は常にエンコード)
　- 前後に改ページのある画像が常に拡大されていた
　　→画像単ページの拡大オプションに従うようにした
　- 縦に合わせて表紙幅を狭くした場合の横オフセットが効いていなかったのを修正
　※表紙プレビューの幅調整が実際の画像表示と合わない場合があるのは要調整
b11 (2012/09/21)
　- 画像zipの変換で縦長画像が縦に合っていなかったのを修正
b10 (2012/09/20)
　- 文中全角の処理を調整
　　(Koboで文中全角の行末で非表示が追い出しになっていたのでReaderと設定を分けた)
b9 (2012/09/20)
　- 文中全角の行末で非表示対応は0x2000+0x2002の空白2文字に変更(Readerに対応)
b8 (2012/09/20)
　- 文中全角の追い出しと行末で非表示(Koboのみ)の設定を「詳細設定」タブに追加
　　行末で非表示の場合、Readerでは禁則処理されないが表示は問題なし
　- 自動縦中横の設定を「詳細設定」タブに追加
　- 数字1桁の縦中横設定(前後は全角)
b7 (2012/09/17)
　- 画像設定の画面縦横比を画面サイズに変更（設定忘れで値も使われていなかった）
　- 画像単ページ化の時に小さい画像を画面サイズに拡大表示する設定項目追加
　- 表紙の画像の幅を狭くできるようにした
　- 文中の全角スペースの禁則を追い出しになるように調整 (Reader対応のため)
　　(全角1文字のみ 全角スペース前がタグでない場合)
　- 目次内全角スペースが半角にならないように修正
b6 (2012/09/16)
　- 読めないJpegと色がおかしくなるJpegがあるのでJAIを利用 (lib追加)
　- 目次内全角スペースが消える → 半角で表示
　- 文中の全角スペース(1文字のみ)の禁則を調整 (行末は0.5文字分のみ表示)
b5 (2012/09/16)
　- 4bit以下のPNGは縮小後に4bit(グレー16階調)で出力
　- 8bitPNGの縮小後は元画像と同じColorMapで出力
　- 文中の全角スペース(1文字のみ)は折り返しでの禁則されるようにした
　　（行末の全角スペースと前の文字は送り出される (ルビと縦中横内除く)）
b4 (2012/09/15)
　- Zipからのpngファイル読み込みエラーを修正 (ImageIOがZipのストリームを直接readできない)
　- 4bitPNGは8bitPNGで出力(24bitPNGになっていた) (ImageIOで4bitは判別不可？)
　- jpeg圧縮率と画質が逆じゃなかった（開発環境のみなぜか逆になる）
b3 (2012/09/15)
　- 表紙で指定したファイル名がプレビューに表示されていなかった
　- jpeg圧縮率と画質が逆だった
　- ×傍点を文字数が同じルビに (前方参照注記のみ例外対応)
b2 (2012/09/14)
　- 前方参照注記内の｜で1文字ずれるバグ修正(半角|になってた)
　- 表紙や出力先のパスが長いと画面からはみ出すのを修正
　- 確認画面にスキップ追加
b1 (2012/09/14)
　- 画像の前に改ページがある場合に改ページ目次が出るように修正
　- 字詰めの中に罫囲みがある場合のみ罫囲みを字詰めの高さにする
　　（罫囲みの中に字詰めは文字の高さになってしまう）
　- １行に複数の画像がある場合に画像単ページ化されるよう修正
　- 「画像設定」タブパネルで画像処理用の値を設定可能に
a10 (2012/09/13)
　- コメント行判定を「-」50文字以上に変更 (文字数が若干足りないものが多いため)
　- ［＃「」に「」のルビ］の注記に対応
　- 画像の横550px以上は単ページ化 (Readerではみ出るため 400x600以上とは別の幅のみの条件)
　　→ サイズは設定可能にする
　- 表紙の縮小を縦または横が100%までに制限
　- 拡大縮小ボタン画像入れ忘れ
a9 (2012/09/12)
　- 表紙画像なしの場合に確認画面表示後に変換されないバグ修正
　- 注記付き注記をルビに変換
　- ①～㊿をローマ数字と同様に縦中横
a8 (2012/09/12)
　- 初回変換時確認画面が出ないバグ修正
　- 表紙トリミング時の保存画像フォーマットをjpgに (pngだと大きくなりすぎるため)
a6-7 (2012/09/12)
　- 前方参照注記内のルビは無視して処理
　- 表題前に表紙以外の画像がある場合に表題左右中央指定が効かないバグ修正
　- 表紙が縦長画像の場合は縦に合わせる
　- 画像取得周りのソースの整備
　- 確認画面での表紙のトリミングと表紙画像前後変更(要UI調整)
a5 (2012/09/07)
　- 目次スタイル微調整 (行間0.5文字)
　- 左右中央の表紙ページがあれば目次はその後に追加
　- 目次の縦書き横書き指定
　- 確認画面での表紙プレビューとDnDでの設定 (トリミング操作用に大きめに表示)
a4 (2012/09/06)
　- 目次を横書きにしてスタイル調整
　- 目次ページ出力設定
　- 画像ePubの時にテキスト用cssファイルは出力しない
a3 (2012/09/05)
　- 拡張子cbzは画像ePubに変換
　- 画像サイズが指定より大きければ縮小 (※縮小前の画像は保存されない)
　　→縦1600見開きだとReaderで表示できない対策(Koboは表示可)
　- 縮小サイズの指定UI (横、縦、画素数で最小になる倍率を利用)
　- ボタンのアイコン変更
a2 (2012/09/04)
　- zip内サブフォルダの下にtxtがある場合の画像サイズ取得を可能に
　- 縦横比の比較の値が整数になっていた
　- 横書き時の左右中央スタイル修正
　- 横書き時の画像の中央寄せを縦書きのスタイルと同じに(横書きだとリサイズがうまくいかない)
a1 (2012/08/31)
　- タグの階層取得とチェック (出力時のバッファ内のタグの開始と終了のカウント)
　- 画像縦横比による自動幅調整 (画像が横にはみ出る対策)
　　　(幅600以上で横/縦=3/4ならwidth:100%; height:auto;)
　- 指定サイズ(現状400x600固定)以上の画像は単ページ化
　ｰ 単ページ化した画像の後に改ページ注記がなければ次の目次は出さない

----
[1.0.6] - date: 2012/09/04
b50-52 (2012/08/31)
　- 字下げエラーになって字下げされないバグ修正
　- 表題取得で3行の時の副題優先取得オプション
　- 画像zip変換でcssが足りていなかったのを修正
b49
　- 改ページ後にbrタグが出ていたのを修正
　- 表題のタグがpの中にならないように変更
　- 出力先が無い場合にフォルダを作成するか確認
　- 確認ダイアログで次以降の変換前確認を設定
　- 出力先もファイルまたはフォルダのDnDで設定可能に
　- 他UI調整
b48
　- 画像が前にあると表題がエラーになるのを修正
b47
　- 改ページ後の改行が消えるバグ修正
　- 目次に画像ファイル名またはタイトルは出力しない
b46
　- 改ページ後の改行pタグ出力がおかしかったのを修正
　- フォント用cssを分離 (Readerでのフォント指定用)
b45
　- 改ページ処理を調整
　　　最初の文字やタグ出力時に改ページ処理
　　　空行はカウントして文字やタグ出力時にまとめて出力 (ページ最後の改行は出力しない)
　　　連続改ページ等での空ページは無視される (連続改ページする場合は全角スペース等入れる必要有り)
　- 2桁元号で1桁目のみ縦中横になっていたのを修正
　- 数字1文字の縦中横条件調整 (年1月 月2日 第3刷 第4版 第5巻)
　- 表題取得処理調整 (3行の場合2行目先頭が"―"でなく3行目が"訳""編纂""校訂で終われば2行目が著者)
　- ブロック注記とインライン注記のdivとspanの調整
b44
　- 字下げ字詰め注記で字詰めにならないバグ修正
　- 太字とゴシック体注記スタイル調整
　　　Koboデフォルトフォント時 → ゴシック太字
　　　Kobo他のフォント → 太字
　　　Reader → ゴシック
　- 元号の後の半角数字を縦中横
　- 「年」と「月」の間の半角数字は縦中横
　- 表題と著者を左右中央で表示 (調整中 表紙画像がある場合等)
b43 (2012/08/25)
　- ゴシック体注記対応 (Koboはデフォルトフォント時のみ有効 太字にはならない)
　- 小書きスタイル調整
　- 「ここから改行天付き、折り返して○字下げ」の「ここから」なしも対応
　　（ブロック注記扱いで次の字下げで自動で閉じる [林不忘]安重根 のみ？）
　- 外字が4バイト文字のログに出力
　- 4バイト文字の変換指定＋未変換時は注記表示
　　(Koboは4バイト文字以降行末まで表示されなくなる 2バイト文字は表示できないが文字は消えない)
　　(Readerは4バイト文字でもJIS漢字なら表示可でそれ以外も後ろの文字は消えない)
　- Zipファイル内にローマ数字があるとエラー (Zipファイルエンコード指定を"Shift_JIS"→"MS932"に変更)
b42 (2012/08/24)
　- 複数のtxtファイルの連続変換ができなくなっていたのを修正
　- 「」の含まれる前方参照注記に対応 (［＃「魔境「蕨の切り株」」は中見出し］)
　- 小書き注記対応 (［＃「○○」は小書き］)
　- 訓点返り点追加 (［＃二レ］)
　- 画像単一ページの画像位置を左右中央寄せに
b41 (2012/08/24)
　- 縦横中のタグをdivからspanに変更 (WebKit系対策)
　- 画像のタグをdivからspanに変更 (WebKit系対策)
　- 画像単ページのファイルが無い場合に目次が出ないように修正
　- 表題取得処理調整 (5行: 表題,原作表題,副題,著者,訳者)
　- 底本：自動改ページ時に前の空行を除外
　- 注記で目次が切れないように修正
　- 拡張ラテン文字注記でない〔〕を出力して内部を外字変換
　- 出力先を変換時にリストに追加 (存在しなければ追加しない)
　- コメントが短い場合にWRAN
b40 (2012/08/23)
　- 注記内の外字注記が2つ以上の場合のエラー対策
　- 縦横中変換調整 (ルビ内は適用しない等のエラー対策)
　- ローマ数字がルビ内で表示されなくなったのを修正 (ルビ内は横向き)
　- 半角スペースの前後も半角なら自動縦中横を無効に
　　(英文での誤変換防止 全角スペース区切りなら縦中横になる)
　- 画像が無い場合はimgタグを出力しない
　- 拡張子自動修正 (png, jpg, jpeg 小文字のみ)
　- １ページ目に本文がなければ目次はタイトル文字列
　- SwingWorkerでの別Threadでの実行と実行中のUIのDisable
　- 表紙画像をファイルのDnDで設定
　- 表紙画像のブラウザからのDnD動作調整 (現状末尾画像拡張子のURLのみ)
　- 表紙画像指定時に先頭画像が表示されないバグ修正
b39 (2012/08/22)
　- 《》の代替文字の前後の半角数字2文字が縦中横になるように修正
　- ローマ数字が縦中横内になければ強制縦中横
　- 1月1日のような日付表記は数字1文字も縦中横
　- 表紙画像を0000.jpg/pngにしてzip扱い時に先頭に来るようにした
　- zip画像のみの場合は画像ePub作成(仮)
　　 (リサイズ等無し Koboスクロールテスト中(なぜか左が切れる 横書き×))
b38 (2012/08/20)
　- 注記内外字は変換後に注記がつかないようにする
　- 訓点返り点追加(四,丁)
　- 単一画像ページの100%指定がされなくなっていたのを修正
　- 画像指定外字注記は画像注記に変更
　- 文中の画像は改行されないようにスタイル調整 (Koboのみ右寄せになるのは調査中)
　- 縦中横下の文中画像がずれないように調整
b37 (2012/08/15)
　- 取り消し線 二重は普通の取り消し線で代用
　- 著者名の下の余白が正しく出ていなかった
　- コメント警告行数を21行以上に変更
b36 (2012/08/15)
　- 底本の目次が出ないように修正
　- コメントが閉じていないor長すぎる場合警告表示
b35 (2012/08/15)
　- 半角＆の変換漏れ
　- 見出し終わり注記のログ出力抑制 （インライン注記で閉じていない場合用にコメントアウトしていたため）
b34 (2012/08/14)
　- 変則注記にさらに対応
　- ログ出過ぎなので明確な非対応注記は出さない
　- ［＃字下げ終わり］に対応
b33 (2012/08/14)
　- 画像は拡張子の . がある物のみ
　- 字下げ複合注記で開始していなかった場合に字下げ終了タグを出さない
　- 字下げが閉じていない場合等のエラーをログに表示 (xhtmlエラーの可能性有り)
　- ［＃ここから○字下げ。］も判別
　- 破線罫囲み、枠囲み、破線枠囲みに対応
　- 変換エラー確認用に未変換の注記をすべてログに出力
　- 返り点前方参照注記に対応
　- 「底本：」前に改ページがなかったら改ページ（目次には表示しない）
b32 (2012/08/14)
　- 改行のみの行が出ない場合があったので改行をpで括る
　- 表題取得を青空文庫記載事項に合わせ、本文中のスタイルも調整
　　(表題 原題 副題 副原題 著者名 訳者名 / 表題 副題 著者名 訳者名 / 表題 副題 著者名 / 表題 著者名)
b31 (2012/08/13)
　- 複合字下げ注記終わりでのエラー対応 (［＃ここで字下げ、罫囲み終わり］等)
b30 (2012/08/13)
　- 出力先パス履歴(最大10件)
　- 先頭画像が表紙で表示出力で画像単ページの場合に空ページが出ていたのを修正
　- imgタグで src=画像ファイル.jpg のように"か'で括られていない場合に対応
　- ファイル名の拡張子より前に . がついていた場合に対応
b29 (2012/08/12)
　- 入力ファイルのサブフォルダ以下すべてのファイルに対応
　- 字下げ複合注記に対応 (字下げ、罫囲み、中央揃え)のみ
　- 罫囲みの高さが常にページ下までになっていたので文字に合うようにスタイル調整(display:inline-block)
b28 (2012/08/12)
　- ページ左右中央じ地付き地上げのスタイル調整
　- cssファイルの共通部分分割
b27 (2012/08/11)
　- 先頭が画像＋改ページの場合、先頭画像を表紙ページで出力すると空ページができるバグ修正
b26 (2012/08/11)
　- 地付き、地上げが効かなくなっていたのでスタイル調整
b25 (2012/08/11)
　- ページの左右中央注記に対応
　- 改ページ前の空白行を除去 (余計な空白ページがでないように)
　- 禁則処理での下の空行をなくすため p {text-align: justify;} を追加
　- 文字列置換 (本文とルビに適用) の置換前文字を２文字まで対応 (replace_sample.txtをリネームして利用)
b24 (2012/08/09)
　- 文字列置換設定ファイル(replace.txt)追加 (本文とルビに適用)
b23 (2012/08/08)
　- 傍線スタイルをundreline→border-right/leftに変更 (二重線・破線・点線対応)
　- 画像注記エラー処理調整 (注記内で（が閉じていない場合)
　- 出力先パス指定
　- 表紙ページがあれば目次に「表紙」追加
b22 (2012/08/07)
　- 文字置換 (<<>>＜＜＞＞を《》に 3個以上はそのまま)
　- 文字置換（“”を〝〟に XMDF用に逆に変換していたのは修正）
　- Kobo栞用IDを行のpにつける (栞が数行ずれる場合があるが少し軽量化)
b21 (2012/08/06)
　- 表紙ページ追加で先頭の挿絵を利用した場合は本文中から削除
　- 画像にmax-height:100%(横書きならmax-width:100%)を設定して大きい画像に対応 (横に長いと左がはみ出る)
　- cssのclass文字数を減らした
　- 余計な br や p が出ていたのを修正
b20 (2012/08/05)
　- 表題下のコメント行処理Bugfix
　- 地付き地上げスタイル調整
b19 (2012/08/05)
　- ファイル名からタイトル取得でのNullPointer例外を修正
　- 表紙に入力ファイルと同じファイル名(拡張子以外)の画像を利用
　- 訓点送り仮名に対応
　- 画像ページは画像注記のタイトルまたは<imgタグのaltを目次に設定
b18 (2012/08/04)
　- 改行を<br/>から<p></p>括りに変更 (kepubだと特に変わらず)
　- ページの左右中央で余計な改ページが出ていたので改ページなしに
　- 2行目がコメントブロック-54文字になら著者は取得しない
　- ファイル名文字制限エラー対策で256文字以下に(著者名max64文字)
　- toc.ncxで空ページのChapterの制御文字が出ていた
b17 (2012/08/04)
　- ページ余白を@pageで指定 (余白0.5文字(左は0) Readerのルビ欠け対策)
b16 (2012/08/04)
　- 表紙ページ出力(仮)
　- 強制改ページ機能(未完成)を無効に
b15 (2012/08/03)
　- ここで字下げ終わりの複合注記に対応
b14 (2012/08/03)
　- 確認ダイアログ調整
　- toc.ncx出力
　- 画像単ページの目次をファイル名に
　- 中央揃え注記(仕様外)に対応
　- 訓点(返り点)注記に対応
　- 画像注記は . がなければ訓点送り仮名
　- 表示できない外字は小書きで注記を表示
b13 (2012/08/03)
　- 画像単ページ調整 (［＃（画像.jpg）］注記がマッチしていなかった)
b12 (2012/08/02)
　- 表題の確認ダイアログ表示
　- 表題行が「表題＋著者名」の場合は3行以上なら2行目を副題にする
　- 字下げ折り返しの文字数設定間違い修正
b11 (2012/08/01)
　- ePubの最新仕様に合わせてメタデータ等調整 (参考にしたePub3が古かったため)
　- 画像単ページ時に画像全体表示用スタイル適用
　　(上下の行が［＃改ページ］で挟まれている画像注記、先頭行の画像は下が［＃改ページ］のxhtmlのみ)
　- タイトル取得と画像単ページ判別の前処理の修正
　- UTF-8以外の外字はルビに注記表示
b10
　- <IMG SRC= の大文字表記にも対応
　- 字下げの複合注記は、字下げのみ最低限処理してxhtmlエラーを回避
b9
　- "<"→"&lt;" ">"→"&gt;" にすべて置換 (「<メールアドレス>」等の記載に対応)
　- <a .*></a>タグ削除
　- ファイル名からタイトルと作者指定 ("[著作者] タイトル (青空文庫).zip")
　- 目次(仮) (本文先頭行＋改ページ後の先頭本文で設定(Max64文字))
　- 折り返し字下げ注記で2行目以降のインデントずれを修正 (各行を<p></p>で括る ブロック注記の行は括らない)
　- 字詰めスタイル調整 (divに字詰め文字数のmax-height指定)
　- 複合注記［＃ここから○字下げ、○字詰め］［＃ここから○字下げ、罫囲み］対応
　- 改ページ処理の改行を出力しない 画像の改行も無くして<div><img></div>に
　- kepub栞対応 (拡張子.kepub.epub時のみ)
　- 表紙ファイル指定 (ファイル選択,URL,先頭の挿絵, 表紙なし)
　- 出力ファイルを setWritable(true)
　- コマンドラインからの実行に対応(仮) (引数 ファイル複数 オプション未対応)

----

[1.0.5u1] - date: 2012/07/24
　- 改ページの後ろの改行が次ページの先頭に出ていたのを修正
[1.0.5] - date: 2012/07/24
　- 注記対応 (字詰め、罫囲み、字下げ内の罫囲み)
　- タグを p から div に変更してスタイルも調整
　- 閉じていない［＃見出し］注記のタグエラー対策に必ず１行で閉じる (［＃見出し終わり］は無視)
　- 画像を含むzipファイルに対応
　- コマンドラインからの実行に対応(仮) (引数ファイル名1個のみ)

[1.0.4u1] - date: 2012/07/23
　- 小見出し注記でのタグ設定間違いのみchuki_tag.txt修正
[1.0.4] - date: 2012/07/22
　- 傍線スタイル調整
　- 縦書き横書き切り替え設定
　- 外字注記 UCS-コードに対応 (U+と同じ)

[1.0.3] - date: 2012/07/22
　- 縦中横、圏点スタイル調整 (-webkit -epub 記述追加)
　- 訓点が画像として扱われてしまったのを修正 (１文字なら訓点)
　- 拡張子を選択式に
　- Windowサイズを記憶
　- 圧縮率を調整 (画像は非圧縮)
　- nav.xhtml(仮)を出力

[1.0.2] - date: 2012/07/22
　- スタイルの width:100% 削除
　- すべての画像にカバー画像指定が入っていたのを修正 (先頭のみ設定)
　- 画像注記 ［＃（表紙.jpg）］ が読めていなかったのを修正
　- Window位置を記憶

[1.0.1] - date: 2012/07/21
　- スタイルのフォント色と余白を調整
　- zip内のtxtファイル１つのみ変換に対応 (zip内画像、複数txtは未対応)
　- 出力ファイルの拡張子指定

[1.0] - date: 2012/07/21
　- AozoraXMDFの注記設定を変更してePub3対応版を作成
　- Zipアーカイブ形式でePub3ファイル一式を出力

