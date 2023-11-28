### Hi, I'm Aslam 👋🏽


- 🧑‍💻 Full Stack Developer
- 📷 Photographer
- 🎭 A long time ago, in a galaxy far far away, an actor 
- 🌱 Currently learning websockets/service workers 


I am proficient in PHP, Javascript, CSS and React and also have experience in System Administration, Database mangement and API construction following RESTFUL principles. 

I was an actor and headshot photographer, but a musculo-skeletal disorder changed all that. Now I am putting all my resources into my love for technology 💻. I still do photography from time to time, check it out ➜ [aslamhusainphotography.com](https://aslamhusainphotography.com).

I Love writing **vanilla javascript**, love the functional programming of **React**, but also the OOP discipline of writing **PHP** classes! I am keen to learn more about lower level languages and improve my knowledge of **Data Structures and Algorithms**.

I've been a self taught web developer for 15 years. My first foray into coding was in the 1990s with Macromedia's Director (the prehistoric Flash) when I was 10 years old. I was building very (VERY) basic, Final Fantasy inspired RPGs, accompanied by similarly rudimentary, but very earnest 3D animations I made with Cinema4D.  I would pass the games out to my friends in grade school via the 100 floppydisks 💾 it took to archive them. (Thankfully ZipDisk came along in '94 - 100 MB of storage, WHAT?!?). These were simpler times. There was no YouTube, no StackOverflow, and very little documentation available. So progress was... glacial. Now the resources available for learning seem limitless and I am always hungry for more.


## Things I've built recently

### Video Editor
I built a vanilla javascript video editor interface that can handle trimming and cropping videos in browser. While the editor doesn't perform the video manipulation it exports an object with user edits that can be sent to a server where these operations can be performed. You can see a work example here: [https://aslamhusain.com/video-editor/](https://aslamhusain.com/video-editor/)

### Rectangle Packer algorithm
For a project I'm currently working on I need to stitch multiple videos together on the serverside to create the illusion of multiple videos playing simultaneously, which is not a viable option for the browser. The stiched video grids need to be created for different screen sizes. The problem I encountered was, how do I fit a variable number of videos into various screen sizes while maximizing the space used? The videos' aspect ratio is known, but the grid dimensions and screen size are not. I discoverd that this is a NP-Hard math problem, the Rectangle packing problem "where the objective is to determine whether a given set of small rectangles can be placed inside a given large polygon, such that no two small rectangles overlap. Several variants of this problem have been studied." I wrote my own heuristic algorithm that finds a best fit by starting with a best guess for the size of each video and then adjusts until certain optimal constraints are met. 

The second problem was to handle looping of the videos. Each video in the grid loops, so the entire grid video must loop as well. The hitch is that the videos have variable lengths. I used the euclidian lowest common denomintaor with prime factorization in order to determine the shortest length the grid video would have to be in order to accommodate all the loops of the videos. 

I wrote a series of PHP classes to solve these problems and stich the videos together serverside using FFMPEG on the commandline.

### PHP QueryBuilder and Database Classes

I wrote my own Database, Search and Query Builder classes, focussing on a fluent interface design to allow method chaining that both simplifies and allows for complex MYSQL queries.  I tried to balance flexibiltiy with complexity, leaving room to scale the classes for more sophisticated queries, while also avoiding unncessary bloat. The higher level Search Class allow me to perform both FULLTEXT match...against searches and searches that leverage the LIKE operator with wildcards. I enjoyed writing with the fluent design pattern because it makes the code both readable and flexible. 


### React piano keyboard

For a Jazz Radio station "coming soon" landing page, I built a simple piano keyboard which is playable with touch or the mouse. See it in action [https://straightnochaser.ca](https://straightnochaser.ca)


### React Table Component
I built my own Table component that handles operations like sorting, filtering, pagination and select and deleting rows. This is the front end solution that works nicely with the above database classes.


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
