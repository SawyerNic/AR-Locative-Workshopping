# Workshop 4

[repo link](https://github.com/SawyerNic/AR-Locative-Workshopping/tree/main/Workshops/Workshop-4)

This workshop was a little frustrating, as even with continuous testing, I was not ever able to see my entity.  I also had to spend a lot of time configuring live server to run https on my home computer by generating .key and .pem files so that I didn't have to upload to pages every time I tried to test out my app.

### Effort #1

To try to get a blue ball to spawn near me I logged out my current location and used those exact coordinates as a location in the places array. After testing this and tweaking my coordinates I was ultimately unsuccessful. There are a few reasons why this may be the case. When reading the documentation for a-camera and gps-new-camera, it mentioned that location based services would be innacurate on wifi, however there would be no way I could test my application without wifi because I am using live server and need to access the locally hosted app from my phone. I then tried to simulate the coordinates for the camera, but to no avail. I was still unable to see the blue balls.

### Effort #2

I decided to go ahead and try the dynamic poi using the overpass API, but I still wasn't able to see anything. After modifying camera settings and making small tweaks I decided to call it wraps and write this blog post. I think for the final project I will be doing things from scratch instead of trying to make a template work.

### 
