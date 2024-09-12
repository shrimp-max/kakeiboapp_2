# ①課題番号-プロダクト名

家計簿webアプリ

## ②課題内容（どんな作品か）

- phpMyadminを使って、収支を投入できる
- 投入した収支を一覧で確認できる

## ③DEMO

https://ebitaku.sakura.ne.jp/kakeiboapp/index.php

## ④作ったアプリケーション用のIDまたはPasswordがある場合

なし

## ⑤工夫した点・こだわった点

- これまでの課題よりも実用的にするために、きれいなUIを心掛けた
- 収支一覧表の、収入と支出を一目見てわかるように色を付けた

## ⑥難しかった点・次回トライしたいこと(又は機能)

- DBは作成済みなので、カテゴリや財布の選択肢を自分で追加できるようにしたい
- 絞り込み機能を実装するにあたり、select文を入れてみたが、以下のエラーが出てしまい、取得したいカラムがundefinedとなってしまった。
  - :Undefined array key "syushi" in C:\xampp\htdocs\kakeibo\kakeiboapp\insert.php on line 6
- 各レコードに編集ボタンを設置して、投入後の編集を可能にしたい（SQLのupdate,delete?)
- 別ページに収支のグラフを挿入したい（chartjsのリベンジ）

## ⑦質問・疑問・感想、シェアしたいこと等なんでも

- [質問]
- 更新画面（detail.php）に遷移する際に、もともと入力していたデータを保持させる必要がある。<br>```<select><option>```でリストから選択するものを保持させる方法について、```<?=$v["category"]=="食費" ? 'selected' : '' ?>```のように、要素を直打ちして条件式を書くのではなく、関数を使って書きたかった。要素（"食費"）を取得するには、どんな式を書けばよいのかがわからなかった。
- [感想]
- 
- [参考記事]
  - 1.三項演算子 [https://www.sejuku.net/blog/23070]
  - 2. チェックボックスのchecked属性をphpで受け取る方法[https://magazine.techacademy.jp/magazine/19671]
  - 3. textareaはvalue属性が使えないので、開始終了タグの間にぶっこむ話[https://qiita.com/Kent2525/items/b07bb3fb2b521fce580d]
  - 4. 4. Chartjs使用時のReferenceError: Chart is not defined が出たときの対処法[https://harutoblog.com/1733]
# kakeiboapp_2
