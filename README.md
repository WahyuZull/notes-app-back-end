# Notes App API
Submission Kelas Belajar Membuat Aplikasi Back-End untuk pemula - Dicoding.com


## Base URL

https://notesapp-backend.netlify.app

## Endpoints

### Get List of Notes

> Mendapatkan daftar catatan

- URL: `/notes`
- Method: `GET`
- Response:

```json
[   
    {
        id: 9,
        tags: "terselesaikan",
        body: "Fixed a bug in the authentication flow",
        title: "Bug Fix",
        createdAt: new Date(),
        updatedAt: new Date(),
    },
    {
        id: 10,
        tags: "belum terselesaikan",
        body: "Implemented a new feature for user profile customization",
        title: "New Feature",
        createdAt: new Date(),
        updatedAt: new Date(),
    },
    {
        id: 11,
        tags: "terselesaikan",
        body: "Refactored the codebase for better readability and performance",
        title: "Code Refactor",
        createdAt: new Date(),
        updatedAt: new Date(),
    },
]
```

### Get Detail of Note

> Mendapatkan detail catatan

- URL: `/notes/:id`
- Method: `GET`
- Response:

```json
{
    id: 9,
    tags: "terselesaikan",
    body: "Fixed a bug in the authentication flow",
    title: "Bug Fix",
    createdAt: new Date(),
    updatedAt: new Date(),
},
```

### Post Note

> Menambahkan catatan

- URL: `/notes`
- Method: `POST`
- Response:

```json
{
    id: 9,
    tags: "terselesaikan",
    body: "Fixed a bug in the authentication flow",
    title: "Bug Fix",
}
```

### Edit Note

> Mengubah catatan

- URL: `/notes/:id`
- Method: `PUT`
- Response:

```json
{
    id: 9,
    tags: "terselesaikan",
    body: "Fixed a bug in the authentication flow",
    title: "Bug Fix",
    createdAt: new Date(),
    updatedAt: new Date(),
},
```

### Delete Note

> Menghapus catatan

- URL: `/notes/:id`
- Method: `DELETE`
- Response:

```json
{}
```
