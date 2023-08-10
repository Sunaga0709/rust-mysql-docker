# 環境構築
### `.env`を`.env.example`からコピー
パスワードやDB名を独自で設定する場合は適宜envの値を変更する

```
cp .env.example .env
```

### Dockerビルド
```
make build
```

### Docker起動
```
make up
```

### Docker停止
```
make down
```

### Docker動作状況確認
```
make ps
```

### Rust実行
```
make cargo-run
```

### リンタ
```
make cargo-lint
```

### フォーマット
```
make cargo-fmt
```

### クレート追加
クレートを追加したらDockerビルドを再度行う<br>
バージョン指定やフィーチャーを指定する場合は`Cargo.toml`に記述しビルドを行う
```
make cargo-add-crate crate={ クレート名 }
```
