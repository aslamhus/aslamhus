### Hi, I'm Aslam 👋🏽


- 🧑‍💻 Full Stack Developer
- 📷 Photographer
- 🎭 A long time ago, in a galaxy far far away, an actor 
- 🌱 Currently learning websockets/service workers 


I am proficient in PHP, JavaScript, CSS and React and  have experience in Front end development, System Administration, Database management and API construction following RESTFUL principles. I have built many websites from scratch as well as used website builders like Wix, Squarespace and Wordpress.

I was an actor and headshot photographer, but a musculoskeletal disorder changed all that. Now I am redirecting all my resources into my love for technology 💻. I still do photography from time to time, check it out ➜ [aslamhusainphotography.com](https://aslamhusainphotography.com).

I Love writing **vanilla JavaScript**, love the functional programming of **React**, but also the OOP discipline of writing **PHP** classes! I am keen to learn more about lower level languages and improve my knowledge of **Data Structures and Algorithms**.

I've been a self taught web developer for 15 years. My first foray into coding was in the 1990s with Macromedia's Director (the prehistoric Flash) when I was 10 years old. I was building very (VERY) basic, Final Fantasy inspired RPGs, accompanied by similarly rudimentary, but very earnest 3D animations I made with Cinema4D.  I would pass the games out to my friends in grade school via floppydisks 💾. (Thankfully ZipDisk came along in '94 - 100 MB of storage? Revolutionary!). These were simpler times. There was no YouTube, no StackOverflow, and very little documentation available. So progress was... glacial. Now the resources available for learning seem limitless and I am always hungry for more.


## Things I've built recently

### Spotify API Client 
I built a lightweight Spotify API Cliet library in PHP to query the Spotify database, build playlists and get user data. It offers multiple options for authentication – managing user permissions, server-to-server use cases and refresh tokens. Other features include an ORM design for entities like Artists, Albums, Tracks and Playlists. You can find the repo here: [https://github.com/aslamhus/Spotify/blob/main/README.md](https://github.com/aslamhus/Spotify)

### GoogleDriveUploader Library
For a project that required archiving and uploading large audio files to a client's Google Drive account, I built a PHP Library that peforms basic uploads for small files and resumable uploads for large files, in this case over 300MB, with the Google Drive API v3.0. I enjoyed the many challenges of building this library such as using generator functions to allow for asynchronous uploads, providing an abort/cancel upload feature, and implementing a resumable upload feature that uploads the file in chunks. This library is publicly available to install via composer `aslamhus/google-drive-uploader`. I have provided extensive documentation about the set up which requires creating a service account on Google Cloud Console to handle authentication. You can find the repo here: [https://github.com/aslamhus/GoogleDriveUploader](https://github.com/aslamhus/GoogleDriveUploader) 

### Video Editor
I built a vanilla JavaScript video editor interface that can handle trimming and cropping videos in browser. While the editor doesn't perform any video manipulation by itself, it exports an object with user edits that can be sent to a server where these operations can be performed. You can see a working example here: [https://aslamhusain.com/video-editor/](https://aslamhusain.com/video-editor/)

### Rectangle Packer algorithm
For a project I'm currently working on I need to stitch multiple videos together on the server to create the illusion of multiple videos playing simultaneously. Playing 10+ simultaneously is not a viable option for the browser. However, stiching the videos together as a single video provides a workaround for browser constraints. But stiching the videos together into a grid on the server posed the following problem,  "how do I fit a variable number of videos into dynamic screen sizes while maximizing the space used?" The videos' aspect ratio is known, but the grid dimensions and screen size are not. I discovered that this is a NP-hard math problem, known as the *Rectangle packing problem* "where the objective is to determine whether a given set of small rectangles can be placed inside a given large polygon, such that no two small rectangles overlap. Several variants of this problem have been studied." I wrote my own heuristic algorithm that finds a best fit by starting with a best guess for the size of each video and then incrementing or decrementing the size until certain optimal constraints are met. 

The second problem was to handle looping of the videos. Each individual video in the grid loops, so the grid video must loop as well. The hitch is that the videos have variable lengths. After much research, I used the Euclidean lowest common denominator with prime factorization in order to determine the shortest length the grid video would have to be in order to accommodate all the loops of the videos. 

I wrote a series of PHP classes to solve these problems and stitch the videos together on the server using FFMPEG.

### PHP QueryBuilder, Database and Search Classes

I wrote my own Database, Search and Query Builder classes, focusing on a fluent design that enables method chaining to facilitate MYSQL queries.  I tried to balance flexibiltiy with complexity, leaving room to scale the classes for more sophisticated queries, while also avoiding unnecessary bloat that sometimes accompanies larger libraries. I chose PDO as the database interface layer. The higher level Search Class allows me to perform both FULLTEXT match...against searches and searches that leverage the LIKE operator with wildcards. I enjoyed writing with the fluent design pattern because it makes the code both readable and flexible. 

### Simple Log Class

For some of the more complex automations for clients, I am relying more and more on logging to maintain, watch and debug these systems. I built a simple PHP Log class with features for writing, searching, clearing, and overwriting log entries. You can find it here: [https://github.com/aslamhus/Log](https://github.com/aslamhus/Log)


### React piano keyboard
For a Jazz Radio station "coming soon" landing page, I built a simple piano keyboard which is playable with touch or the mouse. See it in action [https://straightnochaser.ca](https://straightnochaser.ca)


### React Table Component
I built my own Table component that handles operations like sorting, filtering, pagination and select and deleting rows. A particular challenge was to create an efficient pagination system for result sets with 10s or 100s of pages.


### Backup applet
Most recently, I used **Linux/Applescript** to build an applet that automates the backup of all the websites on my server. A cron job runs the app every month. It shows a progress bar that keeps me apprised of the backup status/progress (archiving directories, rsyncing, etc). Each backup/snapshot is organised by date and time, and I can customise the needs for each site with a .backupignore file. It also sends me an email report if the backup fails or is successful every month. 

### My first NPM package!
I use the File API a fair bit, so I decided to create a library/package I could reuse that selects, reads, and previews files. You can check it out here [@aslamhus/fileselect](https://github.com/aslamhus/fileselect)

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

- Typescript
- Python
- Node 
- C++
- Tensor Flow

## Other Skills

- Graphic Design / Retouching (Adobe Photoshop / Adobe Lightroom)
- Video Editing (Final Cut Pro X)
- API testing (Postman)
- Writing (I'm also a playwright/poet)


## Some of my recent web dev work

[Cellar Live](https://cellarlive.com)
A website for one of Canada's leading Jazz Labels. Built with Wix. I am proud of an automated script I wrote for this website which queries their discography and populates their site's database. Previously, their company was having to manually update their discography across Bandcamp and their website, which could be tedious. Now a CRON job handles this for them.

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
