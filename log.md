# 100 Days Of Code - Log

### Day 0: September 1, 2025

**Today's Progress**: Create and publish a test app with Ionic!

**Thoughts:** To start off the 100 days of code, I started down the path of building an android app using Ionic and AngularJS.
I downloaded Node.js and Android studio and the Java JDK. It was a bit confusion going through the NPM and Ionic commands. I mostly followed the tutorial to get the app up and running. 
The next issue I faced was getting the keystore generated. I solved this by double checking the path the keystore file was being saved to. It turns out I wasn't in the right directory for it to save it. Once I changed the path, the keystore generated with no further issues.
The app was the basic photo gallery. Not bad for the first Ionic App I’ve attempted to follow and do. I struggled with getting it uploaded into the Google play store. I didn’t realize that it had to be in AAB format and not the APK. 

I ran into a few additional issues uploading the AAB file to the Google Play store. 
1) the package nameing was an issue. It had to be in com.xxx.xxx format.
2) I didn't realize that the default package was already uploaded into the Play store so I had to rename my temp app.

**Link to work:** The [tutorial](https://ionicframework.com/docs/angular/your-first-app) I used from Ionic.



### Day 1: September 2, 2025

**Today's Progress**: Build a heatmap to track progress!

**Thoughts:** Today I wanted a way to visualize my progress while doing the 100 days challenge. I really like how GitHub displays activity via a heatmap. I started by creating a table and looping from 0-52 to build the week columns and the day values. I was able to get the colors I wanted but it felt clunky. I found this heatmap library called cal-heatmap that I liked so I decided to switch to it. There were some issues I faced when getting the heatmap to load correctly. Once I was more familiar with the library, it worked out really well.

**Link to work:** The [Heatmap Github](https://cal-heatmap.com/) repo I used. 

**Link to work:** See my [Heatmap Demo](./Demos/heatmap.html) that I created. 


### Day 2: September 3, 2025

**Today's Progress**: Build a task tracker and note form!

**Thoughts:** I am very unorganized and often start things and don't finish them because I get distracted by the next thing. I decided to practice my PHP skills and front end development by creating a To-Do list and a note taker. The languages used are jQuery, Bootstrap, PHP for backend and MySQL to store the data. I've worked with PHP what I thought was a lot but my skills are rusty. Using the PDO->Prepare() for connecting to a MySQL database is something that I have done, but it has been a while. I learned more about parameterization with PDO. 


### Day 3: September 4, 2025

**Today's Progress**: Add Bootstrap Modals and look pretty!

**Thoughts:** I decided to focus on improving the UI of the To-Do page that I built yesterday. I hooked up the AJAX methods to be able to comunicate with the APIs I build to Add new tasks, Get the tasks, Get the task detail and mark them as complete. It seem like I didn't do a lot but I did connect a lot of dots to make it function more like a usable application.

![ToDo Screenshot](./screenshots/day-4-screenshot-todoPage.png)

### Day 4: September 5, 2025

**Today's Progress**: Crypto Ticker!

**Thoughts:** Today I went with a simple C# application that I have been wanting to do for awhile. I have wanted to create a small application in C# that would be the top most app on the screen and show the current prices of certain cryptos I was interested in. I decided to use the API from Coinbase as my source for the current prices because it has an endpoint that I didn't have to authenticate for. One of the key features that I wanted to build was to have an indicator that shows how much the value has gone up (green) or down (red) as a visual indicator. That was done by keeping a history of the most recent value and compare it against the current value (delta). I used the datagridview element because it had the table look I was going for. The hardest part of this was keeping track of the math. 

**Link to work:** The [Coinbase API](https://api.coinbase.com/v2/exchange-rates) I used. 

Screenshot 1
![ToDo Screenshot](./screenshots/day-5-cryptoTicker-1.png)

Screenshot 2
![ToDo Screenshot](./screenshots/day-5-cryptoTicker-2.png)


### Day 5: September 6, 2025

**Today's Progress**: ToDo Update and Crypto Ticker Update!

**Thoughts:** After watching the Crypto Ticker for awhile today, I realized there were some bugs in it. I gave the ToDo list some miliage and added the tasks there and realized I didn't have a way to mark tasks as being done. I created the API for that and added a green button to it.

It wasn't correctly showing the delta value even though the current value did change. I realized that the table was updating at a much slower rate than the Coinbase API was being checked. So the delta value would have been updated several times before the table was refreshed. 

I added some alert logic for display a message box if the coins start to go up to fast or down in a give time, or if it reaches a certain price point. It has been fun watching it tick and update. 