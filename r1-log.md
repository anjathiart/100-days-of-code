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

### R1D36 - 20200906
Commerce project is messy now. I have refactored my models and also rethought my related names. It makes more sense now when I do backward relationship queries. So even though I have broken everything, I'm understanding a bit better. I'm playing around and tweaking and it is taking long but I want to understand and it is engaging for now.

### R1D37 - 20200907
Commerce project. Not messy anymore. It took less time than I thought to implement my model changes. Eveything is working well again now. What is left is adding listings data for demonstration purposes and final testing and style polising.

### R1D38 - 20200908
Commerce project. Polished a few things like displaying messages on pages where there is no data available (like a category wihtout listings). Realised that bids and comments should propably not be manyToMany fields inside the listing model. Because, they are tied to one unique listing, and thus should rather be foreignKey relationships. So even though I thought I was doing good to refactor my models before, I was wrong. I added a lot of listing data via the admin panel. I then tried adding one via the 'create_new' page, and there are some bugs. The urls are not being captured properly by the form. I will look into this next.

### R1D39 - 20200909
Commerce project. Found my "bug". I just wasn't assigning the imageUrl a value when creating the model instance. Oops. I've added some simple built in front end validation. I also added some backend logic for empty comments. Added a few comments to the code. Fixed some style issues. Now I'm ready to do the demo and get to the next project.

### R1D40 - 20200910
CS50W Module Javascript. A few things that I learnt:
- dataset property of an element. For example data-color="green" can be accessed via element.dataset.color.
- submit inputs have a disabled property.
- Event listener DOMContentLoaded... I have always used document.onload(...)
- toFix(decimal) to round a float to 'decimal' decimal places (instead of Math.round(...) etc.

### R1D41 - 20200911
CS50W Module User interfaces. This was a good overview of DOM events and dom manipulation. I've always avoided CSS animations; I should really try incorporate it into the next few projects. To me it just isn't necessary and over the top, but the example he showed of show / hiding posts and using animations to improve the user experience was cool. So I want to get to a point where I feel comfortable with animations (and CSS Grid for that matter) as I do now with flexbox. React (via cdn) was also touched on. It's nice to have a simple introduction to how it fits in on a low level, and also I guess now I have seen JSX. 

Even though not required, I will make an effort to include in my following projects:
- Some animations that have purpose other than looking cool
- React where it makes sense

### R1D42 - 20200912
CS50W Commerce project. Polished a bit and fixed some bugs with unauthenticated users and views / pages / template tweaks for them. Did the screen recording of the project. 
- Video link: https://youtu.be/71YrEOlvQRU
- Repo linke: https://github.com/anjathiart/commerce

### R1D43 - 20200913
Started CS50W 2020 Project 3: Mail. *Design a front-end for an email client that makes API calls to send and receive emails.*
I familiarised myself with the app structure and started working on the compose new mail logic. I was losing my log data in dev-tools when ever the page reload was triggered. This might be trivial but it's good to know I can change the settings for the dev-console to 'preserve-log'.

### R1D44 - 20200914
Mail Project. I struggled a bit to get the React JSX script working but eventually found a way and am now rendering react components on my page. Email cards are rendered to show the list of emails in each mailbox. Learnt that JSX uses 'className' instead of 'class' - but the warnings / error reporting in the dev-console is really very specific which helps.

### R1D45 - 20200915
Mail Project. I created another react component for reading an email. I also attached some logic to archive and un-archive emails and it all works quite nicely once it's set up. Need to do some DOM cleanup though and am thinking of the "clean" way to keep track of the 'ReactDOM'. I'm using JSX which is different to Vue SFC's that I'm used to. 

### R1D46 - 20200916
Mail Project. Added some state and methods to the read-mail component and implemented the reply UI and functionality. All styling still to be done.
- Life is much easier with the sublime 'Babel' and 'Babel-snippets' package for babel react JSX syntax highlighting
- Was reminded of `white-space: pre-wrap;` for conserving line breaks etc
- Learnt that to comment within React code-stuff that comments must be wrapped in curly braces as well: `{ // comment }`
- Added some onClick handlers within the React components to trigger methods previously fired with document.eventlisteners.

### R1D47 - 20200917
Mail Project. Went over all the requirements step by step tweaking where necessary.
Learnt:
- How to conditionally render an element wihtin the React render function. Basically wherever you want to use JS just use curly braces and treat html as 'deconstructed' variables
- Had an issue passing a function to an eventlistener. Bugs came up because this function I passed in can take an optional argument:
`document.querySelector('#compose').addEventListener('click', () => compose_email());`
vs
	`document.querySelector('#sendMail').addEventListener('click', send_email);`
... So good idea to read up on functional programming and how this workds under the hood

### R1D48 - 20200918
Mail Project. Spent over 2 hours displaying and animating a simple message based on a response. Not using async/await, so using timeout fumctions to time animations / next function execution etc. Not used to it and sat and fiddled for such a long time. ALso keeping up with which elements to show / hide based on x, y, z is dirty. Should just learn  how React components can be animated outright, but doing it with vanilla first.; have avoided animations (in general) for long.

### R1D49 - 20200919
Mail Project. Polishing, styling tweaks and code clean up. Next I need to add some accounts to generate some email content etc.

### R1D50 - 20200920
Watched CS50 Web 2020 lecture on Testing and CI/CD. Unit testing functions, server request / responses, models and also front end in-browser testing. Learnt a bit about github actions.
- Would like to know how to use github actions where one repo is dependent on another repo
 Also short intro to Docker. Not sure how I will use all of this in final project. CD - continuous delivery and / or continuous deployment.
 
### R1D51 - 20200921
Finished Mail project. Recorded screen cast and submitted
- Link to demo video: https://youtu.be/B9a-E1Lf67s
- Link to repo: https://github.com/anjathiart/mail

### R1D52 - 20200922
Started the final module and covered the first half: Scalability. Nice to have a simplified overview of it. Loadbalancing, multiple servers, database splitting and database replication, and caching (client and / or server side). Also started brainstorming my final project idea: An english vocab builder app (inspired by the vocab builder on my Kindle). Pitty Kindle does not have an API, so won't be able to pull existing data from that.

### R1D53 - 20200923
Finishing final lecture, part 2: Security.
- How does public-private key encryption work? It is explained at a high level but not in detail.
- GIT: always destroy commits where credentials / sensitive info were exposed accidentally
- Learn more about environment variables and how to use them for secrets / keys / etc
- Cross-site request forgery: django csrf token takes care of this

Started setting up and looking at CS50W 2020 Project 4: Network

### R1D54 - 20200924
Network project. Started setting up my models / url and view structure. Successfully loading posts through the api routes into frontent via JS.

### R1D55 - 20200925
Network project. Updated models. Added api endpoint to fetch current user in the jsx. Converted posts and post list to react components and added jsx for rendering it. 

### R1D56 - 20200926
Network project. I learnt how to pass arguments etc to 'event handler functions' within the REACT render function. Had to include the jsCookies module CDN to get / pass the csrf token to and forth.

### R1D57 - 20200927
Network project. Worked on JS and views for connecting like / unlike to api and loading a user's profile and posts for that user. Spent a lot of time thinking and going back and forth with how best to design the api calls. How to separate concerns, and what to separate or what to combine.

### R1D58 - 20200928
Network project. Frustrating session. Spent a long time fixing a bug in all the wrong places. Only later realised that I had a bad reference in a manytomany field within the User model. Instead of ...manyToManyField(self..) I should have used ...manyToManyField("User"...). Good reminder not to glimpse over stackoverflow answers without understanding the exact context / relevance of the question first. I also battled with filtering on manyToMany fields, and in the end it was really simple, indicating that I'm not grasping the concepts 100%.

### R1D59 - 20200929
Network project. Much better session. Implemented capability to edit your post with checks for user scope and backend validation. Getting the hang of the react render and how to do two-way binding. Am using `value={ x }` and `onChange={ e => x = e.target.value }` vibes. Didn't search long but didn't see a `v-model` equivilant.

### R1D60 - 20200930
Network project. Fixed some DOM logic and implemented the view for seeing posts of users one follows. Keeping track of some state as global variables (for example the heading based on the current view. Keen to see how routing and state is managed when using a vue-cli-type react cli. I want to split the posts endpoints up further and not use query params to determine what to serve because the query params currently cannot be processed concurrently (separation of concerns).

### R1D61 - 20201001
Network project. I refactored the posts endpoints based on R1D60's comments. Added logic for posting a new post (was doing it via admin panel before). I also fixed the way I get all the posts for users the current user followed using a single query to ensure chronological ordering. Need to test the api for routes being hit when user is logged in or not, implement pagination and then styling.

### R1D62 - 20201002
Network project. Just working on styling right now. Using SASS and the bootstrap defaults that came with the project start files. Think I should go look at the bootstrap offerings and try change things up a bit. Getting tired of the same btn btn-primary button on all my projects.

### R1D63 - 20201003
Network project. Still working on UI/UX. Using a bit more of bootstrap utilities. But I find once you start with bootstrap the color scheme seems constraining. Also, couldn't find box-shadow utilities for it. So used this link for my cards: https://codemyui.com/awesome-box-shadow-effect-for-card-ui/. Need to still style the user profile section and then polish UI and add pagination, and write some tests to check the api scope is adhered to.

### R1D64 - 20201004
Network project. Implemented pagination on the back end using Django Paginator class. Busy implementing it in the UI. Learnt that you can use IIF's inside the React render function to loop and so keep the `this` binding for event handlers that call react component methods. 

### R1D65 - 20201005
Network project. Have used a combination of bootstrap 4 and django Paginator class to implement pagination as a React component. It is done. Also spent some time on further styling. I've learnt that customizing bootsrap theme colors requires installing it as a package and then using the SASS functionality it gives, so for now I'm just using their colours and overriding manually where I need.

### R1D66 - 20201006
Network project. Writing unit tests. I've created one simple test to check that unauthorised actions can't be performed when editing posts.
Learnt how to:
- setup the test file and write a basic test
- create post / put requests and using `json.dumps(...)` to create the request data
- simulate a logged in user and the request user
- simulate an anonymous user
- use `pip install nose pinocchio django_nose` with some extra settings in settings.py for nice test output
Really seeing the value of unit tests, as already found some hidden bugs.

### R1D67 - 20201007
Network Project. Spent some time today dealing with authentication vs forbidden etc. I've created a fetch wrapper function that intercepts the response and deals with error codes. All 401's get redirected to login. Django's `login_required` decorator was being buggy in that it returns 200 that redirect happened but the javascript code continues. Instead I am handling these cases differently. Which probably makes sense since these are api endpoints more than page views? Not sure. Next I must handle the other errors by possibly just mounting a 'alert' component in the view.

### R1D68 - 20201008
Network project. Busy implementing the front end error message modal for request errors. 

### R1D69 - 20201009
Network project. Worked on polishing and styling.

### R1D70 - 20201010
Network project. Had issues with my error handling with a form element that was handled using fetch in the JS. Removed the form tag and now it behaves accordingly. I'm getting a strange error with React ` TypeError: Failed to fetch` even though the page works fine and behaves as expected. Leaving for now. I have some spaghetti in the JS, not as ETC and Orthognal as I'd like it to be. Next is writing unit tests and then on to next project where I will put more thought into the structure of my views and functions.

### R1D71 - 20201011
Network project. Wrote some more unit tests to check api-endpoints which require authentication and ironed out some small things. 

### R1D72 - 20201012
Lingui learn app. Started playing with the worknik and oxford dictionaries api's. Preferring Oxford for now. But will use randomWord endpoint from wordnik. At a loss of where to start as I don't just want to jump in. But I setup the django-app structure so long.

### R1D73 - 20201013
Lingui Learn app. Setup some initial urls, views, templates and models. Had to fiddle with the settings file a bit. Realised today there is a button in sublime to convert spaced-indents to tabbed-indents (haha). 

### R1D74 - 20201014
Network project. Sorted out some last minute bugs. And submitted code and video for this project.
- demo video: https://www.youtube.com/watch?v=P_QSEHIOCck
- repo: https://github.com/anjathiart/network

### R1D75 - 20201015
Linguilearn. Playing with the django-frienship package to manage friend requests etc.
https://github.com/revsys/django-friendship
Learning about better exception handling and use of the ctx object. So far I've hooked up adding a friend by username. 

### R1D75 - 20201016
Liguilearn. Added more endpoints. Realizing that instead of writing js to test these I should just write unittests outright and not pollute my app. Struggling to get js modules in browser without webpack working. I'm sure it is possible. Trying solutions on the web but not succeeding.

### R1D76 - 20201017
Linguilearn. Wrote unittests for sending / cancelling friend requests. Using `nose` for nice logging.
Still learning:
- Flag `-s` allows for displaying print statements using `Nose`
- Seems like db updates done within one test does not get preserved in further tests.
- how to use `assertContains` with JSONresponses. `assertIn` is fuzzy.
- The json response string is accessed via `response.content`

### R1D77 - 20201018
Linguilearn. Refactoting my views into a module structure with view files for auth, frienship etc. (routes so to speak). Learnt that I have to make use of this `__init__.py` file within the views folder to achieve this. Also learnt that in python / django package structure one you use `.`'s to show directory level. So, `.` or `..` (two up). `...` (three up). Added the accept friend view and unit test. Overiding django.shortcuts `get_object_or_404()` method used in the official django-friendship package as I don't want to deal with raised Http errors. Rather pass it via ctx and status.

### R1D78 - 20201019
Linguilearn. Adding more views and unit tests. 

### R1D79 - 20201020
LinguiLearn. Learnt:
- how to implement my own decorator function that checks for user authentication before processing request, and how to keep it in a separate module.
- That the django object_or_404() method is unneccessary and just using try, catch instead so that can add custom status messages
- how to use the django require_http_methods decorator to deal with 405 errors instead of repeating same check on every view

### R1D80 - 20201021
Linguilearn. Successfully hooked up the oxford dictionaries API to search for words (if they are 'head words')

### R1D81 - 20201022
Linguilearn. Implemented extra layer to first hit oxford 'lemma' endpoint to find the head word of a word (for example if user types in a plural) before getting the word information. Looks like the free version of the API does not allow to look up sentence examples which is a let down. I now have functions that sit on a layer above the url endpoints in my api - so must decide how to structure it into modules.

### R1D82 - 20201023
Spent time setting up my dev environment again. Reading up on django model managers and custom model methods as I want to separate business logic out of the api layer. Read about services as a layer in between the api and the models. But I'm going to try make use of custom managers and querysets_as_managers. But I think this is the main thing that I was looking for:
`Define custom methods on a model to add custom “row-level” functionality to your objects. Whereas Manager methods are intended to do “table-wide” things, model methods should act on a particular model instance.

This is a valuable technique for keeping business logic in one place – the model.`

### R1D83 - 20201025
Linguilearn. Updated the word_search endpoint to have an extra step where the word is first looked for in the DB before hitting the Oxford API, and then saving it to the DB if a valid match is found. Also added a route for a user to add a word to their list. And added more unit tests.

### R1D84 - 20201026
Linguilearn. Renamed some routes and models. Decided to append all api views with 'api/'. Added more endpoints for users managing their entries. Busy implementing much of this as model methods. Have not needed to implement managers yet. Wrote some unit tests. Next I want to write some exceptions to use in the models for error handling in the views.

### R1D85 - 20201027
Linguilearn. Defactored the oxford api calls into one function to simplify return values. Added custom exceptions to use in my models. Simplified and cleaned up code in the models and views. Still unsure if I'm breaking good practice by referencing another model type in a model method, instead of using a custom manager on the model. But since this is a 'per-row' method, I don't want to use a manager (?)

### R1D86 - 20201028
Linguilearn. Hooked up a cool api "Words API". It gives a lot more detail on the free version, and one can hit the examples / definition / etc endpoints. I am still needing to use the oxford dict api to get the "base" word / "head" word in case of derived words being searched for by the user. Then I can send the word to the words api to get examples and definitions. The challenge now is that the result list returned by words api can be a long list, and the order is not necessarily from most relevant / literal to least. So I need to determine how I present the results to the user, and also how I represent the examples. It's also a lot to store in a local db if I don't want to always query the api services when a user reflects on saved words. But even if they choose the definition that suits their context best when the results is first presented, it would require models to store definitions, models to store examples, with links to determine which are linked to which, and then how to keep track of which user chose which definition / example for which word search. So for now I will just query the api everytime a user revisits a word. For this app use case.

### R1D87 - 20201029
Linguilearn. I decided I may want to design my models differently. Left Entry model as is and created a Word model with the word and also manyToMany fields with learning, mastered, and liked users respectively.

Learnt how to:
- Create a manager for my model to do some of the reworking for me and keep the views clean
- Run a single test case within a test file `./manage.py test myapp.MyTestCase.test_something`

### R1D88 - 20201030
Linguilearn. Added a route for searching for users based on email or username. Then moved to front end to implement searching for a user so that one can send friend requests. Restructured my secureFetch fn to return the parsed result object directly. Also playing with async/await and getting more comfortable with awaiting promises. Unlike previous projects where I call the next function within the .then() call, I am decoupling it so that the result is captured in a variable and the next step / fn is called outside the .then().catch() statements. I think this will be much cleaner, as before I had this long chain of dependency from one funtion, calling the next function within itself, then within the next calling the render function to populate the DOM.

### R1D89 - 20201031
Linguilearn. Working on the front end. Had to tweak my secureFetch / promise function to add async / await when resolving json(). For some reason I need async / await for rejecting `reject( await response.json())` but didn't need to do this for resolve(). All this means is I don't fully understand under the hood. As I'm working on my front end logic, I realise I need a lot more information about the users search result. If I want to conditionally show add / cancel / remove / etc wrt friendship requests, I need access to a lot more data in the response body.

### R1D90 - 20201102
Linguilearn. You think you have something but then you realise far from it! But I worked a bit on the back end again. Realised I don't want to have such a full on friendship request / search / etc thing on the front end. This is more about the words and learning. So I'm going to change it that you just enter a friends email to invite them, and then let the response message deal with the cases of "already a friend", "request already sent", and so on. I will have to write further functions to calculate if a friend request was accepted or not and then filter that out of the resulting requests lists, in order to display the correct information on the user profile / notification section. Fun times.

### R1D91 - 20201103
Linguilearn. Decided that the users/friends endpoint will only return pending friendship requests and current friends of the user. Also decided that adding a friend is by entering an email and letting the backend response be shown as a success or error popup (for now). Keep changing things around. meh.

### R1D92 - 20201104
Linguilearn. Played around more with my endpoints for 1) getting the current user and 2) getting a user's profile information. Realising I need to design (wireframe / story board) the UI/UX properly as my api calls keep changing based on how I keep changing how I want the front end to look / function like. Realising the importance of this now, even for a small app like this!

### R1D93 - 20201106
Linguilearn. Today was one of those 'aha' days. Refactoring my jsx to have one `ReactDom.render()` call to mount the whole front end. Similar to what we do in Vue at work. It is confusing since I'm writing all the code in a jsx script and not using singe file components, a store, router, ES6 module imports or webpack. This might get tricky down the line as the main view / pageView changes. And then I might have to have more than one render()'s. But I don't think so. What is not so great is that I will potentially be passing values up multiple level of parent-child components. Which might mean that I should at least, for now, render the error / msg modals outside the main #app. Learningn react this way, only using JSX, is making me understand a lot more about how things work, even though I still have some 'magic' happening (where things work but I'm just following documentation exmaples...). 

### R1D94 - 20201107
Linguilearn. Following from yesterday, have now separated all non `<App />` components into separate file, and util functions into its own file. Feels backwards doing this and not using module imports, but that is ok. Added some layout classes with layout debug styling to see how it all fits. 

### R1D95 - 20201108
Linguilearn. Took a step back from coding and spent time brainstorming / building on my ideas and then formalising the best model structure that would serve this. It might have got a bit out of control / scope, but I think I pulled it back. Excited to feel a bit more control and forward planning. Having done what I have up to now did help lead to a reshuffle, but it ties in with how I am envisioning my UI/UX. I have not thought of the 'learn game' yet. Doh. But the idea there is to limit the amount of words you can have in your 'learning' column (there will now be options for 'queued', 'mastered', 'learning'). So for example, if the maximum words to be learning is 20, then the 'learning game' won't end up flashing 1000 words+ at you at random. I've come up with a nice table structure that also allows for much more user specific data entry for a particular word with personalised choices of definition / example, and also allows other fields for reference.  

### R1D96 - 20201110
Research / proposals. No coding but busy putting together a spec with a friend with a small business to create a web presence for him. This will force me to learn a CMS framework and live deploy etc, which I have no experience with and been looking for a good opportunity to learn and get real-world experience.

Also, this: Optional chaining and null coalescence coming in ES2020:
```js
let familyTree = {
    us: {
        children: {}
    }
}

// with _.get
const grandChildren = _.get(familyTree, 'us.children.theirChildren', 'got no kids' );

//with optional chaining and null coalescing 
const nullCoalescing = familyTree?.us?.children?.theirChildren ?? 'got no kids'
console.log(nullCoalescing) //got no kids
```
https://www.freecodecamp.org/news/javascript-optional-chaining-explained/#:~:text=Optional%20chaining%2C%20represented%20by%20%3F.,of%20object%20properties%20in%20JavaScript.

### R1D97 - 20201112
Did some reading in `The Pragmatic Programmer`. Some highlights of the hour:
- Which units to use when COMMUNICATING an estimated time that something may take (1-15 day? user days, 16-30 days? user weeks, ... and so on).
- Customizing your shell (if it's going to be your home for a while, might as well make it comfortable) -> aliases, wrappers etc,
- LEARN YOUR EDITOR CAPABILITIES
	- Try spending 2 - 5 days coding in your editor(s) without touching the trackpad / mouse (except maybe when having to google how to do something without it)
	- Pause when you realise you are doing something repeatedly and find out if you editor has a shortcut for this, and if it doesn't find a (good) plugin.
- TRACER BULLET approach vs Prototyping (pros cons and when to use which)

The last point is actually the one that I needed to learn today. I've slowed down in my project because I want to do it all at once, but I don't want it to end up being an prototype that I recode anyway (...because prototypes are meant to be discarded). So I'm going to try use this Tracer bullet approach to get myself back on track with Linguilearn. More details in The Pragmatic Programmer. I understand it as taking one feature / story / functionality, and implement it from UI -> API -> Logic -> Models -> Database, in a  way that it is usable, deployable, functional. And if it does not hit the 'target', you have one 'line' to trace back. 

### R1D98 - 20201113
Linguilearn. Yesterday's reading paid off. I plucked out Trello, wrote some stories, organized each story into UI, API, Models, Tests, and listed the tasks to complete that story. And so quickly tracer bullet trajectories became clear, and refactoring a story to make it more explicit (adjusting the target?), and so I chose the main story of "User wants to lookup a word of interest".
So just by trying out this stragegy, I feel a lot less overwhelmed, have a cleared understanding of the 'WHAT', and the how is emerging. I have my word search UI component, and next must link it to the api call (which I have already written and done some tests on)
Also made use of https://colorhunt.co/palette/118962 for some quick colour schemes (temporary)

### R1D99 - 20201114
Linguilearn. Moving forward with yesterday's momentum. My api endpoints for searching and serving details is working. The UI shell is there for this component, but I havent made the `InputText` component reactive yet.
Did a lot of refactoring and added an extra section to my tracer-bullet-style-trello-story-card, calling the `checklist` "sprouted questions" for now, to keep track of things I must consider / keep in mind / research / address... later, or in a different card. For now focusing on one trace.

### R1D100 - 20201115
Linguilearn. Search / View word. I have made the components reactive. Users can now search for a word and the results are displayed in a list. I am slowlyy understanding better how to use the render() function to add variables, run some loops, etc, and why / how. But just by trial and error. I'm in a good flow and things are coming together nicely. TRACER BULLETS ARE MY NEW BEST FRIEND.
