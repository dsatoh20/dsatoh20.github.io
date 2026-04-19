# Association Between BCR-ABL Tyrosine Kinase Inhibitors for Chronic Myeloid Leukemia and Cardiovascular Events, Major Molecular Response, and Overall Survival: A Systematic Review and Meta-analysis
DOI: 10.1001/jamaoncol.2015.5932
>**臨床医のための疫学・統計 輪読会メモ**

## RQ
Tyrosine kinase inhibitor(TKI)と血栓症には関連があるか。
## 手法
2014年10月21日時点で出版されている研究論文、過去３年間の国際学会抄録、及びClinicalTrials.govに登録されている研究を対象としたメタアナリシス。
### P
主にclinicaltrials.govから抽出した10の研究に参加した患者3043名
### E
imatinibの後発TKIの投与
### C
imatinibの投与
### O
imatinibに比べて、心血管イベントリスクが高い
## 知見
- dasatinib,nilotinib,ponatinibはimatinibに比べて心血管イベントのリスクが高い
## 考察
- [アイクルシグの添付文書](https://www.kegg.jp/medicus-bin/japic_med?japic_code=00066524)を確認したところ、有害事象の発生頻度として、血球減少が約半数で生じるのに対して、心血管系イベントは3%前後だった。このような頻度の少ない有害事象が本当に薬剤によるものか検証すべく、メタアナリシスが採用されている。メタアナリシスでは、複数の報告を統合することでサンプルサイズを大きくし、検出感度を上げることを期待できる。
- 一方で、サンプルサイズをただ大きくすることには危険もある。ロスマンの疫学では"It is better to be vaguly right than precisely wrong.
"という格言が引用されていたように、バイアスの制御が不十分であれば、p-value functionのグラフは真でないpoint-estimateを中心にスリムになっていく可能性がある。
- ロスマンの疫学では、バイアスは、selection bias, information bias, confoundingの3つに区別している。メタアナリシスで注目すべきは、selection biasであろう。ロスマンの疫学で定義されるところでは、selection biasとは、被験者の選択方法と研究参加に影響する要因によって生じるエラーである。メタアナリシスを解釈する際には、被験者を報告と読み替える。
- selection biasを制御する方法として、本研究では、1. 複数の研究者でチェック、2. random effect modelとの比較(=感度分析)を用いている。
- 1は、報告の選別に際して事前に設定したプロトコルに準じて3名でチェックしたとあるが、論文の著者3名の間に非科学的な結託がないことは如何にして示すのだろうか。
- 2は、random effect modelによって、抽出する報告ごとの特性を踏まえた解析を実現している。fixed effect modelで有意な結果が出たのに対して、random effect modelで有意な結果が出なかったとしたら、どう解釈すべきか。まずは、本来はリスク比=1なのに、あたかもリスク比>1に見せかけるようなselection biasが残存している可能性を考える。おそらくは、サンプルサイズの大きい報告について、リスク比>1という結果が出たものを優先的に抽出したことが疑わしい。
- メタアナリシスを正しく解釈する上で、selection biasのほかに、publication biasについても議論したい。publication biasは、研究者が望む結果が得られた研究のみが報告されることに起因するエラーである。本研究では、funnel plotによってpublication biasが小さいことを示した。
- 本研究では、抽出する報告を吟味する中で、ClinicalTrials.govに掲載されていることが重視されているが、これもpublication biasを小さくすることに寄与していると考えられる。なぜなら、ClinicalTrials.govは試験を開始する前に登録するというルールがあり、出版時点で恣意性がはたらきにくいだろうから。ただし、研究者が望むような結果が出なかった場合に、結果の登録が遅れることなどは想定されるため、これだけでpublication biasの制御が十分であるとはいえない。
- メタアナリシスは、エビデンスレベル最高と位置付けられるものの、バイアスの制御は決して簡単でなく、解釈は一筋縄ではいかない。診療においても、Cochraneレビューなどシステマティックレビューを参照することがあるが、果たしてそれがprecisely wrongな報告でないか、慎重に見極める必要はあるだろう。
## 批判的吟味（疫学的視点）by Claude Code

### 1. 採択バイアス（Selection bias）の残存可能性

ユーザーの指摘は正当だが、さらに掘り下げたい点がある。本研究の採択基準は「RCTまたは前向きコホート」に限定されているが、**介入群（後発TKI群）と比較群（imatinib群）の追跡期間の非対称性**が問題になり得る。後発TKIはimatinibより後に承認されたため、長期フォローアップデータが少なく、心血管イベントが後期に生じる薬剤であれば過小評価される。採択された10試験の追跡期間分布を確認し、感度分析（追跡≧2年のみ）が行われているかを確かめることが重要。

### 2. 異質性（Heterogeneity）の扱い

メタアナリシスで最初に確認すべきは I² 統計量である。本文中にfixed effect modelとrandom effect modelの比較が登場するが、**I²が高い（>50%）状況でfixed effectモデルを採用することは統計的に不適切**である。ユーザーの考察「fixed effectで有意・random effectで有意でない場合はselection biasの残存」は一つの解釈だが、より基本的な解釈は「試験間で真の効果量が異なる（heterogeneityが大きい）ため、単一のプール推定値は意味をなさない」である。その場合はサブグループ解析（薬剤別・心血管イベント種別）で効果修飾因子を探る方向が正道。

### 3. 複合アウトカムとしての「心血管イベント」の問題

「心血管イベント」は動脈血栓（心筋梗塞・脳梗塞・末梢動脈疾患）と静脈血栓（DVT・PE）、さらには不整脈（QT延長・胸水）を混在させた複合アウトカムである可能性がある。各TKIの作用機序は異なり（dasatinibは胸水・肺動脈高血圧、nilotinibは動脈硬化促進、ponatinibは汎血管障害）、これらを一括集計すると**効果の方向性が打ち消し合う・または誇張される**。PICO上のOを細分化した感度分析が提示されているかを確認すること。

### 4. 交絡：適応による交絡（Confounding by indication）

imatinibはCML第一選択として長く使用されており、後発TKIはimatinib抵抗性・不耐容例（≒高リスク群）に使われることが多い。すなわち**後発TKI群はベースラインの心血管リスクが高い可能性**があり、薬剤効果と患者背景の混在が生じる。RCTのみを採択していれば無作為化によりこの問題は緩和されるが、前向きコホートが混在している場合は交絡の除去が不完全になる。ここがSokal/ELTS scoreなどのベースライン調整の有無を確認すべきポイント。

### 5. Publication biasの検出力の限界

funnel plotの非対称性がpublication biasを示唆するという解釈は一般的だが、**10試験という少数ではfunnel plotの検出力は著しく低い**（Cochrane HandbookはN≧10を推奨）。Egger's testやBegg's testも同様に検出力不足となる。ユーザーの「ClinicalTrials.gov登録による制御」の指摘は正しいが、登録された試験の"outcome switching"（事前登録アウトカムを後から変更）については本研究では評価されていない可能性が高い。

### 総評

ユーザーの考察はバイアスの概念的整理として水準が高い。次のステップとして、**各バイアスを「どの方向に」「どの程度」効果推定値を歪めるか**まで議論できると疫学的思考がより実践的になる。本論文においては、適応による交絡と追跡期間の非対称性がいずれも「後発TKIの心血管リスクを過大評価する方向」に働く可能性があり、結論の堅牢性は慎重に評価すべきである。
## 輪読会(20260419)後の気づき
- [発表資料](https://docs.google.com/presentation/d/1fijBhR31RdWufvGkcisWfeREsyfVTevsPD-o8hu5w14/edit?usp=sharing)