# auctioner 
API-DOKUMENTATION
1.	Get all products
To get all the existing products from the database you will have to make a get request on: 
 
http://localhost:3000/data/products

2. For a specific auction:
To get information about a specific auction you will have to make a get request on:

 http://localhost:3000/data/auction/:id

3. Get auction based on search keyword:
To get specific products based on a search keyword you will have to make a get request on:

 http://localhost:3000/data/search/:keyword

4. Post new account:
To register an account in the database you need to make a post request on:
http://localhost:3000/data/user 
 
5. Log-in request, log-in status and log ut: 
To make a login request you will have to post one existing email address and a password that matches the email address on:
 http://localhost:3000/data/login 
and get a Boolean message if the login was successful or if it failed.

To check if a user is currently logged in on the webpage you need to make a get request on:
http://localhost:3000/data/login 
and will then get a Boolean message if the user is logged in or not.

To log out from an account you will have to make a Delete request on: 
http://localhost:3000/data/login 
and the user will be logged out from the page.

6. Place a bid on an auction
To place a bid, you must be logged in as a user on the website, then you will have to make a put request on the following link: 
http://localhost:3000/data/auction/:id

 
7. Add an auction to the database:
To add an auction to the database you will have to make a post request on:
 http://localhost:3000/data/auctions 
that makes with all the data needed to create an auction.

 
8. Get auctions based on a specific category and keyword:
To get auctions based on a specific category you will have to make a get request on:
 http://localhost:3000/data/search/categories/:category

and to get auctions based on a specific category and keyword together you will have to make a get request on:
 http://localhost:3000/data/search/categories/:category/:keyword

9. Get auctions that have not been sold:
To list all the auctions that have not been sold you will have to make a get request on:
 http://localhost:3000/data/status/not-sold

10. Get all auctions that have been sold:
To list all the auctions that have been sold you will have to make a get request on:
http://localhost:3000/data/status/sold

11.  all ongoing auctions:
To get all ongoing auctions you will have to make a get request on:
http://localhost:3000/data/status/ongoing

12. Get all finished auctions:
To do that you will have to make a get request on:
http://localhost:3000/data/status/completed

13. Get all auctions logged in users have made:
 To list all the auctions that the logged-in user has made you have to make a get request on:
 http://localhost:3000/data/my-auctions

14. Get all auctions where the logged-in user has made a bid:
To list all the auctions that the logged-in user has made a bid on you have to make a get request on:
 http://localhost:3000/data/my-bids

15. Get a specific profile page from an existing user:
To get a profile page from the database you will have to make a get request on:
http://localhost:3000/data/profiles/:id
