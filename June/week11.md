<h1 align="center">🇯 June 🇯</h1>

## _(Monday) June 20_ 📢

>### Forrest Gump Ping-Pong API 🏓
```javascript
//Index
const express = require('express')
const api = express()
const morgan = require('morgan')

api.set('port', process.env.PORT || 3000);

//Middlewares
api.use(morgan("dev"));
api.use(express.json());

api.use('/api/testing', require('./routes/pingpong'));

api.get('/', (req, res) => {
    res.json({message: `Redirect to: http://localhost:3000/api/testing`});
})

api.listen(api.get("port"), () => {
    console.log(`Server running on port ${api.get("port")}`);
});
```

```javascript
//Routes
const { Router } = require("express")
const router = Router();

router.get('/', (req, res) => {
    res.json({ response: "This is a PingPong API"});
});

router.get('/ping', (req, res) => {
    res.status(200).json({message:"Pong!"});
});

router.get('/pong', function (req, res) {
    res.status(200).json({message:"Ping!"});
});

module.exports = router;
```
>#### Testing 🚀
<img src="/June/assets/pingpong.gif" alt="PingPong API" width="400">

>### Delayed Response API ⏳
```javascript
const express = require('express')
const api = express()

api.get("/api/delay/:delay", function(request, response){
    const delay = request.params.delay;
     setTimeout(function(){response.send("Hello World!")}, delay)
})

api.listen(3000, function() {
    console.log("Server running on http://localhost:3000/api/delay/3000")
});
```

## _(Wednesday) June 22_ 📢

>### Age Prediction API 👶-👴
```javascript
//Index
const express = require('express')
const api = express()
const morgan = require('morgan')

api.set('port', process.env.PORT || 8000);

//Middlewares
api.use(morgan("dev"));
api.use(express.json());

api.use('/api/age', require('./routes/ageprediction'));

api.get('/', (req, res) => {
    res.json({message: `Age Predictor API`});
})

api.listen(api.get("port"), () => {
    console.log(`Server running on port ${api.get("port")}`);
});
```

```javascript
//Routes
const { Router } = require("express")
const router = Router();

router.get('/', (req, res) => {
    res.json({ error: "Missing parameter 'name' was expected."});
});

router.get('/:name', (req, res) => {
    const year = 365;
    const {name} = req.params;
    randomAge = Math.floor(Math.random() * (101-0) + 0);
    ageOnDays = year * randomAge;
    
    res.status(200).json({name, age: `${randomAge}`, days: `${ageOnDays}`});
});

module.exports = router;
```

>#### Testing 🚀
<img src="/June/assets/agepred.gif" alt="Age Prediction API" width="400">

## [📎 Back to main page !📎](/home/readAura.md)
