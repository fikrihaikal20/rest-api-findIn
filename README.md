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
         "passwaord" : "string",
         "nama" : "string",
         "no_telp" : "int",
         "universitas" : "string",
         "prodi" : "string",
         "nim" : "int",
         "nik" : "int",
         "tahun masuk" : "date",
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
         "passwaord" : "string",
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
         "video" : 
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
         "tipe" : "part time | full time",
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
         "tipe" : "part time | full time",
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
         "tipe" : "part time | full time",
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
         "tipe" : "part time | full time",
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
         "tipe" : "part time | full time",
         "deskripsi" : "string",
         "tenggat" : "date",
         "panduan" : " ",
     }
}
```

Response :

```json 
{
    "message" : " "
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
         "cv" : " ",
         "resume" : " ",
     }
}
```

Response :

```json 
{
    "message" : " "
}
```

## Profile Student

Request :
- Method : GET
- Endpoint : `/api/profileStudent/`

Response :

```json 
{
    "message" : " "
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
         "cv" : " ",
         "resume" : " ",
     }
}
```

Response :

```json 
{
    "message" : " "
}
```

## View Edit Student

Request :
- Method : GET
- Endpoint : `/api/editStudent/`

Response :

```json 
{
    "message" : " "
}
```

## Edit Student

Request :
- Method : PUT
- Endpoint : `/api/editStudent/`
- Body :

```json 
{
    "data" : {
         "cv" : " ",
         "resume" : " ",
     }
}
```

Response :

```json 
{
    "message" : " "
}
```

## Dashboard Student

Request :
- Method : GET
- Endpoint : `/api/dashboardStudent/`

Response :

```json 
{
    "message" : " "
}
```
## Profile Recruiter

Request :
- Method : GET
- Endpoint : `/api/profileRecruiter/`

Response :

```json 
{
    "message" : " "
}
```

## lowongan

Request :
- Method : GET
- Endpoint : `/api/lowongan/`

Response :

```json 
{
    "message" : " "
}
```

## Delete lowongan

Request :
- Method : DELETE
- Endpoint : `/api/lowongan/`
- Body :

```json 
{
    "data" : {
         "cv" : " ",
         "resume" : " ",
     }
}
```

Response :

```json 
{
    "message" : " "
}
```

## Tutup Lowongan

Request :
- Method : POST
- Endpoint : `/api/tutupLowongan/`
- Body :

```json 
{
    "data" : {
         "cv" : " ",
         "resume" : " ",
     }
}
```

Response :

```json 
{
    "message" : " "
}
```


## View Detail Lowongan

Request :
- Method : GET
- Endpoint : `/api/detailLowongan/:id`

Response :

```json 
{
    "message" : " "
}
```

## View Edit Lowongan

Request :
- Method : GET
- Endpoint : `/api/editLowongan/:id`

Response :

```json 
{
    "message" : " "
}
```

## Edit Lowongan

Request :
- Method : PUT
- Endpoint : `/api/editLowongan/:id`
- Body :

```json 
{
    "data" : {
         "cv" : " ",
         "resume" : " ",
     }
}
```

Response :

```json 
{
    "message" : " "
}
```

## View Applier

Request :
- Method : GET
- Endpoint : `/api/applier/:id`

Response :

```json 
{
    "message" : " "
}
```




