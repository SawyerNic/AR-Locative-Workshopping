# Development scarier than a night at the museum

The idea: A robot that would walk back and fourth under the bridge connecting the Engineering Hall and Golisano.

What actually happened: A moving museum located in my apartment.

# Let's explore what went wrong:

To create an experience that was more than just a downloaded object visible in a specific place, I decided to explore ways to speed up my development process. My computer doesn't have the best geolocation capabilities and also lacks a gyroscope, so testing my experience through the camera of my computer is nearly impossible and definitely not optimal. The obvious solution was to use my phone to test out my experience. However, I didn't want to wait for my GitHub Pages to redeploy every time I pushed changes to my remote repository, so I wondered if there was a way I could access my locally hosted page from Live Server on my phone. As it turns out, I could! All I had to do was type in my IP address followed by the port my Live Server was using. But here is where we run into the first roadblock:

### Permissions and Protocals!

When doing AR development that requires a combination of all these permissions—location, orientation, and camera—DO NOT try to use Safari! It took me around an hour to figure out that, even after specifically requesting permission for all of these, Safari was just not going to work for thorough testing of my experience. When I opened the website, it gave me a popup: "After camera permission prompt, please tap the screen to activate geolocation." I did that, and then it gave me a "Sorry - Media Devices API not supported" error. I tried many things to debug, but ultimately I kept running into dead ends and bloating my page. It kept requiring more from my web app just to even turn on the camera, so I eventually gave up and decided to try Chrome instead. Even after switching to Chrome, I kept running into one roadblock: it required me to use HTTPS, which was a problem because Live Server uses HTTP by default. Luckily, there is a pretty simple fix described in this gist:[https://gist.github.com/prof3ssorSt3v3/edb2632a362b3731274cfab84e9973f9](https://gist.github.com/prof3ssorSt3v3/edb2632a362b3731274cfab84e9973f9)

After all these issues were resolved, I was finally able to work on the actual experience. However, it had to be simple and couldn't be what I initially envisioned because, throughout all the debugging, I had to head back home. So, I was constrained to my apartment. I decided to turn my apartment into a moving museum because strange things have been happening at night, such as random objects moving, unexplained sounds, and other sorts of weirdness. A sort of "Night at the Museum"-type experience, if you've ever seen that movie. I added the _Buste d'Auguste couronné de chêne_ and gave it some basic and slow movements. It looks very strange on the camera, but it does give off an unsettling feeling, which I think a lot of good art achieves.

### Video:

### Photos:

![](https://holocron.so/uploads/f80414dc-img-6264.png)

![](https://holocron.so/uploads/d36dccd4-img-6265.png)

![](https://holocron.so/uploads/53b01738-robot-sketch.jpg.jpeg)


