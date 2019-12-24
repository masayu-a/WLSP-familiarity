# WLSP-familiarity

## Description
『分類語彙表』増補改訂版データベースに対して、クラウドソーシングにより親密度情報・位相情報を付与したもの

## Features 

### wlsp-fam.txt.gz
ベイズ推定前のファイル

1行目がヘッダ。

- 1列目：文字刺激の単語
- 2列目：分類語彙表情報
- 3列目：観点 (KNOW, WRITE, READ, SPEAK, LISTEN)
- 4列目：単語ID (WID)
- 5列目：実験協力者ID (SID)
- 6列目：評定値 (1-5)

### bunruidb-fam.csv
ベイズ推定後のファイル

1行目がヘッダ。

- 1列目：レコードＩＤ番号
- 2列目：見出し番号
- 3列目：レコード種別
- 4列目：類
- 5列目：部門
- 6列目：中項目
- 7列目：分類項目
- 8列目：分類番号
- 9列目：段落番号
- 10列目：小段落番号
- 11列目：語番号
- 12列目：見出し
- 13列目：見出し本体
- 14列目：読み
- 15列目：逆読み
- 16列目：「知っている」評定値
- 17列目：「書く」評定値
- 18列目：「読む」評定値
- 19列目：「話す」評定値
- 20列目：「聞く」評定値
- 21列目：「生産」評定値
- 22列目：「受容」評定値
- 23列目：「書記」評定値
- 24列目：「音声」評定値
- 25列目：「生産-受容」評定値
- 26列目：「書記-音声」評定値


## Author
- 浅原正幸 (国立国語研究所)

## References 
Masayuki Asahara (2019) Word Familiarity Rate Estimation Using a Bayesian Linear Mixed Model, 
Proceedings of the First Workshop on Aggregating and Analysing Crowdsourced Annotations for NLP, pages 6–14.
https://www.aclweb.org/anthology/D19-5902.pdf

浅原正幸 (2020) Bayesian Linear Mixed Model による 単語親密度推定と位相情報付与, 『自然言語処理』, 27(1), To Appear.

## License
CC BY-NC-SA 3.0 https://creativecommons.org/licenses/by-nc-sa/3.0/deed.ja

## Credit
National Institute for Japanese Language and Linguistics (2019) WLSP-familiarity (ver. 1.0)

## Contact
kotonoha@ninjal.ac.jp
