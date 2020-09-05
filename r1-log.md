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

### R1D21 - 20200822
Commerce project. I fixed small bugs with the watchlist route (view according to Django). I worked on the bidding logic for a listing (first bidder min value, >1 bid min value, place or accept bid based on who the user is). The "accept_bid" route still needs to be done. I also worked on adding comments to a listing. I have a lot of styling left to do but most of the logic is there.

### R1D22 - 20200823
Working on commerce project. Added a view for accepting a bid, and working on the categories implementation. My design for the latter is not great. I'm a bit frustrated as it feels like I'm trying to hammer everything together with the "nails" that I have, i.e. the little knowledge that I have. Instead, I know there are cleaner, less messy and more efficient ways to work with the django models. I will have to go over the documentation patiently before forming these kind of habits.

### R1D23 - 20200824
Working on commerce project. I think I made a breakthrough in understanding the "related_name" field in the Django models. I have shuffled my models around and it is much cleaner now. The implementation is also much cleaner now. I link comments and bids to listings in the respective models, leaving it out of the listings model explicitly. I also realise that I have way too many "views", and can merge them. For example my filter view can just be a GET with query params on the index view, and creating a listing can be a POST on the listing view. Similar with commenting. But then I will have a lot of conditionals within the Listing view. I'm not sure what the cleanest way to do this is. But, my filter view is now working and was quite simple once I refactored my django models.

### R1D24 - 20200825
Commerce project. I moved the absorbed the filter view into the index view. I learnt how to pass dynamic query strins via the href tag. I also confirmed to myself today that python variables have function / program scope, but not block scope when it comes to if / for / while and so on. Useful to know. I realised I didn't think my index view through enough yet, as current price has to be added to the filtered results, and this requires an annotation on a reverse query (made using 'related_name'. But I have left these few things and got stuck into the styling. I'm using Sass. I have started on the index page making cards and the side nav showing categories. I am using https://javisperez.github.io/tailwindcolorshades/#/ to generate some shades of blue (my primary colour), and https://jsonformatter.org/css-to-sass to convert between css and sass where needed. Styling is a rabbit hole, but quite fun.

### R1D25 - 20200826
Felt exhausted today and almost skipped. Working on commerce project styling. Specifically styling the headernav, side nav, and listing cards. I made a small breakthrough with flex-box today. I'm forever struggling with justify-self. Learnt that you must use margin-left auto, or margin-right auto, instead. Hmm. I'm also organizing my sass styles in a way that is general so that it can be applied accross all pages.

### R1D26 - 20200827
Commerce project. Worked today on styling the listing page with comments. Tweaking the layout and styling is very finnicky. Don't want to spend too much time doing it as this can become a time drain. Refactored my HTML and Sass style-nesting to make logical sense and I find doing the latter well helps one see how parent elemenents impact children. So it is quite important to spend some time thinking of how to structure the html and sass.

### R1D27 - 20200828
Still on the commerce project and still styling the listing page. My html was becoming so nested and mangled, so too my sass file. Changed my mind on the layout and tweaking it constantly. Flex align-self / justify-self is not working for me. I need to read up a bit more about it. I think flex-stretch too. And perhaps it's time to start using css-grid. I've been avoiding it ever since, but flex-box now feels natural so I just need to get to the same point with grid.

### R1D28 - 20200829
Worked on styling and UI for the commerce projects. I untangled my html and refactored a lot of the sass and also realised that I have been using flexbox wrong for a long time. I though that align-items start is the same as the default and now I learnt that 'stretch' is the default and usually what you want. And I have been specifying align-items: start for a long time then trying to tweak the layout to fit that. And then margin-auto to align chldren works perfectly.

### R1D29 - 20200830
Working on Commerce project. I have updated the layout / styling on my login / register / create pages to match the other pages. I returned to the backend and am now understanding the django queries as it relates to related_name of linked objects, so I'm annotating info required in the template within a query instead of drilling down into each model. Bids / current prices are showing now in the related pages. I've added dates to comments and they are displayed chronologically now. I'm not going to spend too much time on styling from here. Now it is polishing off the logic, properly validating input / output, displaying validation messages on the page and also creating an error page. The user also needs to be notified if / when their bid is accepted.

### R1D30 - 20200831
Working on Commerce project. I've learnt how to add query strings to a httpredirect with reverse(). I am now passing status code and message to the listing view when a bid is placed. The status message is then displayed in the template. I have moved validation of the bid value to the django view so that I can show this functionality. I've also tweaked the listing view, specifically how it determines the whether a user has a listing on their wathlist. For this I learnt about this .exist() extention on a django query. I also refactored the html a bit on the listing page.

### R1D31 - 20200901
Working on commerce project. I've updated some silly model field names and also learnt that blank=True allows a field to be blank in the amin panel (useful). I also added created_at fields for listins and bids and these are now displayed in the templates. I am working on refactoring the listing template. Accepting bids is also working again. I still need to think of how I want to alert a user if his/her bid was accepted. I am displaying a lot more information about bids on the listing page which is good.

### R1D32 - 20200902
Working on commerce project. Worked on the listing page styling and html refactor. I've cleaned up the template to show the relavent information based on user priveledge, bid status and so on. I've learnt that Django templates ignore html comments. My CSS file is mangled due to changing the structure / layout. What is left is finalizing the CSS / UI and handling notifying a user if their bid has been accepted. I also need to spend some time adding example listings.

### R1D33 - 20200903
Commerce project. Decided to just use an extra page for users to see all the listings they have bid on and the status of their bid. Should probably show the ones that they have won first. Not using any javascript so I'm a bit limited in some ways with how responsive etc my page is. I've realised my django models are a bit messy and again considering if bids should be a child of listing as many to many, or if bids should have a listing as a foreign key (currently have the latter). The way I'm naming related names makes no sense to me, and it results in very hard to read code.

### R1D34 - 20200904
Commerce project. Worked on a bit of the frontend for the listing page and the page showing "your" bids and their status. Created new users and played around a bit. When I have a good enough intenret connection I'll create more listings so that I can do a demo video for hand in. I'm not satisfied with my backend as my models and views are not very pretty, even though it works for the purpose.

### R1D35 - 20200905
Related to the commerce project. I started reading the Django model and query documentation. Might seem a bit late, but having context from problems I've run into thus far makes it more useful in a way. I got some tips on good convention with laying out one's models. I want to read further on this and then clean up my models and views. 
