# SIM-Data-Jemaat
SIM Data Jemaat adalah aplikasi open source yang dapat digunakan untuk Mengelola Data Jemaat pada suatu Gereja.

**Table of content:**
- [Fitur Utama](#Fitur-Utama)
- [Persyaratan](#Persyaratan)
- [Memulai Proyek](#Memulai-Proyek)
- [Images](#images)
  - [`.images` directory](#images-directory)
  - [`pre-commit` hook](#pre-commit-hook)
- [markdownlint](#markdownlint)
- [License](#License)

## ⭐ Fitur Utama
- Menambah, mengedit dan menghapus Data Jemaat
- Nenambah, mengedit dan menghapus Data Distrik dan Kelurahan
- Mencari data berdasarkan kata kunci
- Melihat laporan presentase jumlah anggota Jemaat

## 🛠️ Persyaratan

- OS: Windows 10/11, Linux with Wine
- IDE : Microsoft visual studio 2022 Community Edition
- Bahasa Pemrograman : C#
- Database Sistem : SQLite

## ✈️ Memulai Proyek

Unduh repositori ini ke komputer anda :

```shell
git clone https://github.com/tifapratama/SIM-Data-Jemaat.git
```

## Images

### `.images` directory

Keep all images in `.images` directory of the project root. This allows moving markdown documents across any subdirectories without the need to update links to images.

Regardless of where the markdown page is placed within the repository, all image links are related to the project root as below:

```markdown
![img](/.images/sample-image.png)
```

![img](/.images/sample-image.png)

### 🛡️ License

`pre-commit` hook automatically detects the image files that are not referenced anywhere within the repository anymore and removes them.

Proyek ini dilisensikan dibawah lisensi MIT. Silakan baca [LICENSE](./LICENSE) untuk detailnya.

```shell
chmod 755 .images/untrack-unused-images.sh; \
ln --symbolic ../../.images/untrack-unused-images.sh .git/hooks/pre-commit
```


