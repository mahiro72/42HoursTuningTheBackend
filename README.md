# 42時間耐久パフォーマンスチューニング
<div align="center">
<img src="./document/img/title.png" alt="属性" title="タイトル">
</div>

___

優勝しました！！
チームの勝利👑

<a href="https://twitter.com/DreamArts_PR/status/1515585442200301570">
  <img src="https://user-images.githubusercontent.com/70263039/163705428-427f318f-068a-40d6-af21-428d0675cde3.png" >
</a>


## 役割分担：
- ynakamot：リーダー、データベース、backend全般
- myoshie：データベース関連（インデックス追加、クエリ改善）
- xizhu：ログ関連、画像関連

## 取り組んだ内容：
- 環境構築
    - local環境のjsのホットリロード（nodemon）
    - 計測、ログ出力（slowquery、Performance、alp等）
- 改善
    - MySQL
        - インデックスをはる
        - tomeActive等のメソッドのクエリを効率化（for文の中のクエリを単体のクエリする）
        - max connectionsを増やす
    - backend
        - 逐次処理の並列化（Promise)
        - 画像圧縮、IOの高速化
    - nginx
        - 特になし

___
<br>

競技参加者は、初めに[document](./document)を参照してください。

## ディレクトリ構成
```
.
|- debug/           # 運営者デバッグ用(非公開)
|- development/     # 開発用リソース置き場
|- document/        # 競技に関するドキュメント
|- local/           # ローカル実行関連
|- provisioning/    # 競技環境構築関連(運営者向け)
|- scoring/         # 採点関連モジュール
```

<br>
<br>
