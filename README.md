# WLSP-familiarity (version 4.0) (2024/06/30)

## Description
『分類語彙表』増補改訂版データベースに対して、クラウドソーシングにより親密度情報・位相情報を付与したもの

## Features 

### bunruidb-fam.csv
ベイズ推定後の単語親密度推定値 (平均 0.0, 分散 1.0 の正規分布)

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

### subjrate.txt
ベイズ推定後の実験協力者の語彙力の推定値 (平均 0.0, 分散 0.5 の正規分布)

1行目がヘッダ。

- 1列目：実験協力者ID
- 2列目：回答数
- 3列目：語彙力評定値

## Changes

### version 3.1 から version 4.0 における変更 (2024/06/30)
- 2018年から2023年の 18,686,785 データポイントについて再推定

### version 3 から version 3.1 における変更
- 欠損値 84519「同意する」を補完したうえで再推定

### version 2 から version 3 における変更
- 「表層形＋分類語彙表番号」についての親密度ではなく、**「表層形」のみについての親密度**に変更しました（多義語の扱い）
- 2021年データを追加しました
- 150回答未満の実験協力者は継続して排除します。
- 実験協力者 6732人分の語彙力を推定します (subjrate.txt)
- 単語親密度の評定値を平均 0.0, 分散 1.0 の標準正規分布、実験協力者の語彙力の評定値を平均0.0, 分散 0.5の正規分布として推定します
- 区切り記号に対しては評定値が含まれておりません
- ※84519「同意する」が欠損値です

### version 1 から version 2 における変更
- 2018年のデータに追加して、2019年・2020年のデータを追加しました
- version 1 において評定値が割り当てられていなかったもの（欠損値）についても推定値を割り当てました
- 150回答未満の実験協力者のデータを排除しました
- 実験協力者 5000人分の語彙力を推定しました (subjrate.txt)
- 単語親密度の評定値を平均 0.0, 分散 1.0 の標準正規分布、実験協力者の語彙力の評定値を平均0.0, 分散 0.5の正規分布として推定しました
- 区切り記号に対しては評定値が含まれておりません
- ※84519「同意する」が欠損値です

## Author
- 浅原正幸 (国立国語研究所)

## References 
Masayuki Asahara (2019) Word Familiarity Rate Estimation Using a Bayesian Linear Mixed Model, 
Proceedings of the First Workshop on Aggregating and Analysing Crowdsourced Annotations for NLP, pages 6-14.
https://www.aclweb.org/anthology/D19-5902.pdf

浅原正幸 (2020) Bayesian Linear Mixed Model による 単語親密度推定と位相情報付与, 『自然言語処理』, 27(1), pp.133-150, https://doi.org/10.5715/jnlp.27.133

## License
CC BY-NC-SA 3.0 https://creativecommons.org/licenses/by-nc-sa/3.0/deed.ja

## Credit
National Institute for Japanese Language and Linguistics (2021) WLSP-familiarity (ver. 3.0)

## Contact
kotonoha@ninjal.ac.jp
