# #100DaysOfCode Log - Round 1 - Anja Thiart

The log of my #100DaysOfCode challenge. Started on 2 August 2020

## Initial goal
I want to complete CS50 Web, the follow up to CS50 Computer Science. 
In parrallel to the above, I want to develop my personal website and incorporate my projects from the course, as well as the preceding course, as I go along.

## Log

### R1D1 - 20200802
My first day. I created this repo. I updated the last project I worked on's repo (called Taper Journey) and found the video I made demonstrating it and added that to the repo. Also pushed psets from that course (CS50 Intro...) to a private repo.

### R1D2 - 20200803
Watched CS50W lecture 1 (HTML, CSS) and 2 (GIT). Started with project 0 creating the home page (normal search) of a google search frontend / clone. The css will be reusable on each page.

### R1D3 - 20200804
I worked on project 0 on the image search and advanced search pages. I learnt that the name of a form input becomes the query paramater keys (don't know how I didn't know that before). Functionality is complete. I did have to use some javascript for the google "I'm feeling lucky" search clone (not sure if this was intended for the project). Now I have some styling left and the screencast.

### R1D4 - 20200805
Today I completec coding up the google clone frontend. I was reminded that I often read over things too quickly, since on second reading over the project brief, they actually make it clear that the 'name' attributes become the query parameters. I have submitted the code to Submit50 but still need to make the video and fill the form.

### R1D05 - 20200806
Submitted the YouTube video of Project 0 and everything (https://www.youtube.com/watch?v=05eHUQ03eMA&feature=youtu.be). I learnt how to timestamp youtube vids. I also watched the Python lecture. Was reminded of decorators and how I can see it functioning as middleware. Looks like we'll be using OOP as well which I need to touch up on.

### R1D06 - 20200807
Added my google search clone to my github account https://github.com/anjathiart/google-search-clone. Watched the lecture on Django. Python-Django is totally different to what I'm used to using Node-Vue. But as I follow along I can tell how the one method relates to the methods used at work. It's a new way of thinking about it which is good. The tooling / configuration / structure of a python-django app is a mindset shift for me.

### R1D07 - 20200808
Started Project 1: Wiki (CS50W). I'm getting used to the Django frontend and folder structure. I'm confused with the "not namespaced" error I get as I believe that I am implementing things namespaced. I'm sure it will make sense later on. I've implemented a dynamic route for viewing entries, as well as an error page for 404 not found.

### R1D08 - 20200809
Continued with my wiki. I'm struggling a bit with the django-python syntax but getting there. I spent quite some time on some pretty obvious bugs. My search route is working and displaying correctly now. I'm also feeling more comfortable with render vs redirect. I have also learnt that changes to my css does not automatically get registered and for that, I must bypass the cache with a hard refresh. This is not the case with Vue.

### R1D09 - 20200810
I have implemented the new entry creation as well as the edit views / templates and it is working fine. I learnt that, for some reason, Django will throw errors for view / url variables referenced, even if that code is commented out in the html template. I am not using "reverse" and I don't understand how it works, which is bothering me.

### R1D10 - 20200811
Lost track of time playing around with python regEx syntax in an attempt to write a markdown-to-html parser. I finished all the functionality of the wiki, including the random entry page and rendering the entry pages as HTML and not markdown (using the python markdown2 package). Now I'm intrigued by writing my own parser. The RE syntax and inner workings is baffling me, but after playing around for 3 hours (with a lot of hardcoding) I am closer to understanding it that I've ever been, even though I don't understand much at all. Keen to maybe polish off this project using Markdown2 package, and then start a new mini-side project to write my own markdown-to-html parser, as I can see this is going to be a rabbit hole.

### R1D11 - 20200812
Worked on Wiki project. Condensed some django view functions that didn't need to be separate, removed the markdown-parser I was playing with. Tweaked the styling slighly. Next I want to use a lamda function to filter out items of a sequence (array).

### R1D12 - 20200813
I completed and submitted CS50W project 1: wiki.  I converted my search view to use filter-lambda function and also learnt how to do an inline if-else statement in python (I'm used to using terneray operators in JS). Brief video link here: https://www.youtube.com/watch?v=y9Ef_KkbobQ&feature=youtu.be.

### R1D13 - 20200814
Watched CS50W leture 4: SQL, Models and Migrations. A lot of new things. I like this idea of models and how simple it is to interact with the data. I learnt that the reverse() function in Django is like redirect. It can take a field args="" in case there are parameters that the view function takes in. I learnt that the HTML/Django template also has access to the request that rendered it. Authentication and loggin in and out looks so easy using the Django libraries for it. I'm curious to see how middleware and so on fit in with Django, but I suppose that comes in with APIs. What defines something as an API anyway? The Django admin app to interact with the sqlite db is cool. I wonder how it works when using mysql instead. I learnt that Django comes with mysql out the box.

### R1D14 - 20200815
Started planning out the next project, commerce. Its a simple e-commerce auction interface (think eBay). I've started thinking about and mapping out what my sqlite / django models will look like and how they will be related to each other. A requirement that isn't listed in the brief, but that I think is important, is to add some form of notification panel where one can see if your listings were commented on, bidded on, or if you have won a bid for an item you wanted.

### R1D15 - 20200816
Filled out more of the django models for commerce project. I also started writing the HTML templates. All new to me so I'm learning as I go. I need to add some data so that I can test my views, models and pages. Will do that next before I carry on with the dev.

### R1D16 - 20200817
Worked on Commerce project. I am busy implementing the "new listing" page and am successfully capturing and displaying the latter. I still have to do proper validation. I've learnt that the user details is contained in the request object. I also setup the superuser and can now interact with my db data from the admin dashboard. I'm getting frustrated with the bootstrap classes messing with what I would expect. I will probably remove bootstrap later, but then I might go down a styling rabbit hole - which is not the aim of this particular project.

### R1D17 - 20200818
Worked on Commerce project by imnplementing the create_bid route and related django models. I'm slowly getting the hang of the latter, more like getting the hang of how to ask google for help effectively. I figured out that to update manyToMany fields one has to first get the object as a new object, then add the field, then save it again; you cannot use .update(). Didn't spend time on styling; I'm enjoying learning the django patterns / syntax.

### R1D18 - 20200819
I really didn't feel like doing this today, but eventually just started and here I am. Worked on commerce project. I'm working on the bids logic for a listing. I haven't done validation yet, but making a bid and retrieving the maximum bid of a listing is working. Also went in circles on how to model the Watchlist links, and decided in the end to create its own model. Spending a lot of time in the Django query docs. Enjoying it. Also learnt that splitting lines in python requires a '\' at the end. Small victories.

### R1D19 - 20200820
Worked on commerce project. Worked on watchlist view / url / models. Realised eventually that having a separate watchlist model was hacky and does not make much sense. Some things become very clear when you start implementing it. Django models are still abstract in my mind, and I forget that relating objects as foreign keys constructs that "link" for you in the background. I have a small bug with hitting "back" in the browser that came about where I redirect back to the same page that the watchlist form submission came from. Will look at that later.

### R1D20 - 20200821
Commerce Project: frustrating struggling with getting queries on manytomany fields of an object working, but eventually got somewhere (near the end). I've changed the watchlist logic successfully but that is a bit all. Still have some weird bugginess with the add / remove redirecting (mentioned some issues on previous day's commit). 
