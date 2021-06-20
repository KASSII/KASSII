[![](https://raw.githubusercontent.com/KASSII/KASSII/main/profile-summary-card-output/default/1-repos-per-language.svg)](https://github.com/vn7n24fzkq/github-profile-summary-cards) [![](https://raw.githubusercontent.com/KASSII/KASSII/main/profile-summary-card-output/default/2-most-commit-language.svg)](https://github.com/vn7n24fzkq/github-profile-summary-cards)  

# Repositories  
## pytorch_templates  
**About**  
基本的なDeepLearningタスクの実装をまとめたリポジトリ。  
データとラベルを準備してコマンドを実行するだけで簡単に学習・推論ができるようになっている。  
実験などの際にデータさえ作ればすぐに学習・評価できるようになることを目的として作成。  

タスクごとに実行方法やデータフォーマットをREADMEに記載し、examplesに実際のデータセットや実行例を置くことで使い方が分かりやすくなるように工夫している。  
また、学習ループの処理や重みの保存、ログ出力処理などを共通処理クラスとして実装することで、シンプルでわかりやすいコードになるように工夫している。  
タスク共通で同じスクリプト構成にできるため、ソースコード管理をしやすくなっている。  

**URL**  
https://github.com/KASSII/pytorch_templates  

**Skills**  
  * Python  
    * PyTorch  


## libtorch_templates  
**About**  
C++によるDeepLearningの推論コードをまとめたリポジトリ。  
pytorchの学習結果をlibtorch用に変換するスクリプトも合わせて実装している。  
Pythonで学習したAI機能を簡単にC++でデプロイできるようにすることを目的として作成。  

any型を使用して前処理クラス（Transform、PreProcess）を実装することで、PyTorchと同じように前処理を定義できるように工夫している。  
また、それぞれのタスクごとにCMakeを作成してビルドを簡易的にできるようにしている。  

**URL**  
https://github.com/KASSII/libtorch_templates  

**Skills**  
  * C++
  * libtorch
  * CMake

## reinforcement-learning  
**About**  
強化学習の各種アルゴリズムの説明、および対応するスクリプトをまとめたリポジトリ。  
強化学習アルゴリズムの理解および実装方法の習得のために作成。  
実装する中で気づいた点なども実装メモとしてREADMEに記載している。  

**URL**  
https://github.com/KASSII/reinforcement-learning  

**Skills**
  * Python
  * 強化学習  

## ai-webapp  
**About**  
画像をAIで解析し、結果を表示するwebアプリのソースコードをまとめたリポジトリ。  
特別な環境設定や知識が無くても誰でもAI機能を使えるようにすることを目的に開発したアプリ。  

フロントエンドはシンプルで直感的に使い方が分かるようなデザインにしている。  
また、Ajaxを用いることでページ読み込みすることなく結果の表示ができるように工夫している。  
バックエンドは各AI機能を独立したAPIとして実装することで、機能追加・削除を簡単にできるシステム構成になるように工夫している。  
AIタスクごとに定義した仕様に従ってAPI実装し、DBに情報追加するだけで簡単に機能を追加することができるようにしている。  

**URL**  
（リポジトリ）  https://github.com/KASSII/ai-webapp  
（デモサイト） http://kassii.xyz/ai_demo/project/

**Skills**
  * HTML
  * CSS  
  * JavaScript
  * Django  
  * FastAPI
  * PyTorch
  * サーバー構築
    * nginx
    * Gunicorn
    * Uvicorn


# Published Apps
## Fothello  
**About**  
AIと対戦できる変則オセロアプリ。  

ゲームルールの検討からGUI実装、AI機能実装まで行なっている。  
GUIでは、動作が分かりやすいアニメーションにしたり、次に置ける手の場所に色付きエフェクト表示させるなど使用者が視覚的に分かりやすくなるように工夫をしている。  
AI部分は通常のオセロと同じ盤面評価をすると弱いAI（得点倍の色を最初に使い果たして最後に逆転負けすることが多い）になってしまうため、4色オセロ用の評価基準をチューニングして実装するなどの工夫をしている。  

**URL**  
https://play.google.com/store/apps/details?id=com.KASSII.Fothello

**Skills**  
  * Unity
  * ゲームAI
    * αβ法
 
## 言葉電卓  
**About**  
自然言語処理AIを用いた「単語の意味」を演算するアプリ。  
学習済みword2vecモデルで単語をベクトル化することで意味の計算を行なっている。  
モバイルアプリで実装するにあたり、学習結果をそのまま使用するとメモリサイズが大きすぎて動作が重くなるため、livedoorニュースコーパスを解析して頻出単語のみを抽出することでメモリサイズを抑える工夫をしている。  

**URL**  
https://play.google.com/store/apps/details?id=com.kassii.vocabulary_calculator

**Skills**  
  * 自然言語処理  
    * word2vec
  * Flutter
