# API POINTS



## Users


### Menampilkan data users
```
GET: /users

response:
[
{
    "id": "1",
    "name": "Thoriq Azis Hakim El Karim",
    "motto": "\"Make your day as a way, you must planning wherever you want\"",
    "desc": "Hi Everyone! Sebagai mahasiswa sistem informasi universitas Ahmad Dahlan angkatan 2020 saya masih sangat awam dalam hal percodingan. masih mengalami fase trial and error yang sangat sering, sehingga harus belajar terus menerus. Jalan yang saya tempuh masih panjang, seperti kutipan saya diatas \"Make your day as a way, you must planning wherever you want\"",
    "ig_url": "https://www.instagram.com/trick_thoriq04/",
    "github_url": "",
    "avatar_url": ""
},
{
  ...
}
]
```
### Menampilkan data user dengan ```id``` tertentu 
```
GET: /users/[id]

response:
{
    "id": "1",
    "name": "Thoriq Azis Hakim El Karim",
    "motto": "\"Make your day as a way, you must planning wherever you want\"",
    "desc": "Hi Everyone! Sebagai mahasiswa sistem informasi universitas Ahmad Dahlan angkatan 2020 saya masih sangat awam dalam hal percodingan. masih mengalami fase trial and error yang sangat sering, sehingga harus belajar terus menerus. Jalan yang saya tempuh masih panjang, seperti kutipan saya diatas \"Make your day as a way, you must planning wherever you want\"",
    "ig_url": "https://www.instagram.com/trick_thoriq04/",
    "github_url": "",
    "avatar_url": ""
}
```
### Menambahkan data user
```
POST: /users

data:
{
    "name": "Thoriqqq",
    "motto": "Ini Motto",
    "desc": "",
    "ig_url": "",
    "github_url": "",
    "avatar_url": ""
}

response:
true    //if true
false   //if false
```
### Mengubah data user
```
PUT: /about

data:
{

    "id":"4",
    "name": "Thoriq",
    "motto": "",
    "desc": "",
    "ig_url": "",
    "github_url": "",
    "avatar_url": ""
}
response:
true    //if true
false   //if false
```
### Menghapus data user
```
DELETE: /users/[id]

response:
true    //if true
false   //if false
```
## ARTICLES
### Menampilkan articles
```
GET: /articles

response:
[
{
    "id": "1",
    "title": "Jack all the trades is a master of none",
    "description": "\"Hidup akan lebih mudah jika menguasai semunya\"",
    "author": "Thoriq Azis Hakim El Karim",
    "thumbnail_url": "https://i.pinimg.com/564x/fd/22/27/fd22270b02ab43eaffc61b72e3dd4010.jpg",
    "content": "article_1.md"
},
{
    ...
}
]
```
### Menampilkan article berdasarkan ```id```
```
GET: /articles/[id]

response:
{
    "id": "1",
    "title": "Jack all the trades is a master of none",
    "description": "\"Hidup akan lebih mudah jika menguasai semunya\"",
    "author": "Thoriq Azis Hakim El Karim",
    "thumbnail_url": "https://i.pinimg.com/564x/fd/22/27/fd22270b02ab43eaffc61b72e3dd4010.jpg",
    "content": "article_1.md"
}
```
### Menambahkan article
```
POST: /articles

data:
{
    "title": "Articles",
    "description": "Artikel kosong",
    "author": "Thoriq Aziz",
    "thumbnail_url": "https://i.pinimg.com/originals/93/95/84/9395847a93b4f8b1af37905351af2cb8.jpg",
    "content": "article_2.md"
}

response:
true    //if true
false   //if false
```
### Mengubah article
```
PUT: /articles

data:
{

  "id": "4"
  "title": "Articles",
  "description": "Blank article",
  "author": "Thoriq Aziz",
  "thumbnail_url": "hhttps://i.pinimg.com/originals/93/95/84/9395847a93b4f8b1af37905351af2cb8.jpg",
  "content": "article_2.md"
  
}

response:
true    //if true
false   //if false
```
### Menghapus article
```
DELETE: /articles

response:
true    //if true
false   //if false
```

# DATABASE DESIGN
![Design Database](https://raw.githubusercontent.com/wenispr2703/tekweb2022/main/images/Desain%20DB.png)
