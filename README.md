# じゃんけん

## index.html
- コンソールに以下のように出力するじゃんけんプログラムです
    `index.html`を開いたら、コンソールを開いてください
    https://i.gyazo.com/b469e7465bd8d6feaa072a034395b3cd.png
    ※フォントの関係で✌（ちょき）だけ小さな文字になっています
    
    コンソールで以下のような表示が行われます。
        ```
        じゃんけん...ぽん！
        PLAYER1:✌ PLAYER2:✋
        PLAYER1の勝ち！
        ```
- 再度プレイするにはブラウザーをリロードします

- グーチョキパーの絵は絵文字を使用して表現します
    const hand = ['👊','✌','✋']   // それぞれの絵文字は「ぐー」「ちょき」「ぱー」の変換で出る(Google日本語入力の場合）
- PLAYER1とPLAYER2は両者ともコンピューターで、ランダムな手による全自動の戦いです
    ランダムに👊✌✋を決めるのは、次のコードを使用します
        const player1 = hand[Math.floor(Math.random()*3)]
    これで player1 に'👊','✌','✋'のどれかが割り当てられました
- PLAYER1とPLAYER2のどちらが勝ったかの判定は次のようにします
    ```
    if( player1 === player2 ){
        console.log('あいこ')
    }else if( player1 === '👊' && player2 === '✌'){
        console.log('PLAYER1の勝ち！')
    ...(続く)
    ```

## index2.html

コンソールではなく、画面上に結果を表示するようにします。
https://i.gyazo.com/51d7914019d991622200d128f9b03107.png

## index3.html

絵文字ではなく、画像素材を使用して以下のような表示にします。
https://i.gyazo.com/c7d4482e48a429b0989d565afa86b648.png

画像素材は「かわいいフリー素材集　いらすとや」の以下のものを使用してください。
https://www.irasutoya.com/2013/07/blog-post_5608.html


