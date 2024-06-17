> 以下の内容はあくまで参考です。ここまでのものを作るという意味ではないので、注意ください。内容的にもでっち上げに近いです（提案内容に影響を与えないためです）。ただし、作成する内容や筋を通すことは重要です。  
> また、例として記載しているのは、1章以降は全て「こういうことを書くと良い」というもので、同じように書くだけでは、説明が不足していますので注意して下さい（このエリアは削除してください）

# 0. タイトル
**説明:** 企画名や班番号、チームメンバーの列挙（学籍番号、名前）をしてください。企画名は、プロジェクトの目的や内容を端的に示すと良いでしょう。また、副題でアプリ名を追加することも考えられます

- **例:**
  - **企画名:** スマートホーム環境の実現に向けたM5Stackユビキタス環境の開発
  - **班番号:** RWC24-group00
  - **チーム名:** あればぜひ書きましょう
  - **チームメンバー:**
    - 2312110000：近大 マグロ
    - 2312119999：近大 タイ
    - 2312111111：近大 ナマズ
    - 2312112222：近大 クエ
    - 2312113333：近大 マンゴー

# 1. 前期役割分担

**プロジェクトリーダー**  
- 田中 太郎: プロジェクト全体の管理、進捗確認

**デザイナー**  
- 近大 タイ: ユーザーインターフェースの改良、ユーザビリティテスト。なおサブリーダーも兼ねるため、リーダーの業務について把握しつつ、欠席の際には作業を代替した。

**プログラマー**  
- 近大 ナマズ: 新機能の実装、バグ修正
- 近大 クエ: 新機能の実装、バグ修正
- 近大 マンゴー: 新機能の実装、バグ修正

# 2. システム化の背景
**説明:**  
ここでは、なぜこのシステムが必要かを説明します。現在の課題や問題点を明確にし、それを解決するためにIoT技術をどう活用するかを述べます。この背景説明は、システムの目的（次章）が妥当なもの（確かにそのアプリがいる）ということを示す基礎となります。  
また、M5Stackの技術調査も含めてください。M5Stackの利用は課題上必須です。

## システム化のニーズ / シーズ
スマートホーム技術の普及により、より効率的で快適な生活環境の実現が求められている[^1]。例えば〜

## 関連するサービス
Google Home[^2]やAmazon Echo[^3]などが既に市場に存在するが、特定の機能やカスタマイズ性において不足している点がある。具体的には〜

## M5Stackの技術調査
M5Stackは多機能なIoTデバイスであり、センサーやモジュールを簡単に接続できるため、スマートホームシステムに適している。例えば今回の提案においては〜〜

# 3. システムの目的
**説明:**  
後述の概念設計と合わせて、要件定義に該当します。前節の背景に基づきながら、開発するアプリが持つべき特徴についてまとめてください。5W1Hに基づいて説明することが望ましいです。  
これは、「想定している顧客」に、「誰（何）が、いつ、どこで、何を、何故、どのように提供するか」を整理することで満たしてください。この際、顧客の抱える課題を、前述のシステム化の背景と関連づけて説明することも重要です。

**例**  
忙しい共働き家庭や、高齢者のいる家庭である。これはシステム化のニーズ / シーズともこのように関連しており、温度調節や照明制御、セキュリティシステムを統合したアプリケーションを提供することで、このような価値を生み出す。  
具体的に、まず忙しい共働き家庭では、これが、こういったタイミングで、この場所で、これを、このように提供できます。これにより、このような価値が提供され、要件を満たします。

# 4. システムの概念設計
システムの外部仕様設計のラフになります。前述の要求を受けて、機能やシステム構造を具体化してください。内容としては、実装のアウトラインを述べ、その詳細を説明する形で、画面レイアウト（UI/UX含む）や、利用する機器、技術・ライブラリ、システム構成図を用意し、これらについて解説してください。

## 画面レイアウト
UIの図を貼り、その説明を記載してください。説明には、それぞれの画面でユーザにどのような意図で何を提供するかを、要件と結びつけながら説明してください。UIやデバイスごとに、節を分けても問題ありません。モックアップの図をそのまま用いてください。

## システム構成図
**説明**
システムのそれぞれのセンサーやM5Stack、サーバーシステムなどの要素が、他とどういう関係性にあるかを図で示してください。今回は簡易的で良いので、以下のサイトのような記載を検討してください。  
https://blog.soracom.com/ja-jp/wp-content/uploads/2021/02/fig01.png

画面レイアウトと対応づけた説明をすることも心がけてください。

## 利用する機器
**説明**
利用する機器と、その説明を記載してください。画面レイアウトと関連づけて説明すると良いです。

**例**  
- M5Stack   
  M5Stackとは〜〜。今回は温度センサのために〜〜。モーションセンサーにおいても〜〜。
- Raspberry Pi  
  Raspberry Piとは〜〜
  
## 利用する技術・ライブラリ
- MQTTプロトコルを使用してデータを送信  
  MQTTプロトコルとは〜〜
- AWS IoTを使用してデータを管理  
  AWS IoTとは〜〜
- Pythonを用いたデバイス制御プログラム  
  Pythonとは〜〜

# 5. 主要なプログラムの解説
**説明:**  
提案するアプリの特に主要な機能について、「具体的にこうやれば実装できそう」というところまで調べたという説明を記載してください。具体的にはソースコードを抜粋しても良いですし、図を用いて説明しても構いません。主要な機能ごとに節を分けて記載してください。もちろん、引用は必須になります。  
ソースコードを用いた説明は必須ではありませんが、本ドキュメントを見るだけで、確かに実装を前提としてしっかり調査をしているとわかる（すぐに開発に移れる）ことを示すようにしてください。

## 温度センサーのデータ取得プログラム（例）
DHT11は低価格で購入できる温湿度センサーであり、本システムではこのセンサを活用することを前提とする[^5]。このソースのサンプルを以下に示す。記述の意味は〜〜。よってこの方法を用いれば、温度センサーの活用理由であるこれこれを満たせると考えた。

```python
import RPi.GPIO as GPIO
import dht11
import time
import datetime

# initialize GPIO
GPIO.setwarnings(True)
GPIO.setmode(GPIO.BCM)

# read data using pin 14
instance = dht11.DHT11(pin=14) # GPIO14を使用

try:
    while True:
        result = instance.read()
        if result.is_valid(): # データを正常に取得できたら
            print('Last valid input: ' + str(datetime.datetime.now()))
            print('Temperature: %-3.1f C' % result.temperature)
            print('Humidity: %-3.1f %%' % result.humidity)
            
        time.sleep(6) # データ出力間隔

except KeyboardInterrupt:
    print('Cleanup')
    GPIO.cleanup()
```

# 6. 後期の役割分担

**プロジェクトリーダー**  
- 田中 太郎: プロジェクト全体の管理、進捗確認

**デザイナー**  
- 近大 タイ: ユーザーインターフェースの改良、ユーザビリティテスト。なおサブリーダーも兼ねるため、リーダーの業務について把握しつつ、欠席の際には作業を代替した。

**プログラマー**  
- 近大 ナマズ: 新機能の実装、バグ修正
- 近大 クエ: 新機能の実装、バグ修正
- 近大 マンゴー: 新機能の実装、バグ修正

# 7. 後期作業のガントチャート
**説明**
ガントチャート（英語：gantt chart、gantt diagramm）は、さまざまなプロジェクトやプログラムに使用され、生産管理・工程管理などに用いられる表の一種です。詰まるところ、誰がいつまでに何やるリストで、他のタスクとの兼ね合い（こちらが終わらないとこちらが進められないなど）も一見して確認できるようにするための表です。  
一般的に、ガントチャートは棒グラフを用いたチャートで、縦軸にはWBSを元にしたタスクや担当者を、横軸には日時や進捗率を記します。各タスクから横長の棒グラフ（ガントバー）が伸びており、作業の進捗や期間を示しています。    
以下に、上記の説明（やや加筆しています）も含まれた説明がありますので、参考にしてください。  
https://www.jooto.com/contents/what-is-ganttchart/

本授業においては、Google Spreadsheetのテンプレートにガントチャートがありますので、そちらを活用していただければ良いです。  
https://www.jooto.com/contents/spreadsheet-gantt/

# 8. 参考リスト
**説明:**  
参考文献をこちらにリストアップしてください。Webサイトに限らず、書籍等も記載してください。書き方は１年次の基礎ゼミの図書館の利用説明でもあったこちらの資料を参考にしてください[^4]。他についても、Web等で調べると出てきます。  
この箇所のフォーマット上、おそらく分割線が二重になりますが、今回は気にしなくて大丈夫です

**例**  
[^1]: 石橋 大右．“生活をより快適で便利にするスマートホームとは？”．和上ホールディングス とくとくマガジン．2024-05-24．https://wajo-holdings.jp/media/2233 ，（参照 2024-10-01)．
[^2]: Google．“Google Home"．https://home.google.com/welcome/ ，（参照 2024-10-01)．
[^3]: Amazon．“Echo & Alexa”．https://www.amazon.co.jp/b?ie=UTF8&node=5364343051 ，（参照 2024-10-01)．
[^4]: 近畿大学中央図書館レファレンス課．“引用と参考文献の書き方”．近畿大学．2022-05-01．https://www.clib.kindai.ac.jp/search/pdf/guide_quote.pdf ，（参照 2024-10-01)．
[^5]: りょうのすけ．“【DHT11の使い方】Raspberry Piで温度と湿度を取得する方法”．e-DIY．2022-05-17．https://ediy-fan.com/dht11/ ，（参照 2024-10-01)．