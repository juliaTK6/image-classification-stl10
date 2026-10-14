# image-classification-stl10
# STL-10 Image Classification with PyTorch

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_GITHUB_USERNAME/YOUR_REPOSITORY_NAME/blob/main/stl10_classification.ipynb)

PyTorchとGoogle Colabを使用して、STL-10データセットに対する画像分類モデル（畳み込みニューラルネットワーク / CNN）を構築・訓練するプロジェクトです。

---

## 概要

STL-10データセットは、10種類のクラス（airplane, bird, car, cat, deer, dog, frog, horse, ship, truck）で構成される画像認識のためのベンチマークデータセットです。本プロジェクトでは、データの読み込み・前処理からモデルの構築、学習、評価までの一連の流れを実装しています。

### 主な機能・特徴
- **Google Drive連携**: Google Colab環境でGoogle Driveをマウントし、データセットやモデルの重みを永続化
- **データ前処理 & Data Augmentation**: `torchvision.transforms` を用いた正規化・画像変換
- **CNNモデル構築**: PyTorchを使用した画像分類用ニューラルネットワークの実装
- **評価 & 可視化**: テストデータに対する精度計算および分類結果の可視化

---

## データセットについて

* **名称**: STL-10 Dataset
* **解像度**: 96 × 96 ピクセル（3チャンネル RGB）
* **クラス数**: 10クラス
* **取得方法**: `torchvision.datasets.STL10` を使用して自動ダウンロード

---

## 開発・実行環境

* Python 3.x
* PyTorch (`torch`, `torchvision`)
* NumPy
* Matplotlib
* Google Colab (GPUランタイム推奨)

---

## 使い方

1. バッジの「Open in Colab」をクリックして、Google Colabでノートブックを開きます。
2. ノートブック内のセルを上から順に実行します。
   - 最初のセルでGoogle Driveへのアクセス許可が求められた場合は承認してください。
   - GPUを利用する場合は、Colabのメニューから `ランタイム > ランタイムのタイプを変更 > T4 GPU` を選択してください。

---

## ライセンス

本リポジトリのコードは [MIT License](LICENSE) のもとで公開されています。
