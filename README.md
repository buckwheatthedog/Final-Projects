
				 Final Project Reflections:

For my final Projects, I created both my "Data Clay" project, and a prototype for a project I am working on with families. 

1. For the Data clay project, I intended to record the process of making something through some sort of sensor. I played round with accelerometers, force sensors and flex sensors until I landed on force sensors because they suited the build platform I had designed and were giving the most consistent results without calibration. This also made them easier to use in the field. My working style for the first project included modifying existing Arduino and processing examples to accommodate for 4 force sensors together. 


2. For my second final project, a prototype for family structure and accountability, I created a context based prototype that communicates over Wi-Fi. The prototype records a task with a simple button press, starts a countdown timer, and when the task is done, it sends the next device a string of characters over wifi that the other board "subscribes" to, continuing the process until all objectives are complete.


Along the way with both projects, I learned to overcome the following 5 things (as well as many others): 

1. Modifying existing sketches is a practical and thought invoking way for me to solve problems with code. If I can put pieces and chunks of a puzzle together, it not only helps me see parts of the functionality already manifested, but also helps me have a basis in case I want to totally change it. As I started my first project, modifying examples gave me a good way to lower the barrier to entry. I then felt confident enough to 

2. By stepping back and creating a flowchart (or Psuedocode) in my case, it can help you solve a problem much more thoroughly and systematically. When I used this method, I ran into less errors. Before writing down my problem in detail, I was lost at where to begin.

3. In my family prototype project, I had tons of trouble connecting one board to the other board through Wi-Fi. The Photon board I was using contained an example called the “Buddy System” whereby one board subscribes to the other. I had issues involving subscribing to the wrong Photon names and identifiers, because every time I wanted to run my prototype in a new place, I had to change the name of the board. I got help with this section of the debugging. We ended up creating code that references one board ID that stays constant using an if/ else statement to handle any board identifier that was added.
“if (myId.equals("290045000851353531343431")) { // device ID
        me = "homework"; // name of my current board
        next = "chores"; // name of the next board. 
    } else {
        me = "chores"; // if myID is not the above, it must be “chores”, because there is only 2 possible boards in this prototype. 
        next = "homework";
    }
“

4. I was getting confused and hung up on new variables I had never seen before for a long time during my process.  Things like “char”, “unsigned long” etc. we’re confusing to me as I tried to decode examples. I realized that of course, everything is in the reference. As soon as I checked the reference, I was able to get my code working, using the correct variable to handle each class of data. 

5. Ultimately the largest problem I had with both projects was figuring out where to spend the most time trying to debug something. Since I was most comfortable with the physical wiring, I started there, and then tried to work up into the code ladder. This worked, but I realized my wiring was correct most of the time. Going forward, I think I will start with the element that I had the most trouble with, because this is likely where the “bugs” live. 
