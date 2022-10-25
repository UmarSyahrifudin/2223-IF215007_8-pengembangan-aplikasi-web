```javascript

const express = require('express')
const app = express()
const port = 3000
const cors = require('cors')

app.use(cors({
    origin: '*'
}));

app.get('/', (req, res) => {
  res.send('Hello, Selamat Datang Di Your Guide!')
})

// Tambah Rute
app.post('/rute', (req, res) => {
    res.json(
      {
        id: 32432,
        author:"umar",
        content: "langsung aja dipraktekkan ya, sebelum install express, kita install dulu nodemon, nodemon ini dipake untuk eksekusi file javascript, mirip ama node, bedanya nodemon mantau perubahan filenya, dan auto restart kalo filenya diubah. Jadi ga usah repot stop start stop start kalo beres edit",
        gambar: "gambar",
      }
    )
  })

// Lihat list Rute
app.get('/rute', (req, res) => {
    res.json([
      {
        judul: "Rute Ke PVJ dari Cicalengka",
        author:"umar",
        content: "langsung aja dipraktekkan ya, sebelum install express, kita install dulu nodemon, nodemon ini dipake untuk eksekusi file javascript, mirip ama node, bedanya nodemon mantau perubahan filenya, dan auto restart kalo filenya diubah. Jadi ga usah repot stop start stop start kalo beres edit",
        gambar: "gambar",
      },
      {
        judul: "Rute Ke PVJ dari Cicalengka",
        author:"umar",
        content: "langsung aja dipraktekkan ya, sebelum install express, kita install dulu nodemon, nodemon ini dipake untuk eksekusi file javascript, mirip ama node, bedanya nodemon mantau perubahan filenya, dan auto restart kalo filenya diubah. Jadi ga usah repot stop start stop start kalo beres edit",
        gambar: "gambar",
      }    
    ])
  })
  
  // Lihat detail Rute
  app.get('/rute/:id', (req, res) => {
    res.json(
      {
        judul: "Rute Ke PVJ dari Cicalengka",
        author:"umar",
        content: "langsung aja dipraktekkan ya, sebelum install express, kita install dulu nodemon, nodemon ini dipake untuk eksekusi file javascript, mirip ama node, bedanya nodemon mantau perubahan filenya, dan auto restart kalo filenya diubah. Jadi ga usah repot stop start stop start kalo beres edit",
        gambar: "gambar",
      }
    )
  })


// Hapus Rute
  app.put('/rute/:id', (req, res) => {
     res.json(
         {
          id: 32432,
          author:"umar",
          content: "langsung aja dipraktekkan ya, sebelum install express, kita install dulu nodemon, nodemon ini dipake untuk eksekusi file javascript, mirip ama node, bedanya nodemon mantau perubahan filenya, dan auto restart kalo filenya diubah. Jadi ga usah repot stop start stop start kalo beres edit",
          gambar: "gambar",
        }
      )
    })
  
  
  // Hapus Rute
  app.delete('/rute/:id', (req, res) => {
    res.json(
      {
        id: 32432,
        author:"umar",
        content: "langsung aja dipraktekkan ya, sebelum install express, kita install dulu nodemon, nodemon ini dipake untuk eksekusi file javascript, mirip ama node, bedanya nodemon mantau perubahan filenya, dan auto restart kalo filenya diubah. Jadi ga usah repot stop start stop start kalo beres edit",
        gambar: "gambar",
      }
    )
  })
  
app.listen(port, () => {
    console.log(`Example app listening on port ${port}`)
  })



```
