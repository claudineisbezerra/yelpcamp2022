# yelpcamp2022
The Web Developer Bootcamp 2022

## Table of Contents

  - [Installing](#installing)
  - [Database](#database)
  - [Environment Variables](#environment-variables)
  - [Deployment](#deployment)
  - [Dependency Libraries](#dependency-libraries)



## Installing

Create NodeJs App and package.json file:

```bash
$ npm init --yes
```

Clone repository from GitHub:

```bash
git clone https://github.com/claudineisbezerra/yelpcamp2022.git
```

Create reference to GitHub REPO and updates in REPO:

```bash
git remote -v
git remote add origin https://github.com/claudineisbezerra/yelpcamp2022.git
git add .
git commit -m "Description of the change"
git push -u origin master
```


## Database

Local MongDB reference:

```js
mongodb://localhost:27017/yelpCamp
```

Remote MongDB reference using Atlas Service hosted by AWS:

```js
mongodb+srv://[user]:[Password]@[server pefix name].mongodb.net/yelpCamp?retryWrites=true&w=majority
```

## Environment Variables

App Environment Variables:

```js
MAPBOX_TOKEN=[Private mapbox token]
SECRET=[Private secret session authentication]
DB_URL=[MOngoDB URL]
PORT=[Default por number ex: 3000]
CLOUDINARY_CLOUD_NAME=[from Cloudinary]
CLOUDINARY_KEY=[from Cloudinary]
CLOUDINARY_SECRET=[from Cloudinary]
CLOUDINARY_ACCOUNT=zerohum
CLOUDINARY_URL=[from Cloudinary]
```


## Deployment

Create App on Heroku

```heroku
heroku login
heroku create
heroku logs --tail

heroku ps:scale web=0
heroku ps:scale web=1
heroku ps:scale web=2

heroku open

```

Install App on Heroku

```bash
git remote -v
git push heroku master
```


## Dependency Libraries 

```bash
npm install @mapbox/mapbox-sdk --save
npm install cloudinary --save
npm install connect-flash --save
npm install connect-mongo --save
npm install dotenv --save
npm install method-override --save
npm install ejs --save
npm install ejs-mate --save
npm install express --save 
npm install express-mongo-sanitize --save
npm install express-session --save
npm install helmet --save
npm install joi --save
npm install mongoose --save
npm install multer --save
npm install multer-storage-cloudinary --save
npm install passport --save
npm install passport-local --save
npm install passport-local-mongoose --save
npm install sanitize-html --save
```