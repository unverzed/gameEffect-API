<div align="center">
<h1>GameEffect. 🎮 </h1>
  </div>
  
<div align="center">
  <p> <a href="https://game-effect-front-end.vercel.app">deploy: gameEffect - vercel</a></p>
  </div> 
  <h2>Project:</h2>
<p>App to rate games, insert a game into the database, rate, favorite, comment on your favorite and most played games and see other people avaliations.
</p>

<h2>Overview:</h2>
<div align="center">
<img src="https://media.discordapp.net/attachments/908466335158272132/1049356196601147502/Untitled.png?width=946&height=473"/>
 </div> 


<h2>Technologies:</h2>
<div align="center">
<img src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white">
<img src="https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white">
<img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white">
<img src="https://img.shields.io/badge/Prisma-3982CE?style=for-the-badge&logo=Prisma&logoColor=white">
  </div>
  
<h2>Routes:</h2>

```yml 
POST /signup
    - Create an account
    - headers: {}
    - body:{
        "email": "user@gmail.com",
        "password": "user00",
        "username": "user_01",
        "bio": "hello, i'm user and i like games",
        "icon": "https://i.pinimg.com/564x/24/73/c0/2473c02e2ac93f617a28b2b5058bb41d.jpg",
} 
```

```yml 
POST /
    - Login with your account
    - headers: {}
    - body:{
       "login": "user@gmail.com" || "user_01",
       "password": "user00"
}    
```

```yml 
GET /game
    - Search for all games in database
    - headers: "Authorization": "Bearer $token"
    - body:{} 
```

```yml 
GET /recent
    - Return all recent games in database
    - headers: "Authorization": "Bearer $token"
    - body:{} 
```

```yml 
GET /jrpg
    - Return all games by jrpg genre
    - headers: "Authorization": "Bearer $token"
    - body:{} 
```

```yml 

GET /game/:id
    - Should appear the game page 
    - headers: "Authorization": "Bearer $token"
    - body:{} 
```

```yml 

POST /game
    - Should post your game in database
    - headers: "Authorization": "Bearer $token"
    - body:{
        "name": "Persona 5 The Royal",
        "genre": "J-RPG",
        "releaseDate": "15/09/2016",
        "description": "Persona 5 acontece na Tóquio de hoje e segue o protagonista Joker após sua transferência para a Academia Shujin após ser colocado em liberdade condicional por um assalto do qual ele foi falsamente acusado.",
        "pictureUrl": "https://image.api.playstation.com/vulcan/img/cfn/113073qYZHyiDU5-4vu9krqfIPdGCvcGob0VpazrmfyUEbn4qZ64XBJfRKHvwa_tStB4nMD3UDv4Cb9V3iTH6cJymhQ1sJiU.png"
    } 
```

```yml 

POST /game/:id/avaliation
    - Should post an avaliation 
    - headers: "Authorization": "Bearer $token"
    - body:{
          "review": "best game",
          "rate": 5,
          "isFavorite": true
    } 
```

```yml 

GET /game/:id/avaliations
    - Return all avaliations from id game
    - headers: "Authorization": "Bearer $token"
    - body:{} 
```

```yml 

GET /game/:id/rate
    - Return rate from game
    - headers: "Authorization": "Bearer $token"
    - body:{} 
```

```yml 

GET /user/:id
    - Should return user profile
    - headers: "Authorization": "Bearer $token"
    - body:{} 
```

```yml 

PUT /user/:id
    - Should edit the profile info
    - headers: "Authorization": "Bearer $token"
    - body:{
          "bio": "i'm user with a profile edited"
          "icon": "https://64.media.tumblr.com/da87c61d5d7f2bdfe2ae628b42dab196/9bfac5803c11635e-7d/s1280x1920/724bd6a3e3b59f43b5883df081f0838357d0d0e3.jpg"
    } 
```

```yml 

GET /:id
    - Should return 3 favorite games 
    - headers: "Authorization": "Bearer $token"
    - body:{} 
```
```yml 

GET /:id/recent
    - Should return the avaliations with rate
    - headers: "Authorization": "Bearer $token"
    - body:{} 
```

<h2>How to run:</h2>

<h3>Clone the repository:</h3>

```
$ git clone https://github.com/unverzed/gameEffect-front-end.git
```

<h3>Install dependencies:</h3>

```
$ npm or yarn install
```

<h3>Initializing the API:</h3>

```
$ npm start
```

## Author:
  [<img src="https://avatars.githubusercontent.com/unverzed" width=115><br><sub>Vitória Ortega</sub></sub>](https://github.com/unverzed) 
