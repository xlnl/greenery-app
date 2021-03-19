# Greenery

### App Demo: Pending!
<!-- Click [here!](TBD) -->
----------------------------------------------


### Context: 
Inspired by Scotts Miracle Gro My Garden App, which is centered on a digital transformation project for one of my American University's MS Analytics foundational courses, Greenery will provide users the ability to explore and add plants, specifically plants native to their area, to their virtual garden. 

The intention is for users to be inspired to research how to successfully grow plants in a sustainable, bee-friendly way with a virtual garden dashboard catered to delivering necessary information all within the palm of their hands.

----------------------------------------------------------
### Wireframes

Click [here](https://www.figma.com/file/BK1JJaT9Xe3EENsCIF8sxZ/Greenery?node-id=0%3A1) to view the wireframes of Greenery 

### ERD 

Click [here](https://whimsical.com/greenery-erd-P6bCadqEwB85K6B6UhSsXM) to view the entity-relationship diagram of Greenery.

### User Stories

1. As a user, I want to be able to search for plants in general and within my distribution zone. 
2. As a user, I want to be able to read more details about a specific plant, including its growth descriptions and picture. 
3. As a user, I want to be able to save the plant and store it in my virtual garden.
4. As a user, I want to be able to comment on a plant and offer any additional insights I might have. 
5. (**Stretch**) As a user, I want to be able to write notes about my saved plants to reflect on its growth progress.
6. (**Stretch**) As a user, I want to be able to further keep track of plant's growth progress through a tracking form.  
7. (**Stretch**) As a user, I want to be able to see data visualizations of my plant's growth process based on my progress tracker.

----------------------------------------------------------
### Approach

I took inspiration from an app that my group is working on enhancing with AR capabilities for a grad class. I wanted to combine beautiful, user-friendly design with easy functionality. This inspiration was further solidified by my encounter of the beautiful global plants API, [Trefle](https://trefle.io./). 

----------------------------------------------------------
### Unsolved Problems

TBD

----------------------------------------------------------
### Technologies Used
* Whimsicle for ERD 
* Figma for wireframing
* VS Code Text Editor + Node.js + Express + Postgres + Sequelize + Bootstrap/CSS + Javascript + HTML
----------------------------------------------------------
## How to set up from starter code/boilerplate: 

1. Fork & clone this repo

2. Install dependencies
```
npm i
```

3. create a config.json with the following code: 
```
{
  "development": {
    "database": "<insert develop db name here>",
    "host": "127.0.0.1",
    "dialect": "postgres"
  },
  "test": {
    "database": "<insert test db name here>",
    "host": "127.0.0.1",
    "dialect": "postgres"
  },
  "production": {
    "database": "<insert production db name here>",
    "host": "127.0.0.1",
    "dialect": "postgres"
  }
}

```
**Note:** If your database requires a username and password, you'll need to include these as well.

4. Create database
```
sequelize db:create <insert db name here>
```
5. Migrate the `user` model to your database
```
sequelize db:migrate
```
6. Seed all the provinces
```
sequelize db:seed:all
```
7. Add `SESSION_SECRET` and `PORT` environment variables in a `.env` file (can be any string). If planning to use a maps API, make sure you put that as an environment variable as well.

