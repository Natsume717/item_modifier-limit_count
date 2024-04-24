# item_modifier-limit_count
item_modifierの1項目であるlimit_countに関するサンプルになります。

詳しくはブログ記事『[【マイクラ】limit_countでアイテム数を調整する【item_modifier】](https://natsumake.com/item_modifier-limit_count/)』を参考にしてください。

<h3>概要</h3>
アイテムのスタック個数を制限（変更）することのできるitem_modifierの項目。<br>
適用時の所持している個数によっては、その所持数を変更する場合もあります。

<h3>使い方</h3>

データパック導入後、ワールドに入った後```/reload```と打って実行してください。

4種のアイテムが付与されますが、それぞれを手に持った状態で以下のコマンドを実行することで、所持数が変わります。

```copy
/item modify entity @s weapon.mainhand sample:limit_count
```

```copy
/item modify entity @s weapon.mainhand sample:limit_count_range
```

1つ目のコマンドはスタック数を100にします。<br>
ほとんどのアイテムが64個までしか持てませんが、それを無視して1つのスロットに100個持った状態にできます。

2つ目のコマンドでは、15個から30個の間で所持数を制限します。<br>
※最低値と最大値で、適用時に持っていた個数に近い方の数に調整される。

16～29の間だった場合には、所持している数の変化は起きません。
