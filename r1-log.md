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
