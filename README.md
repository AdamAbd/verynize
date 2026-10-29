# Verynize

Repository induk untuk produk dan marketing Verynize.

- `verynize-product/`: submodule aplikasi Electron, editor, CLI/MCP, dan collaboration Worker.
- `verynize-marketing/`: submodule landing page TanStack Start untuk produk.

## Pengembangan produk

Jalankan perintah aplikasi dari folder produk:

```sh
cd verynize-product
npm install
npm start
```

Panduan lengkap ada di `verynize-product/README.md` dan `verynize-product/AGENTS.md`.
Commit perubahan produk di submodule terlebih dahulu, lalu commit pembaruan pointer submodule di repo induk.

## Pengembangan marketing

```sh
cd verynize-marketing
npm install
npm run dev
```

Buka http://localhost:3000. Panduan dan validasi ada di `verynize-marketing/README.md`.

## Clone dari GitHub

```sh
git clone --recurse-submodules https://github.com/AdamAbd/verynize.git
```

Submodule produk dan marketing berada di `AdamAbd/verynize-product` dan
`AdamAbd/verynize-marketing`. Commit dan push perubahan submodule terlebih dahulu,
lalu commit pembaruan pointer di repository induk.
