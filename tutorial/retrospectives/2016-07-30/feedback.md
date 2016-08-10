# フィードバック

初メンターだったmtsmfmにやってみてどうだったか聞いた。聞いた内容とそれを受けて今後どうした方がよさそうかという案をまとめる。

今回、mtsmfmが担当したビギナー2人は「使ってみても気になったところが見つからなかった・詰まったところがなかった」と「時間内にフィードバックできなかった」というよくある難しいパターンだった。

「使ってみても気になったところが見つからなかった・詰まったところがなかった」ビギナーの話を聞いてみると、「カレントディレクトリーの実行ファイルの仕方がわからなことがあったのでそれはやり方を教えた」とのことだった。

おそらく、ビギナーの作業ログだとこのあたりの話。

https://github.com/oss-gate/workshop/issues/90#issuecomment-236337259

> 作業:実行の仕方が分からない。
> 思っていること:もうしわけない、メンターさん。

https://github.com/oss-gate/workshop/issues/90#issuecomment-236337396

> 作業:「./perl -v」で実行。
> 思っていること:できた
> 備考:パスが通ってない場合は明示する。

進行役の説明では、気になったところ・詰まったところに気づく例として「ググった」・「わかりにくかった」あたりだけを説明した気がする。しかし、↑の例のように「メンターに教えてもらった」も詰まったところのサインの1つなのでそれも説明した方がよさそう。

ただ、そうやっていくとあらゆるサインを説明することになりキリがないので、別の対応も検討したほうがよさそう。

今回、サポートメンターには「ぶらぶらして随時メンターをサポートしてください」のようにざっくりとした行動指針で動いてもらったのが、もう少し「ここは必ず押さえるポイント」を共有したほうがよいかもしれない。

たとえば、↑の対策として、午前の「まず動かす」時間の途中（1時間とっているので40分くらい経ったらとかがよさそう）で、サポートメンターが順にすべてのビギナーをまわって、「どんな感じ？」と午前の部の最後の「ふりかえり」のようなことをするのはどうか。初メンターが気づけないような「フィードバックチャンス」でもサポートメンターなら気づけるのではないか。

「ふりかえり」では担当のメンターと違うメンターに作業内容を説明する。この中で担当していたメンターが気づかなかったフィードバックチャンスでも他のメンターが気づけるのではないか（フォールバック？バックアップ？として機能するのではないか）と期待していた。しかし、今回のようにメンターがほぼ初メンターという場合はそれは難しそうである。そのため、「ふりかえり」の前にサポートメンターが一通り確認することで「まず動かす」フェーズでのフィードバックチャンスが1つも見つからない、を防げないだろうか。

（サポートメンターはビギナーのいう「全部すんなりいきましたねー」を信じてはいけない。ビギナーはフィードバックチャンスを見つけるという経験がほぼないはずなので見つけられないことの方が多いはず。）

また、もし、サポートメンターが見ても本当にフィードバックチャンスが0だった場合は、ここで対象OSSを変更する機会にするといいかもしれない。たとえば、Railsを対象としていたけどフィードバックチャンスが0だったのでRails関連のgemにする、とか。これが回るなら、最初に対象OSSをいい感じに決める、というのを頑張らなくてもよくなる。これまでどおりビギナーがやりたいものをやろう！でよくなる。やってみて、フィードバックチャンスがなかったら後で（やり直せる時間のうちに）変更できるからである。

なお、↑でサポートメンターがフォローするのはどうかと書いた内容（フィードバックチャンスの発見・対象OSSの変更）を初メンターに求めるのはやめた方がよいと思っている。そこまで求めるとメンターの敷居が高くなるからである。当日、事前準備なしで参加してもちゃんとビギナーをフォローできるワークショップの内容を維持したい。


「時間内にフィードバックできなかった」ビギナーの件は、「まず1つフィードバックしてみよう」というやり方で対応できないだろうか。たとえば、100点のフィードバックを目指さずに、まずは60点のフィードバックで出して、時間があれば追加のコメントで質を上げていく、といったやり方や、まずはissueで報告して、時間があればpull requestで修正もつけるといったやり方である。

該当の初メンターが、100点を目指しすようにビギナーを誘導したために時間内にフィードバックできなかったというとそういうわけではないが、時間配分が難しかったという感想を聞いたので、フィードバックするための情報をどこまでするか、どこで打ち切るかの判断は初メンターには難しそうである。なぜなら、一回もこのワークショップを通しで経験したことがないからである。（初メンターなので当然である。）

このあたりもサポートメンターが途中で全ビギナーの様子を確認することでフォローできないだろうか。午前の「まず動かす」フェーズと同じことを午後の「フィードバック」フェーズでもやろうということである。「フィードバック」フェーズは1時間30分から2時間を確保しているので1時間経ったら回り始めるとかでどうだろう。

サポートメンターなら残り半分の時間でフィードバックできそうかどうかを判断できると思うので、時間が足りなそうなら「いろいろやりたいことはあると思うけど、今日は○○だけに集中してフィードバックを経験してみましょうか！」とできるのではないか。


あと、進行時の説明資料の「まず動かす」フェーズと「フィードバック」フェーズのそれぞれの説明のところに、メンターが目指すことを明示したほうがよさそう。

まず動かすフェーズのところは以下の通り。

  * フィードバックチャンス（自分が詰まったところ、わかりにくかったところ、ググったところ、メンターに教えてもらったところ）をビギナーに気づいてもらうこと
    * たとえば、メンターが「あれ！？いま詰まったよね！？どうなったら詰まらなかったと思う？これってフィードバックチャンスじゃない？」と言えば気づいてもらえる
  * フィードバックチャンスは自分が気づいていないだけで実はいろいろあったということに気づいてもらうこと（あれ、これ、↑と同じこと？）

フィードバックフェーズのところは以下の通り。

  * 時間内にビギナーにフィードバックすることを経験してもらうこと
    * ただし、メンターが先回りしていろいろ教えてビギナーが単にそれに従うだけだとビギナーの経験が少なくなるので、「教える」じゃなくて「一緒にやる」やり方でフォローする。
    * 100点のフィードバックじゃなくてもよい。60点とかからはじめて、追加情報で質を上げていく方法だってあるから。100点を目指して時間内にフィードバックできないよりは、60点でも時間内にフィードバックできた方がよい。（ビギナーの経験という観点でもフィードバックをもらうOSSとしても。バグの存在を（めんどくさくなって）報告してもらえない（とかTwitterでグチって終わりになる）よりは、多少雑でも報告してもらえたほうが助かることが多い。情報が足りなかったら追加でやりとりすることもできるし。）