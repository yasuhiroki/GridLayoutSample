# GridLayout Sample

GridLayout の height wrap_content が思ったとおりに動作しないと思って作った検証用リポジトリ。  
ちなみに原因は GridLayout ではなく、親Viewの PgaeView が layout_height の wrap_content をサポートしておらず、子View の height から自分の height を計算する仕様がなかったせいだった。
