# クラス図を作ってみよう

source: `{{ page.path }}`

前章でプロジェクトを作って準備が整ったので、ここから本番です！

##  クラス図の追加
メニューより「図」→「クラス図」を選択し、クラス図を作るためのキャンバスを作成します。

<center>
<img src="../1_scrum/img/img7-2.png" width="80%"></img>
</center>

## クラスの追加
クラス図を作るためのキャンバスを作成したら、クラスを追加してクラス図を作成します。

1. クラスを選択します。
1. キャンバスをクリックしてクラスを配置します。
1. 「クラス0」と書かれている部分をクリックするとクラス名を自由に変更できます。ここでは 「LEDTank」とします。

<center>
<img src="../1_scrum/img/pic4.png" width="80%"></img>
</center>

<center>
<img src="../1_scrum/img/pic5.png" width="80%"></img>
</center>

## ライブラリの追加
次に、ライブラリを追加します。今回の事前実習で記述するのはLEDTankのモデルです。これは、LEDTankのアプリケーション部分を司る部分となります。

実際のアクチュエータの駆動や、センサ情報の取得などの動作は実行委員の用意したControllerが行います。Controllerはすでにコードが存在するため、コード生成を行う必要はありません。そこで、ライブラリであることを表すステレオタイプ<<lib>>を指定する必要があります。<<lib>>が指定されたクラスは、コード生成時にコード生成されません。

1. 先ほど「LEDTank」クラスを追加した手順と同じように、「Controller」クラスをクラス図に配置します。
1. 次にステレオタイプを追加します。先ほど作成した「Controller」クラスを選択します。
1. 左側のビューのステレオタイプを選択します。
1. 追加をクリックします。
1. 「lib」と入力します。


図のように、「Controller」クラスの名前の上に「<<lib>>」と表示がされればステレオタイプの設定は終わりです。

<center>
<img src="../1_scrum/img/pic6.png" width="80%"></img>
</center>

<center>
<img src="../1_scrum/img/img7-3.png" width="80%"></img>
</center>


##  関連の追加
クラス図における「関連」とは、そのクラス間で参照があるかどうかを表します。ここでは「LEDTank」クラスは「Controller」クラスを参照し、「Controller」クラスに定義されている関数や変数を用いて制御を行います。つまり、「LEDTank」クラスの中で「Controller」クラスのインスタンスを生成し「LEDTank」はこれを用いてセンサやアクチュエータの制御を行います。

1. 関連を選択します。
1. 「LEDTank」と「Controller」を接続します。

<center>
<img src="../1_scrum/img/pic8.png" width="80%"></img>
図：クラス図とモデル図の例
</center>


## 変数の追加
LEDTankは進んだ距離と、旋回した角度の情報を元にどのような動作状態となるかを決定します。
そのため、LEDTankクラスにdistance（距離）と、angle（旋回角度）の2つを追加します。

1. LEDTankクラスにdistanceのメンバ変数を追加します。LEDTankクラスの黄色のひし形をクリックします。
1. 左のビューに追加するメンバ変数の名前を設定できるので distanceとします。distanceはfloat型とします。

同様に、以下の図のようにangleも追加します。型はfloatです。

<center>
<img src="../1_scrum/img/pic_hen1.png" width="80%"></img>
</center>

<center>
<img src="../1_scrum/img/pic_hen2.png" width="80%"></img>
</center>

次の章よりステートマシン図を書いていきます！