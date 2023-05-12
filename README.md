# Shapes Contract

[Shapes NFT](https://github.com/takeiyuto/shapes) のスマート コントラクトです。

## 動作方法

1. 適切なディレクトリでこのレポジトリをクローンし、ライブラリをダウンロードします。
```bash
git clone https://github.com/takeiyuto/shapes-contract.git blockchain
cd blockchain
yarn
```

2. コンパイルします。
```bash
yarn truffle compile
```

3. 新しいターミナルを開いて、同じディレクトリから、ローカル環境でテスト用ブロックチェーン Ganache を起動します。このとき、以下の `<MNEMONIC>` の箇所を、テストに用いるウォレット アカウントのニーモニックで置き換えて実行します。
```bash
yarn ganache -m "<MNEMONIC>"
```

4. 手順 2. のターミナルに戻って、デプロイします。出力中には、*Contract created* などとして、デプロイされたスマート コントラクトのアドレスが表示されます。
```bash
yarn truffle migrate
```

5. Shapes NFT の[バックエンド](https://github.com/takeiyuto/shapes-backend)と[フロントエンド](https://github.com/takeiyuto/shapes-frontend)を準備します。詳細は、[Shapes Backend の README.md](https://github.com/takeiyuto/shapes-backend/blob/main/README.md) を参照してください。

## ライセンス表示

このサンプル コードは、[MIT License](LICENSE)で提供しています。

# 参照

[徹底解説 NFTの理論と実践](https://www.ohmsha.co.jp/book/9784274230608/)の第9章2節を参照してください。[本書の Web サイト](https://takeiyuto.github.io/nft-book)も参考にしてください。
