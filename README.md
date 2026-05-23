# luckSort Web Demo

Unity WebGL build deployed to GitHub Pages.

## Live Demo

After Pages is configured: https://yufei9527.github.io/luckSort_web/

## Build Info

- Engine: Unity (WebGL build)
- Compression: Brotli (`.unityweb` files)
- Decompression Fallback: enabled (works on any static host without server-side `Content-Encoding`)

## File Structure

```
.
├── index.html
├── .nojekyll          # tells GitHub Pages to serve _-prefixed files / underscore folders as-is
├── Build/
│   ├── build_web.data.unityweb       # ~16 MB
│   ├── build_web.framework.js.unityweb
│   ├── build_web.loader.js
│   └── build_web.wasm.unityweb        # ~8 MB
└── TemplateData/      # Unity default loading template (logo, css, etc.)
```

Total build size: ~24 MB. Well under GitHub Pages 100MB single-file limit.
