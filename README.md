# API Spec FindIn

## SignUp Student


Request :
- Method : POST
- Endpoint : `/api/signup/student`
- Body :

```json 
{
    "data" : {
         "email" : "string",
         "password" : "string",
         "nama" : "string",
         "no_telp" : "int",
         "universitas" : "string",
         "prodi" : "string",
         "nim" : "int",
         "nik" : "int",
         "tahun_masuk" : "date",
         "expertise" : "string",
         "skills" : "string",
     }
}
```

## SignUp perusahaan


Request :
- Method : POST
- Endpoint : `/api/signup/perusahaan`
- Body :

```json 
{
    "data" : {
         "email" : "string",
         "password" : "string",
         "username" : "string",
     }
}
```

## Get all Student

Request :
- Method : GET
- Endpoint : `/api/student`

Response :

```json 
{
    "data" : {
         "id" : "string, unique",
         "name" : "string",
         "universitas" : "string",
         "expertise" : "string",
         "skills" : "string"
     }
}
```

## Get Detail Student

Request :
- Method : GET
- Endpoint : `/api/student/:id`

Response :

```json 
{
    "data" : {
         "id" : "string, unique",
         "name" : "string",
         "universitas" : "string",
         "prodi" : "string",
         "expertise" : "string",
         "skills" : "string",
         "deskripsi" : "string",
         "video" : "string"
     }
}
```

## Find Student

Request :
- Method : POST
- Endpoint : `/api/student/`
- Body :

```json 
{
    "data" : {
         "skills" : "string, unique",
         "expertise" : "string",
         "kota" : "string"
     }
}
```

Response :

```json 
{
    "data" : {
         "id" : "string, unique",
         "name" : "string",
         "universitas" : "string",
         "expertise" : "string",
         "skills" : "string"
     }
}
```

## Get all Intern

Request :
- Method : GET
- Endpoint : `/api/intern`

Response :

```json 
{

    "data" : {
         "id" : "string, unique",
         "posisi" : "string",
         "perusahaan" : "string",
         "lokasi" : "string",
         "tipe" : "string",
     }
}
```
## Get Detail Intern

Request :
- Method : GET
- Endpoint : `/api/intern/:id`

Response :

```json 
{
    "data" : {
         "id" : "string, unique",
         "posisi" : "string",
         "perusahaan" : "string",
         "lokasi" : "string",
         "deskripsi" : "string",
         "tipe" : "string",
     }
}
```

## Find Intern

Request :
- Method : POST
- Endpoint : `/api/student/`
- Body :

```json 
{
    "data" : {
         "tipe" : "string",
         "skills" : "string",
         "expertise" : "string",
         "lokasi" : "string"
     }
}
```

Response :

```json 
{
    "data" : {
         "id" : "string, unique",
         "posisi" : "string",
         "perusahaan" : "string",
         "lokasi" : "string",
         "tipe" : "string",
     }
}
```

## Post Intern

Request :
- Method : POST
- Endpoint : `/api/postIntern/`
- Body :

```json 
{
    "data" : {
         "posisi" : "string",
         "perusahaan" : "string",
         "lokasi" : "string",
         "tipe" : "string,
         "deskripsi" : "string",
         "tenggat" : "date",
         "panduan" : "string",
     }
}
```

Response :

```json 
{
    "message" : "Berhasil post lowongan"
}
```

## Apply Intern

Request :
- Method : POST
- Endpoint : `/api/applyIntern/`
- Body :

```json 
{
    "data" : {
         "cv" : "string",
         "resume" : "string",
     }
}
```

Response :

```json 
{
    "message" : "Berhasil apply intern"
}
```

## Profile Student

Request :
- Method : GET
- Endpoint : `/api/profileStudent/`

Response :

```json 
{
    "nama" : "string",
    "universitas" : "string",
    "prodi" : "string",
    "tahun_masuk" : "date"
    "expertise" : "string",
    "skills" : "string",
    "deskripsi" : "string",
    
}
```

## Post Video

Request :
- Method : POST
- Endpoint : `/api/postVideo/`
- Body :

```json 
{
    "data" : {
         "video" : "string",
     }
}
```

Response :

```json 
{
    "message" : "Berhasil post video"
}
```

## View Edit Student

Request :
- Method : GET
- Endpoint : `/api/editStudent/`

Response :

```json 
{
    "data" : {
        "nama" : "string",
        "universitas" : "string",
        "prodi" : "string",
        "tahun_masuk" : "date"
        "expertise" : "string",
        "skills" : "string",
        "deskripsi" : "string",
     }
}
```

## Edit Student

Request :
- Method : PUT
- Endpoint : `/api/editStudent/`
- Body :

```json 
{
       "nama" : "string",
       "universitas" : "string",
       "prodi" : "string",
       "tahun_masuk" : "date"
       "expertise" : "string",
       "skills" : "string",
       "deskripsi" : "string",
}
```

Response :

```json 
{
    "message" : "Berhasil melakukan perubahan"
}
```

## Dashboard Student

Request :
- Method : GET
- Endpoint : `/api/dashboardStudent/`

Response :

```json 
{
    "data" : {
         "posisi" : "string",
         "perusahaan" : "string",
         "status" : "string"
     }
}
```
## Profile Recruiter

Request :
- Method : GET
- Endpoint : `/api/profileRecruiter/`

Response :

```json 
{
    "data" : {
         "nama" : "string",
         "perusahaan" : "string",
         "limit" : "int",
     }
}
```

## lowongan

Request :
- Method : GET
- Endpoint : `/api/lowongan/`

Response :

```json 
{
    "data" : {
         "posisi" : "string",
         "status" : "string",
         "tenggat" : "date",
     }
}
```

## Delete lowongan

Request :
- Method : DELETE
- Endpoint : `/api/lowongan/:id`

Response :

```json 
{
    "message" : "Berhasil Delete"
}
```

## Tutup Lowongan

Request :
- Method : POST
- Endpoint : `/api/tutupLowongan/`
- Body :

```json 
{
    "status" : "string"
}
```

Response :

```json 
{
    "message" : "lowongan ditutup"
}
```


## View Detail Lowongan

Request :
- Method : GET
- Endpoint : `/api/detailLowongan/:id`

Response :

```json 
{    
    
     "data" : {
         "posisi" : "string",
         "perusahaan" : "string",
         "lokasi" : "string",
         "deskripsi" : "string"
     }
}
```

## View Edit Lowongan

Request :
- Method : GET
- Endpoint : `/api/editLowongan/:id`

Response :

```json 
{
     "data" : {
         "posisi" : "string",
         "perusahaan" : "string",
         "lokasi" : "string",
         "deskripsi" : "string"
     }
}
```

## Edit Lowongan

Request :
- Method : PUT
- Endpoint : `/api/editLowongan/:id`
- Body :

```json 
{
     "posisi" : "string",
     "perusahaan" : "string",
     "lokasi" : "string",
     "deskripsi" : "string"
}
```

Response :

```json 
{
    "message" : "Berhasil edit lowongan"
}
```

## View Applier

Request :
- Method : GET
- Endpoint : `/api/applier/:id`

Response :

```json 
{
    "data" : {
         "nama" : "string",
         "expertise" : "string",
         "no_telp" : "int"
     }
}
```




