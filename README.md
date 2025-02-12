
# 21cineplex-api

Scraping data dari 21cineplex untuk keperluan hobby dan riset, tidak ada hal yang berbahaya atau dapat merugikan website sumber.

## Software
```
- NodeJS v14.19.0 atau lebih dengan versi stabil.
- npm v8.1.3 atau lebih
```

## Paket software
```
- cheerio^1.0.0-rc.10
- axios^0.26.1
- express^4.17.3
- nodemon^2.0.15
```

## Installasi

```
- git clone https://github.com/heirro/21cineplex-api.git
- cd 21cineplex-api
- npm install
```

## Menjalankan projek

### Di local
```
npm run dev
```

### Di server
```
npm run start
```
## Referensi API

#### Dapatkan item film yang sedang berlangsung

```
http://localhost:3180/cineplex/playing
```

| Method | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `GET` | `JSON` | Menampilkan semua Film yang sedang berlangsung di theater. |

#### Dapatkan item film yang akan datang

```
http://localhost:3180/cineplex/upcoming
```

| Method | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `GET` | `JSON` | Menampilkan semua Film yang akan datang di theater. |

#### Dapatkan item semua Kota

```
http://localhost:3180/cineplex/city
```

| Method | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `GET` | `JSON` | Menampilkan semua Kota |

#### Dapatkan item Teater berdasarkan Kota

```
- http://localhost:3180/cineplex/city/{id}
Ex: http://localhost:3180/cineplex/city/12
```

| Method | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `GET` | `JSON` | Menampilkan semua item Teater (2D Reguler, IMAX, Premier) berdasarkan Kota, untuk mendapatkan id kota, menggunakan endpoint /cineplex/city |

#### Dapatkan item semua jadwal film di Teater berdasarkan Kota

```
- http://localhost:3180/cineplex/schedule/{id}
Ex: http://localhost:3180/cineplex/schedule/SBYCIWO
```

| Method | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `GET` | `JSON` | Menampilkan semua jadwal Film di Teater berdasarkan Kota, untuk mendapatkan id Teater, menggunakan endpoint /cineplex/city/{id} |


## Demo

- Now Playing: https://api.jadalak.com/cineplex/playing

- City: https://api.jadalak.com/cineplex/city

- Up Coming: https://api.jadalak.com/cineplex/upcoming

- Teater: https://api.jadalak.com/cineplex/city/12

- Schedule: https://api.jadalak.com/cineplex/schedule/SBYCIWO
