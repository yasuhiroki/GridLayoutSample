# GridLayout Sample

GridLayout の layout_height wrap_content が思ったとおりに動作しなかったので作った検証用リポジトリ。  
ちなみに原因は GridLayout ではなかった。当該のレイアウトは ViewPager を親Viewに持っていて、その ViewPager は標準では layout_height の wrap_content をサポートしておらず、子View の height から自分の height を計算する仕様がなかったせいだった。
