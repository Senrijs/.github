<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./senri-ippo-wordmark-dark.svg">
    <img src="./senri-ippo-wordmark-light.svg" alt="Senri / Ippo" height="64">
  </picture>
</p>

<p align="center">
  <b>千里の道も一歩から。</b><br>
  <i>A journey of a thousand miles begins with a single step.</i>
</p>

<p align="center">
  Web frameworks where the first step is easy — and that go all the way.
</p>

<p align="center">
  <b>English</b> · <a href="./README.ja.md">日本語</a>
</p>

---

## Projects

| | | Status |
| --- | --- | --- |
| **[Senri](https://github.com/Senrijs/Senri)** | A TypeScript web framework for **Bun, Deno and Node.js**, built on Web standards. | 🚧 In development |
| **Ippo** | A React (and later Vue) meta-framework built on Senri. | 📝 Planned |

## Why Senri?

- **One step to start** — `serve(app)` runs the same app on Bun, Deno and Node.js.
- **Errors that teach** — in dev mode, errors show the failing line, a hint, and "did you mean…?" for 404s.
- **See inside** — the `/_senri` dashboard shows every request and how it passed through your middleware.
- **Zero dependencies** — the core uses only `Request` and `Response`.

```ts
import { createApp } from "senri";
import { serve } from "senri/serve";

const app = createApp({ dev: true });

app.get("/users/:id", ({ id }) => ({ id }));

serve(app); // → http://localhost:3927
```

> Why 3927? Because 1 *ri* ≈ 3.927 km — so a thousand *ri* (千里) is about 3927 km.

---

<p align="center">
  <sub>A project from the <a href="https://github.com/skyia-jp">@skyia-jp</a> community · Made in Japan 🇯🇵</sub>
</p>
