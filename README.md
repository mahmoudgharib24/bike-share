# bike-share
my first repository on github 
# My-Udacity-Bikeshare-Project
## Introduction
This Python script is written for Project 2 (Term 1) of Udacity's Programming for Data Science Nanodegree Program and is used to explore data related to bike share systems for Chicago, New York City, and Washington. It imports data from csv files and compute descriptive statistics from the data. It also takes in users' raw input to create an interactive experience in the terminal to present these statistics.

## Dataset
The datasets used for this script contain bike share data for the first six months of 2017. Some data wrangling has been performed by Udacity's staff before being provided to the students of Data Science Nanodegree Program 
To install grip, simply:

$ pip install grip
On OS X, you can also install with Homebrew:

$ brew install grip
Usage
To render the readme of a repository:

$ cd myrepo
$ grip
 * Running on http://localhost:6419/
Now open a browser and visit http://localhost:6419. Or run with -b and Grip will open a new browser tab for you.

You can also specify a port:

$ grip 80
 * Running on http://localhost:80/
Or an explicit file:

$ grip AUTHORS.md
 * Running on http://localhost:6419/
Alternatively, you could just run grip and visit localhost:6419/AUTHORS.md since grip supports relative URLs.

You can combine the previous examples. Or specify a hostname instead of a port. Or provide both.

$ grip AUTHORS.md 80
 * Running on http://localhost:80/
$ grip CHANGES.md 0.0.0.0
 * Running on http://0.0.0.0:6419/
$ grip . 0.0.0.0:80
 * Running on http://0.0.0.0:80/
You can even bypass the server and export to a single HTML file, with all the styles and assets inlined:

$ grip --export
Exporting to README.html
Control the output name with the second argument:

$ grip README.md --export index.html
Exporting to index.html
If you're exporting a bunch of files, you can prevent styles from being inlining to save space with --no-inline:

$ grip README.md --export --no-inline introduction.html
Exporting to introduction.html
Reading and writing from stdin and stdout is also supported, allowing you to use Grip with other programs:

$ cat README.md | grip -
 * Running on http://localhost:6419/
$ grip AUTHORS.md --export - | bcat
$ cat README.md | grip --export - | less
This allows you to quickly test how things look by entering Markdown directly in your terminal:

$ grip -
Hello **world**!
^D
 * Running on http://localhost:6419/
Note: ^D means Ctrl+D, which works on Linux and OS X. On Windows you'll have to use Ctrl+Z.

Rendering as user-content like comments and issues is also supported, with an optional repository context for linking to issues:

$ grip --user-content --context=joeyespo/grip
 * Running on http://localhost:6419/
For more details and additional options, see the help:

$ grip -h
Access
Grip strives to be as close to GitHub as possible. To accomplish this, grip uses GitHub's Markdown API so that changes to their rendering engine are reflected immediately without requiring you to upgrade grip. However, because of this you may hit the API's hourly rate limit. If this happens, grip offers a way to access the API using your credentials to unlock a much higher rate limit.

$ grip --user <your-username> --pass <your-password>
Or use a personal access token with an empty scope (note that a token is required if your GitHub account is set up with two-factor authentication):

$ grip --pass <token>
