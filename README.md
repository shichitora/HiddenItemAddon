# 隠しアイテムアドオン

Minecraft Bedrock Edition向けの「隠しアイテム」に特化した外部アドオン

---

# 概要

隠しアイテムをインベントリに追加したり、独自のコマンドからNBT改変限定アイテムや、隠しエンティティ、隠しパーティクルなども出せるようになります。
また、他エディションのアイテムなどの再現も追加されています。

---

# 機能

1. インベントリ上に「隠しアイテム」や「隠しブロック」を追加します。
2. 新たに**別Edition**や**削除された**アイテムやブロックを再現して追加します。

   ※再現アイテムはインベントリのカテゴリに再現アイテムであることが明記されています。(スポーンエッグは例外)

3. 独自のコマンドを追加します。
   - **/getnbtitem**: NBT改変限定の隠しアイテムを追加します。
     * 構文: `/getnbtitem <"selector:string"> <nbtitem:string>`
   - **/gethiddenitem**: NBTアイテム以外のGiveで出せない隠しアイテムを出せます。
     * 構文: `/gethiddenitem <"selector:string"> <hiddenitem:string>`
   - **/summonhiddenmob**: 隠しエンティティを召喚します。
     * 構文: `/summonhiddenmob <hiddenmob:string> <xyz:float|option>`
   - **/hiddenplace**: 隠し建造物を生成します。
     * 構文: `/hiddenplace <hiddenstructure:string> <xyz:float|option>`
   - **/sethiddenblock**: 隠しブロックを設置します。
     * 構文: `/sethiddenblock <hiddenblock:string> <xyz:float|option>`
   - **/lore**: 手に持っているアイテムの説明文を編集します。
     * 構文: `/lore [set/clear] <string:string|option>`
   - **/name**: エンティティの名前を強制的に変更します。
     * 構文: `/name <entity:target> <string:string>`
   - **/fire**: エンティティを強制的に燃やします。
     * 構文: `/fire <player:target> <int:int>`
   - **/heal**: エンティティのHPを変更します。
     * 構文: `/heal <entity:target> <int:int>`
   - **/remove**: エンティティの存在を消します。
     * 構文: `/remove <entity:target>`

   ※まだありますが、めんどくさいので省きます。
   ※追加されたコマンドは`sctr`の名前空間でも追加しています。

4. 統合版にはない、隠しパーティクルや、隠しエンティティを追加します。
5. カスタムディメンションを追加します。
6. Giveなどのコマンドの変換に隠しアイテムを追加します。

---

# ダウンロード

[こちら](https://github.com/shichitora/HiddenItemAddon/releases)から最新バージョンをダウンロード
