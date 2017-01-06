---
layout: post
title: HTML5の新しい属性「contentEditable」
---
このページ、なんか変だと思いませんか？

実は、投稿の部分が編集可能になっているんです！  
試しに、投稿の中の適当なところをクリックして、バックスペースで消してみると、その通りに文字が消えていきます。

使い方は、

```
<div contentEditable="true"></div>
```

こんな感じです。すごく簡単です。ちなみにこのページでは、jQueryで指定した要素にcontentEditable属性を追加しています。
これ、Webサイトを印刷するときに広告を消してから印刷するみたいな目的に使ったりできそうです。
<script>
  $(function(){
    $('.content').attr('contentEditable', 'true');
  });
</script>
