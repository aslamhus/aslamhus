### Hi, I'm Aslam 👋🏽


- 🧑‍💻 Full Stack Developer
- 📷 Photographer
- 🎭 A long time ago, in a galaxy far far away, an actor 

I am proficient in PHP, JavaScript, HTML, CSS, MYSQL and React with experience in front end development, system administration, database management and small API construction. Over 15 years, I have built many websites both from scratch and with popular platforms like Wix, Squarespace and Wordpress.

## A little about me

After I developed a chronic pain condition, myofascial pain syndrome, I left the arts and redirected all my resources into the tech world 💻. When I am able, I still take the occasional photograph ➜ [aslamhusainphotography.com](https://aslamhusainphotography.com).

Programming is a passion (code is poetry!). I love writing **vanilla JavaScript**, as well as the functional programming paradigm of **React**, but also the OOP discipline of writing **PHP** classes. As a self taught developer, I am always keen to learn more, particularly about lower level languages and **Data Structures and Algorithms**.

My first foray into coding was in the 1990s with Macromedia's **Director** (the prehistoric Flash). When I was 10 years old, I learned to program basic RPGs with action script and since then I've never stopped learning. 


## Things I've built recently


### Video Editor
I built a vanilla JavaScript video editor interface that can handle trimming and cropping videos in browser. While the editor doesn't perform any video manipulation by itself, it exports an object with user edits that can be sent to a backend service. I welcome contributions. If you are interested in contributing, please check out the repo and read the readme/contributing files.

Repo: [https://github.com/aslamhus/](https://github.com/aslamhus/VideoEditor)
Demo: [https://aslamhusain.com/video-editor/]

### Bandcamp Player

I built a Wordpress plugin / custom block using React and PHP that displays artists' 15 most recent albums and allows them to be played in the browser. The player looks best on desktop  or laptop screens. I used Spotify's UI as inspiration. Eventually, I'd like to make this plugin publicly available / licensable. 

Demo: [https://coryweeds.com/music](https://coryweeds.com/music/)

### Spotify API Client 
I built a Spotify API library in PHP to query the Spotify database, build playlists and get user data. It offers multiple options for authentication – managing user permissions, server-to-server use cases and refresh tokens. Other features include an ORM design for entities like Artists, Albums, Tracks and Playlists. 

Repo: [https://github.com/aslamhus/Spotify](https://github.com/aslamhus/Spotify)

### GoogleDriveUploader Library
For a project that required archiving and uploading large audio files to a client's Google Drive account, I built a PHP Library that peforms basic uploads for small files and resumable uploads for large files, in this case over 300MB, with the Google Drive API v3.0. I enjoyed the many challenges of building this library such as using generator functions to allow for asynchronous uploads, providing an abort/cancel upload feature, and implementing a resumable upload feature that uploads the file in chunks. This library is publicly available to install via composer `aslamhus/google-drive-uploader`. I have provided extensive documentation about the set up which requires creating a service account on Google Cloud Console to handle authentication.

Repo: [https://github.com/aslamhus/GoogleDriveUploader](https://github.com/aslamhus/GoogleDriveUploader) 

### Wordpress Theme Development Environment package (with hot module replacement)

I built a composer package `aslamhus/wordpress-hmr` which streamlines WordPress theme development by integrating Webpack and HMR (Hot Module Replacement) for real-time updates during development. It provides a simplified asset management system through a configurable assets.json file, enhancing developer efficiency and enabling modern frontend practices within the WordPress ecosystem.

Repo: [https://github.com/aslamhus/WordpressHMR](https://github.com/aslamhus/WordpressHMR)

### Rectangle Packer algorithm
For a project I'm currently working on I need to stitch multiple videos together on the server to create the illusion of multiple videos playing simultaneously. Playing 10+ simultaneously is not a viable option for the browser. However, stiching the videos together as a single video provides a workaround for browser constraints. But stiching the videos together into a grid on the server posed the following problem,  "how do I fit a variable number of videos into dynamic screen sizes while maximizing the space used?" The videos' aspect ratio is known, but the grid dimensions and screen size are not. This is a NP-hard math problem, known as the *Rectangle packing problem*. I wrote my own heuristic algorithm that finds a best fit by starting with a best guess for the size of each video and then incrementing or decrementing the size until certain optimal constraints are met. 

The second problem was to handle looping of the videos. Each individual video in the grid loops, so the grid video must loop as well. The hitch is that the videos have variable lengths. After much research, I used the Euclidean lowest common denominator with prime factorization in order to determine the shortest length the grid video would have to be in order to accommodate all the loops of the videos. 

I wrote a PHP Library to solve these problems and stitch the videos together on the server using FFMPEG.

You can find the source code for a ```JavaScript``` and ```PHP``` implementation of the algorithm in the Repo. 
I also made a web application to test and analyse the algorithm which you can play around iwth.

Repo: [https://github.com/aslamhus/RectanglePacker/](https://github.com/aslamhus/RectanglePacker/). 

Example: [https://aslamhus.github.io/RectanglePacker/example](https://aslamhus.github.io/RectanglePacker/example/)

### PHP QueryBuilder, Database and Search Classes

I wrote my own Database, Search and Query Builder classes, focusing on a fluent design that enables method chaining to facilitate MYSQL queries.  I tried to balance flexibiltiy with complexity, leaving room to scale the classes for more sophisticated queries, while also avoiding unnecessary bloat that sometimes accompanies larger libraries. I chose PDO as the database interface layer. The higher level Search Class allows me to perform both FULLTEXT match...against searches and searches that leverage the LIKE operator with wildcards. I enjoyed writing with the fluent design pattern because it makes the code both readable and flexible. 

### Simple Log Class

For some of the more complex automations for clients, I am relying more and more on logging to maintain, watch and debug these systems. Though for production APIs I use the excellent library Monolog, I built a lightweight PHP Log class for my own projects with features for writing, searching, clearing, and overwriting log entries. 

### React piano keyboard
For a Jazz Radio station I built a simple piano keyboard with playable keys. 

Demo: [https://straightnochaser.ca](https://straightnochaser.ca)

### React Table Component
I built my own Table component that handles operations like sorting, filtering, pagination and select and deleting rows. A particular challenge was to create an efficient pagination system for result sets with 10s or 100s of pages.

### DevOps - Backup applet
Most recently, I used **Linux/Applescript** to build an applet that automates the backup of all the websites on my server. A cron job runs the app every month. It shows a progress bar that keeps me apprised of the backup status/progress (archiving directories, rsyncing, etc). Each backup/snapshot is organised by date and time, and I can customise the needs for each site with a .backupignore file. It also sends me an email report if the backup fails or is successful every month. 

### My first NPM package!
I use the File API a fair bit, so I decided to create a library/package I could reuse that selects, reads, and previews files. 

Check it out here: [@aslamhus/fileselect](https://github.com/aslamhus/fileselect)

## Languages and frameworks I use

- PHP
- Javascript
- React
- Webpack
- HTML
- CSS
- Linux
- Jquery
- MYSQL
- Node

## Passing familiarity with...

- Swift
- Java
- Applescript


## Skills I want to learn

- C++
- Tensor Flow

## Other Skills

- Photography
- Graphic Design / Retouching (Adobe Photoshop / Adobe Lightroom)
- Video Editing (Final Cut Pro X)
- Writing (playwright/poet)

## Some of my recent web design work

[Cory Weeds](https://coryweeds.com)
A website for one of Canada's leading Jazz musicians. Built with Wordpress. This website has several custom plugins, including a bandcamp plugin that displays all the artists available music in a custom music player. 

[Duende Management](https://www.duendemanagement.com)
A UK based Talent agency. Built with Wix. I loved using Wix's javascript framework **Velo** to create an automated display of all the agency's actors. The client is able to update photos, description and stats for each actor without having to touch the design. 

[Kate Novak](https://katenovak.co.uk/)
A UK based voice over artist. Built with Wordpress. I loved creating two different custom audio players using HTML5 and javascript.


<!--
**aslamhus/aslamhus** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
