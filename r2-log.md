# #100DaysOfCode Log - Round 2 - Anja Thiart
The log of my #100DaysOfCode challenge. Started on 16 November 2020

## Initial goal
- Finish LinguiLearn / LinguiLibrary project (final project for CS50 Web 2020
- Create a business website for a small business I know
- Venture into Tensor Flow / ML with Python

## Log

### R2D10 2010-11-25
Shopping Cart REST API. Spent time with the initial setup of a NodeJS Koa server. Server runs, requests hit but miss my 'ping' endpoint... 

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

