# obsidian-open

Obsidian のノートを https のリンクから開くための中継ページ。
`obsidian://` を直接リンクにできない場所（VS Code の Claude Code 拡張のチャット欄など）で使う。

```text
https://shunichiyoshioka211.github.io/obsidian-open/#50-reference/foo
```

- `#` の後ろは vault からの相対パス（`.md` は省略可）。`#` 以降はサーバーに送られない
- PC では `obsidian://open?vault=context&file=…` へ飛ぶ
- スマホでは `obsidian://pull-open?vault=context&file=…` へ飛ぶ。
  vault 側のプラグイン（pull-then-open）が受け、Git プラグインで pull してからノートを開く
- Obsidian が前に出てページが隠れたら、タブを閉じる。PC ではページのチェックを入れたブラウザに限り、
  フォーカスが外れた時点でも閉じる
- 自動で飛ばなかったときのためにボタンを3つ置いている
