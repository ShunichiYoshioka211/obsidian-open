# obsidian-open

Obsidian のノートを https のリンクから開くための中継ページ。
`obsidian://` を直接リンクにできない場所（VS Code の Claude Code 拡張のチャット欄など）で使う。

```text
https://shunichiyoshioka211.github.io/obsidian-open/#50-reference/foo
```

- `#` の後ろは vault からの相対パス（`.md` は省略可）。`#` 以降はサーバーに送られない
- PC では `obsidian://open?vault=context&file=…` へ、スマホでは GitHub の該当ファイルへ飛ぶ
- 自動で飛ばなかったときのためにボタンを2つ置いている
