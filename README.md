////////////////// step 01 \\\\\\\\\\\\\\\\\\\\\\\\\
1. goto node express (website)
2. create folder name (cmd mkdir <file name>
  2.1 cd <folder name> goto previous folder
3. npm init -y (-y if you have all default setup or you can setup strep by strep)
4. create a entry index.js file 
5. npm i express cors (instal express and cors)

////////////////// step 02 \\\\\\\\\\\\\\\\\\\\\\\\\
1. create a API 
2. API listen 
3. sent request to path name

////////////////// step 03 (example) \\\\\\\\\\\\\\\\\\\\\\\\\
1. const express = require('express') 
2. const cors = require('cors')
3. const app = express()
4. const port =process.env.PORT || 5000
5. app.use(cors())

6. app.get('/', (req, res) => { (rote file show this content)
7.  res.send('travel master is a Home page') // it show 
8. })

9. app.listen(port, () => {     ////start port//
10.  console.log(`Example app listening on port ${port}`)
11. })

////////////////// step 04 \\\\\\\\\\\\\\\\\\\\\\\\\
 ---------------- your build a api -------------- \\
 1. data/hotels.json
 ---------------- you get a api -------------- \\
 2. app.get('/hotels', (req, res) => {
 3.    res.send(require('./data/hotels.json'))
 4.  })

////////////////// step 05 \\\\\\\\\\\\\\\\\\\\\\\\\
 -------------upload your data -----------------
1. vercel (and answer) // .......yeah upload your site

////////////////// step 06 \\\\\\\\\\\\\\\\\\\\\\\\\
--------------- update server --------------\\
1. vercel --prod
