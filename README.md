# Demo NODE&Express Server

## Launch Server
- ```npm install```
- ```npm start``` 
 
- Server listenning on http://localhost:5000

- Routes available :
  * '/' => Welcome Server Home
  * '/articles/' => METHOD GET -> ALL ARTICLES
  * '/articles/' => METHOD POST -> CREATE ARTICLE
  * '/articles/:id' => METHOD GET -> READ ARTICLE
  * '/articles/:id' => METHOD POST -> UPDATE ARTICLE
  * '/articles/:id' => METHOD DELETE -> DELETE ONE ARTICLE
  
## Access To BDD
- add .env file following exemple in .example-env file 
- if you don't have BDD :
- connect to your mysql server 
- ```mysql -u <USERNAME> -p```

#### then run this commands to create `e-shop-node` database and `article` table :

- ``` CREATE DATABASE `e-shop-node`;``` 
- ``` CREATE TABLE `article` (
  `id` INT NOT NULL AUTO_INCREMENT PRIMARY KEY,
  `title` VARCHAR(255) NOT NULL,
  `image` LONGTEXT NOT NULL,
  `content` LONGTEXT NOT NULL,
  `price` INT NOT NULL
  ); ```

#### then add some data :
- ``` INSERT INTO `article` (`id`, `title`, `content`, `image`, `price`) VALUES
    (1, 'Lacoste Chemise Ricky Regal', 'lorem ipsum', 'https://lh3.googleusercontent.com/gVfUbDsexJ5M83kuqzijWixn5tzIXu9Y2pyBfmciQMF50-T2TqoDuKnmvNVtoTMNETDp7BISqdrlM7x1dUSnN_PSzJW13pNXc5Y_l0DgnuyfuV6ZspSwRgPshhaQR3buqdUmlS63', 150),
    (2, 'Lacoste Ricky Regale Velour', 'lorem ipsum', 'https://image1.lacoste.com/dw/image/v2/AAQM_PRD/on/demandware.static/Sites-FR-Site/Sites-master/fr/dw29f8dee1/PH1693_4SN_20.jpg', 220); ```
