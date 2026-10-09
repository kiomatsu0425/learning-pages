# 資本主義学習サイト：マルチモーダル学習設計

## 目的
Google Drive正本「学習計画｜資本主義を体系的に理解する」の6つの問いを自分の言葉で説明できるようにする。
単純な教材リンク集・逐語暗記・受動的な音声視聴を学習成果とみなさない。

## 根拠に基づく設計原則
1. 表現は内容に合わせる。歴史の順序はタイムライン、因果は図、論争は比較、詳細な論拠は文章。
2. 短い図＋短いナレーションを必要時に提供する。音声は自動再生しない。画面に対応する文章を残す。長い読み上げを強制しない。
3. 見る・聞くだけで完了とせず、前提を予測し、比較し、閉じて説明する。
4. 別の説明・反例・不確実性の検討を毎回含める。
5. 翌日・3日後・7日後の想起日を運用上の初期値とする。最適日数の断定ではなく、再提示の出発点。
6. 学習スタイル診断（視覚型・聴覚型）を使わない。複数感覚の刺激を増やすこと自体は目的にしない。
7. 音声やブラウザ操作が使えなくても同じ論点にアクセスできるテキストの代替を提供する。
8. Google Drive学習計画を内容の正本とし、HTMLは学習体験層として運用する。

## Q02試作ページ（capitalism/q02-lab.html）
- Step 1：事前予想。インプット前の仮説を入力
- Step 2：タップできる歴史タイムライン＋任意の音声ガイド
- Step 3：4つの因果説明（技術、相対価格、制度、貿易）の比較。各説明の限界を明示
- Step 4：資料を閉じて90秒〜3分の説明。外部のChatGPT音声会話またはローカル録音。Before→After記録
- Step 5：時間を空けた再説明。再訪時の復習目安表示
- 教材：OpenStax・CORE Econは根拠を確認する資料として任意アクセス
- 技術：純粋なHTML/CSS/JavaScript。GitHub Pages互換。speechSynthesisはブラウザ依存、MediaRecorder音声はページ内一時再生、メモはlocalStorageのみ。JSON書き出しあり
- 非対応：自動音声評価、ブラウザ間同期、バックグラウンド通知、シミュレーションを歴史的因果の証明とする機能

## 検証の観点（利用後）
- リンクから説明まで迷わず到達できるか
- 文章を読むだけの方式と比較し、別の要因・反証も含めて説明できるか
- 翌日・数日後に要点を再生できるか
- 視覚・音声・操作が注意を散らさず理解を助けているか
- Q02で有効と確認できた機能のみQ03〜Q06へ展開する

## 研究参照
- Mayer (2024), The Past, Present, and Future of the Cognitive Theory of Multimedia Learning: https://doi.org/10.1007/s10648-023-09842-1
- Cromley & Chen (2025), A meta-analysis of Richard Mayer's multimedia learning research: https://doi.org/10.1016/j.edurev.2025.100730
- Dunlosky et al. (2013), Improving Students' Learning With Effective Learning Techniques: https://doi.org/10.1177/1529100612453266
- Pashler et al. (2008), Learning Styles: Concepts and Evidence: https://doi.org/10.1111/j.1539-6053.2009.01038.x
