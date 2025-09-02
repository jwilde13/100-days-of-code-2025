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