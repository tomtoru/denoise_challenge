# ノイズ除去の検討

### Outline
ノイズ除去についての試行と備忘です。  
換気扇の音が含まれた単一話者の話し声において、  
なるべく話者の声を損わずに換気扇の音を除去する方法を検討します。


### Notebook

| No. | 手法 | ノイズ除去 | 音質 | 備考 |
| --- | --- | --- | --- | --- |
| 01 | 周波数フィルタ           | △ | △ | - 処理は容易 |
| 02 | wavelet                | △ | △ | - 使いこなせてない感がある |
| 03 | スペクトルサブトラクション | ○ | ○ | - 少し声が濁る印象 </br> -  ノイズの箇所が分かっている必要がある |
| 04 | ウィーナーフィルター      | ○ | ◎ | - 加工後の音質に違和感が少ない </br> - ノイズの箇所が分かっている必要がある |


### Data
'data/noisy_voice.wav'
