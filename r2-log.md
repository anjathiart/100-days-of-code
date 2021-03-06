# #100DaysOfCode Log - Round 2 - Anja Thiart
The log of my #100DaysOfCode challenge. Started on 16 November 2020

## Initial goal
- Finish LinguiLearn / LinguiLibrary project (final project for CS50 Web 2020
- Create a business website for a small business I know
- write a REST api for a shopping cart application
- Venture into Tensor Flow / ML with Python

## Log

### R1D28 2020-12-15
Wordpress website. Started getting familiar with wordpress. Realized its best to use the 2020 wordpress theme so that I can customize more of the style components (fonts etc). Registered the wordpress domain for the small business i'm doing this for. Using free version for now. Will port to local hosting with a ISP once I've finished the first draft.


### R1D27 2020-12-14
Linguilearn. Made the screen recording... but it was 3 minutes overtime. So I learnt how to use an online tool to cut out some of the content, and now I'm busy speeding it up to be just under 5mins. 

Here is the link:
REPO: https://github.com/anjathiart/lingui-learn
Video: https://youtu.be/B5PbrYoQnUA

### R1D26 2020-12-13
Liinguilearn. Redid my readme file adding more information and background for the project submission. Recorded almost 4 screencasts just to realize the microphone was switched off. 

### R1D25 2020-12-12
Linguilearn. Worked on responsive layout and wrote some tests. Also did the initial write up.

### R1D24 2020-12-11
Linguilearn. Added loading page while word info is searched for. Notes can now be written in markdown. Entries can be edited in the page. Improved flow and some responsive stuff as well.

### R1D23 2020-12-10
Linguilearn. Went back to the KanBan bourd to pen all the little loose ends that are outstanding. Implemented ordering and random shuffle on library model / endpoints and added it in on the UI. Front and back end needs to be linked now.

### R1D22 2020-12-09
Linguilearn. Styling, styling, feather icons, styling.

### R1D21 2020-12-08
LinguiLearn. Refactored react components. But now it seems I have too much functionality in the main app component...

### R1D20 2020-12-07
Linguilearn. Added in pagination in the api and frontend. I need to iron out some issues though with the page count etc going back to defaults re-mount

### R1D19 2020-12-06
Linguilearn. Worked on responsive Layout. I have a good layout now that changes nicely for different screen sizes. 

### R1D18 2020-12-05
Linguilearn. Spent time on the UI and cleaning up the layout, structure, and making it responsive. Things are working well on small screens now. Mixture of my own css and bootsrap.

### R1D17 2020-12-03
Linguilearn. Worked at improving the UI by adding an endpoint to fetch 1 detailed entry when clicking on a library entry (which's endpoint now returns less information for each entry. Also fixed a bug or two.

### R2D16 2020-12-02
Linguilearn. Context switching. I have decided to leave out the django-friendship integration for now, even though I had spent a lot of time with implementing it. The main function of the app is to save cool words to reference and learn and just remember. So that is my MVP. Having the ability to add and follow friends is a feature for v2.

### R2D15 2020-12-01
Shopping cart REST API. Managed to refactor the stocklevel add/remove models to be safer. Had to use normal sql syntax since as I couldn't find a way to to it using node-sql. But that is not more important than an optimized query -- which still does not prevent edge cases but it's better than it was. Also added more endpoints, found some HUGE bugs, and finished up the brief api reference in the readme. Done for now. But I realised I wasn't updating the dates in the db when things are updated. oops.

### R2D14 2020-11-30
Shopping cart REST API. Finalized a table schema for my cart orders. It's not very robust. Kind of cauing issues. But I need to focus on a solution that works. Struggling to get my head around edge cases and the node-sql dialect to achieve certain things in one query instead of 3 (which I'm doing now for reserving / releasing stock). Wrote some unit tests and found some good bugs to fix.

### R2D13 2020-11-29
Shopping cart REST API. Spent a lot of time breaking my head about how to populate my products table with sample data from the web. Ended up writing a few scripts to take sample data and transform it / add to it / convert it to my preferred structure. Then I worked on the GET products route. Have added searching. Still have to add filtering by price, category, inStock and then implement pagination.

### R2D12 2020-11-28
Shoppint cart REST API. Added more endpoints, tests, and middleware. Had to learn how to user Joi because hapi/joi has been deprecated. So there was a lot of debugging and so on. Specifically got basic authentication and authorization working now.

### R2D11 2020-11-27
Shopping cart REST API. Worked on the user register and auth routes, controls and models. Focussing on one route at a time, and once I've done all the middleware and schema definitions and validations for one, the rest should fit into that structure easily.

### R2D10 2020-11-26
Shopping cart Database. Created my initial database design, tables, and table structures. For now I haev a user, item and order table. I will probably add a few more to break down all the info about the item, but I don't want to spend time on focussing on all that and rather focus on the implementation of the customer shop cart "micro-service".

### R2D10 2020-11-25
Shopping Cart REST API. Spent time with the initial setup of a NodeJS Koa server. Server runs, requests hit but miss my 'ping' endpoint... just fixed this by typing the koaRouter .get url in the 'hard' way instead of grabbing it from the config file. 

### R2D9 2020-11-24
Linguilearn. Worked on my endpoints and models. Added Entry Model method to handle entry updates for any number of fields to be changed. Cleaned up some code.

### R2D8 2020-11-23
Linguilearn. Improved backend to save word entry details retrieved from external services to the word model. It has improved the performance of the app sooo much. User can now also view their library entries.

### R2D7 2020-11-22
Linguilearn. Worked on retreiving and displaying a users library. Using the array map() function with JSX to spit out library entries as cards". Learnt about reacts ComponentDidMount hook and used it.

### R2D6 2020-11-21
Linguilearn. Worked on changing my table structure based on improvement ideas. Testing a lot in the browser (bad). Loads of debugging of models.

### R2D5 2020-11-20
Did reading in The Pragmatic Programmer. Learnt some new concepts about debugging and problem solving. Also different methods of testing like Design By Contract (DBC). Even if not semantically implementable in my code, it is a good thing to know about when writing out function requirements in a way. 

### R2D4 2020-11-19
Linguilearn. Again, debuggin my API in the browser. Would be slightly less bad if I saved search results to local storage so that I wouldn't have to wait for WordAPI requests so long. Must. Write. Tests. Today I spent time on handling UI/UX/API for saving a new entry with details. Understanding the ...spread operator all of a sudden. And also learnt how to update a nested React state object. It feels like having to do things in a certain way to get things to update correctly is more clear using React Classes without all the other add-ons (like Vuex, Vue Router equivilants).

### R2D3 2020-11-18
Linguilearn. Finding myself testing in the browser instead of just writing more tests :(
Added error / warning message display to the UI and fixed related backend bugs. Need to read up more on python ValueErrors, because I'm using them, converting them to ints, and comparing but I don't know how to access the 'object' (is it an object?)
Also working on the next UI view (filling in personalized details for an entry)

### R2D2 - 2020-11-17
Lingilearn. Python. Spent today refactoring and improving my `/word` endpoints and external API functions. Mainly I converted my conditional returns from the external API functions to raise exceptions if there is a problem, and then handling them in the context of the in-house API with `try` and `except` statemnts. Getting comfortable with exception hanlding in Python and seeing the value in it. Much less spaghetti `if-else` statements.

### R2D1 - 2020-11-16
Linguilearn. I'm comfortably using map() with reactjs and understand what it is doing better. Added lots more word details to search results and am displaying it nicely in my component.

