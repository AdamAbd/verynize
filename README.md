# Better Design

Repository induk untuk produk dan marketing Better Design.

- `better-design-product/`: submodule aplikasi Electron, editor, CLI/MCP, dan collaboration Worker.
- `better-design-marketing/`: submodule landing page TanStack Start untuk produk.

## Pengembangan produk

Jalankan perintah aplikasi dari folder produk:

```sh
cd better-design-product
npm install
npm start
```

Panduan lengkap ada di `better-design-product/README.md` dan `better-design-product/AGENTS.md`.
Commit perubahan produk di submodule terlebih dahulu, lalu commit pembaruan pointer submodule di repo induk.

## Pengembangan marketing

```sh
cd better-design-marketing
npm install
npm run dev
```

Buka http://localhost:3000. Panduan dan validasi ada di `better-design-marketing/README.md`.

## Submodule lokal

Repo ini belum memiliki remote hosting. URL submodule sementara adalah
`../better-design-product.git` dan `../better-design-marketing.git`, bare repositories lokal di samping repo induk.
Simpan repository tersebut bersama workspace ini; clone repo induk saja tidak mencakup objek Git produk.

Untuk clone lokal dengan submodule:

```sh
git -c protocol.file.allow=always clone --recurse-submodules /path/to/better-design /path/to/checkout
```

Setelah remote produk tersedia, push commit produk ke remote tersebut, ganti URL
pada `.gitmodules`, jalankan `git submodule sync`, dan commit perubahan konfigurasi.
