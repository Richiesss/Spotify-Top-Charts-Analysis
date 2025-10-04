<h1 align="center"> 📈 2000-2019 Spotify トップチャート分析 📈 </h1>
このプロジェクトは、音楽統計データセットに対して分析を実行し、過去20年間の音楽トレンドとその変遷を理解することを目的としています。

<h2 align="center"> データセット </h2>

Kaggleの[*Top Hits Spotify from 2000-2019*](https://www.kaggle.com/datasets/paradisejoy/top-hits-spotify-from-20002019)。これは2000-2019年の各年のトップ100トラックの20列を含み、合計2000トラックが含まれています。列にはアーティスト名、トラック名、リリース年、テンポ、時間、ジャンル、インストゥルメンタル度などが含まれます。

<h2 align="center"> コード </h2>

- [**Audio_Summary_Visualized.ipynb**](https://github.com/hina0830g/Spotify-Top-Charts-Analysis/blob/main/Audio_Summary_Visualized.ipynb) <br>
Kaggleデータセットを読み込み、データをクリーニングし、新しいデータセット（pandasデータフレーム）を作成します。最後に、seabornを使用して4つのパラメータ（テンポ、時間、キー、ジャンル）の統計を表示する4パネルプロットを作成します。
- [**Time_Series_Analysis.ipynb**](https://github.com/hina0830g/Spotify-Top-Charts-Analysis/blob/main/Time_Series_Analysis.ipynb) <br>
Audio_Summary_Visualized.ipynbによって作成された[データセット](https://github.com/hina0830g/Spotify-Top-Charts-Analysis/blob/main/Top_Hits_2000_2019)を使用し、年別の平均テンポと時間を計算し、時系列（2000〜2019年）でのキーとジャンルの分布を可視化します。

- [**spotify.Rmd**](https://github.com/hina0830g/Spotify-Top-Charts-Analysis/blob/main/spotify.pdf) <br>
五数要約、箱ひげ図、時間とテンポの線形回帰を表示します。

<h2 align="center"> 結果 / 結論 </h2>

<h3> 結果要約 </h3> 

20年間で、以下のことが分かりました <br>

一般的な時間 : **3分35秒** <br>
一般的なテンポ : **97.92 & 125.20 BPM** (二峰分布 :two:) <br>
一般的なキー: **C#, B, C** <br>
一般的なジャンル: **ポップ、ヒップホップ、ロック** <br>

平均して、2000-2019年の人気曲では平均テンポは*増加*し📈（弱い正の相関）、平均時間は*減少*しました📉（強い正の相関）。短い曲への傾向の増加は、人々の注意力の持続時間の減少に起因する可能性があると推測されます。
<h3> 予測モデル </h3>

**T(t) = 0.313y - 508**、ここでt = 年、T = BPMでのテンポ  <br>
**D(t) = -0.035y + 74.56**、ここでt = 年、D = 分での時間

<h3>  2023年の予測 </h3>

このモデルは、2023年のSpotifyトップ100トラックの平均テンポと時間を**125 BPM**と**3分20秒**と予測しています！ 🥳

