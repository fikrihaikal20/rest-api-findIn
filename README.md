# API Spec

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
         "id" : "string, unique",
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

