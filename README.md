# writing-an-os-in-rust

## A Freestanding Rust Binary

- OS カーネルを書くためには、 OS の機能に依存しないソースコードが必要なる
  - 標準ライブラリがほとんど使えない
- main 関数よりも前に start 関数がよばれる
  - ランタイム（ランタイムシステム）呼び、それが main 関数を呼ぶ
  - プログラム実行: start → ランタイム実行 → main
