# User

# Menampilkan data user


GET: /user

response:
[
    {
        "id"            : "",
        "nama"          : "",
        "nim"           : "",
        "title"         : "",
        "url_ig"        : "",
        "url_git"       : "",
        "url_line"      : "",
        "img_profile"   : ""
    },
    ...
]


# Menampilkan data user dengan "id" tertentu


GET: /user/[id]

reponse:
{
        "id"            : "",
        "nama"          : "",
        "nim"           : "",
        "title"         : "",
        "url_ig"        : "",
        "url_git"       : "",
        "url_line"      : "",
        "img_profile"   : ""
}


# Menambahkan data pengguna


POST: /user

data:
{
        "nama"          : "",
        "nim"           : "",
        "title"         : "",
}

response:
true    // if success
false   // if failure


# Edit data pengguna


PUT: /user

data:
{
        "id"            : "",
        "nama"          : "",
        "nim"           : "",
        "title"         : "",
}

response:
true    // if success
false   // if failure



# Menghapus data anggota


DELETE: /user/[id]

response:
true    // if success
false   // if failure


# Artikel

# Menampilkan data semua artikel


GET: /article

response:
[
    {
        "id"            : "",
        "judul"         : "",
        "slug"          : "",
        "penulis"       : "",
        "title"         : "",
        "deskripsi      : "",
        "sampul"        : ""
    }

]


# Menampilkan data artikel dengan id 


GET: /article/[id]

response:
{
        "id"            : "",
        "judul"         : "",
        "slug"          : "",
        "penulis"       : "",
        "title"         : "",
        "deskripsi      : "",
        "sampul"        : "",
}


# Menambahkan data artikel


POST: /artikel

data:
{       
        "judul"         : "",
        "slug"          : "",
        "penulis"       : "",
        "title"         : "",
        "deskripsi      : "",
        "sampul"        : "",
}

response:
true    // if success
false   // if failure


## Mengedit data artikel


PUT: /article

data:
{      
        "id"            : "",
        "judul"         : "",
        "slug"          : "",
        "penulis"       : "",
        "title"         : "",
        "deskripsi      : "",
        "sampul"        : "",
}

response:
true    // if success
false   // if failure


# Menghapus data artikel


DELETE: /article/[id]

response:
true    // if success
false   // if failure


Database 

User {
        +"id"            : int
        +"nama"          : string
        +"nim"           : string
        +"title"         : string
        +"url_ig"        : string
        +"url_git"       : string
        +"url_line"      : string
        + img_profile    : string
        + getAllUser()
        + getUserById()
        + updateUser()
        + createUser()
        + deleteUser()
    },

 About{
        +"id": int
        +"foto": string
        + getAllUser()
        + getUserById()
        + updateUser()
        + createUser()
        + deleteUser()
    }

Article{
    +"judul":string
    +"title":string
    +"deskripsi":string
    +"sampul":string
     + getAllUser()
    + getUserById()
    + updateUser()
    + createUser()
    + deleteUser()

}
