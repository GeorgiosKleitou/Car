# REPORT COM519 ADVANCED DATABASE SYSTEMS


<h3> Information for the porject</h3>

- https://fine-rose-dalmatian-vest.cyclic.app
- https://github.com/GeorgiosKleitou/Car


<h2><strong><u>Introduction</u></strong></h2>

<p>This website is nothing but a prototype to me, it will be changed and be upgraded upon. The general idea for this website is a promise made to my
Father a bit before I started the university. My father is a mechanic so, promise was made that I will built a database website to help him access car details much easier that he already does. So the general idea came 
to build a website to display cars for car-heads, at least that is what it is at the moment. According to my father before a mechanic operates on a car he must familiarize himself with the car, that would involve an annoying process of hooking an electric I-Pad sort of thing to the car and take a certain amount of time before it diagnoses several staff. The database is meant ot help mechanics be familiarized with stock production cars, at least that is the future of the website. For now the website displays simple stuff, like model name,  engine, cylinders, horsepower etc. Of course if the car is modded that is another story. </p>

<i>(183 words)</i>

<h2><strong><u>System Overview</u></strong></h2>

<p>Before starting the website process a car database was needed. In my endeavors to find a decent car database nothing was found to my liking. That is when the idea of ChatGPT came to mind (<i>https://chat.openai.com/chat</i>). I asked the AI chat bot to create a database using Car model, Origin grouped by Europe, America and Japan, Brand, Horsepower, Cylinders, Year made, Engine and if its Electric or not. A request to the bot was made to include a bit of everything. I grabbed the list and placed it in a json file.</p>

<p>After downloading all the necessary libraries from the lectures and installing them, linked the mongodb to import the database to it with the helpe of the library mongoose. </p>

<p>The seeder only imports the car database as is, there was no need to change any display information as all of it is crucial to be displayed nor to aggregate anything extra, there was no purpose of doing it.</p>

<p>Later on production of a unique Boostrap was attempted but to no avail, every bootstrap template attempted to be used created errors and issues with the code, so I kept the original one from the lectures. Header and Footer were created in the common folder to be used for all of the interface. Header includes a navigation bar while footer functions like a "back to the top" function. Ejs files were created for each purpose of the website, including ejs that are only accessable after logging in. Some of them were created later with the making of their controllers.</p>

<p>The Models made for schemas are Cars, Origin, User and Brands. Car is the schema the car's info , made origin and brand schemas for the Origin and Brand to be a required field. User is a schematic for the user.</p>

<p>For the Controllers, the first creation was cars controller which consists of creating, deleting and sending the user to the update page and the update which updates the user and sends the user to the allcars page. 
Then followed by that the creation of home controller was made to be displayed on the index page, it aggregates the cars and brands so the index page can display how many cars and brands are in the database. 

Then that the user controller was made to include a login feature and a register feature. </p>

<p>Finally the three last controllers, europe, japan and america were made to display pages of the cars specified Origin and include on the page the same update, creation and deletion that cars controllers has.</p>

<p>All of the routing is done to our controllers in app.js including the connection to the mongodb with mongoose with express. In app.js you can see everything is rendering to the correct places, the middle ware is applied and the funcitons of our controller are routed.</p>

<p> Towards the end an API was made to be able to search for cars on the website by brand so the user can feel more comfortable finding cars.</p>

<p>Cyclic took a while to get the handle of it but ultimately took the link from the repository, linked it with my already existing repository (yes, no need to have an empty one) and parsed in my existing mongodb database.</p>

<h2><strong><u>How the website functions for the user</u></strong></h2>

<p>User registers, if the user registers then the user can login. If the user is not logged in he cannot edit or delete anything from the database. Since the website is online everyone can get on it and delete everything inside the database which is not very secure but I wanted to include a register system. The user can choose to see all the existing cars, search the cars by origin, search for a car brand, and if logged in, add a car to the database. The navigation and selections are very user and car-head friendy</p>

<i>(542 words)</i>


<h2><strong><u>Conlcusion & Reflection</u></strong></h2>
<p>The website was built in a very short time frame. The amount of time left from other assessments did not make it easier as this assessment was a big undertaking. The website funcitons but is not as good as I have hoped it to be. Attempts were made to better it by adding more stuff but ultimately resorted in erros. Most of the time wasted was with setting up Github as VsCode Github has put me to a halt many times, creating other repos and had to delete everything and download Github GUI to save my repos from there. Due to the time pressure the website follows everything learned in class. I believe the website I am planning on building will have merit and I will work on it to shape it to what I want. </p>

<i>(139 words)</i>
