<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./senri-ippo-wordmark-dark.svg">
    <img src="./senri-ippo-wordmark-light.svg" alt="Senri / Ippo" height="64">
  </picture>
</p>

<p align="center">
  <b>千里の道も一歩から。</b>
</p>

<p align="center">
  最初の一歩が簡単で、どこまでも届く Web フレームワーク。
</p>

<p align="center">
  <a href="./README.md">English</a> · <b>日本語</b>
</p>

---

## プロジェクト

| | | 状況 |
| --- | --- | --- |
| **[Senri](https://github.com/Senrijs/Senri)** | **Bun・Deno・Node.js・Cloudflare Workers・ブラウザ** で動く、Web 標準ベースの TypeScript 製 Web フレームワーク | 🚧 開発中 |
| **Ippo** | Senri の上に乗る、React(のちに Vue)対応のメタフレームワーク | 📝 予定 |

## Senri の特徴

- **一歩目が簡単** — `serve(app)` だけで、同じアプリが Bun・Deno・Node.js で動きます
- **教えてくれるエラー** — 開発モードでは、エラーが起きた行・直し方のヒント・404 の「もしかして」を表示します
- **中が見える** — `/_senri` ダッシュボードで、すべてのリクエストと、それがミドルウェアをどう通ったかが見られます
- **依存ゼロ** — 本体は `Request` と `Response` だけで書かれています

```ts
import { createApp } from "@senrijs/senri";
import { devtools } from "@senrijs/senri/dev";
import { serve } from "@senrijs/senri/serve";

const app = createApp({ dev: devtools() });

app.get("/users/:id", ({ id }) => ({ id }));

serve(app); // → http://localhost:3927
```

> なぜ 3927 番? 1里 ≒ 3.927km なので、千里でおよそ 3927km だからです。

---

<p align="center">
  <sub><a href="https://github.com/skyia-jp">@skyia-jp</a> コミュニティから生まれたプロジェクト · Made in Japan 🇯🇵</sub>
</p>
