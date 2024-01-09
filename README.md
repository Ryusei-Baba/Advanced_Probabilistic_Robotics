### 2023年度 確率ロボティクス課題
Jupyter Notebookを用いて，ロボットのための推定や行動決定アルゴリズムについてのシミュレーションを行う．

課題内容：価値反復法のアルゴリズムであるQ学習により，迷路を探索する．[プログラム](https://github.com/Ryusei-Baba/Advanced_Probabilistic_Robotics/blob/main/src/maze.ipynb)

---
#### アニメーション
![図1 Q学習による状態価値の変化](/animation/state_V.gif)
![図2 Q学習によるロボットの移動](/animation/move_robot.gif)

---
#### 参考書籍
「つくりながら学ぶ！深層強化学習」，著者：株式会社電通国際情報サービス 小川雄太郎，出版社：マイナビ出版</br>

#### サポートリポジトリ
https://github.com/YutaroOgawa/Deep-Reinforcement-Learning-Book/tree/master

#### 変更点
- 状態（迷路）の拡張
    - 変更前：3×3の9つの状態
    - 変更後：5×5の25つの状態 
- 報酬の変更
    - 変更前：ロボットがゴールに到達したら報酬を+1与えるのみ．
    - 変更後：ロボットがゴールに到達したら報酬を+1与える．ロボットが移動するたびに報酬を-0.05与える．（これにより，ロボットが最短経路でゴールに到達できる可能性がある．）
- ロボットが移動するアニメーションの追加
    - 状態価値に対応したロボットの行動を可視化する処理を追加

---
#### 動作環境
- Ubuntu 22.04 LTS
- Python 3.10.12

---
#### 著作権
馬場琉生 + 小川雄太郎

---
#### LICENSE
[MIT License](https://github.com/Ryusei-Baba/Advanced_Probabilistic_Robotics/blob/main/LICENSE)
