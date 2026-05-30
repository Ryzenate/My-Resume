What can I add that speaks to when I took the IR filter out of the USB camera I was developing DirectShow and TWAIN/AVI drivers for and wrote a DLL to monitor camera stream for motion.  I added an IR emitter to the front of the USB camera, using power from the usb. I created a method to save frames to disk whenever the difference in pixels reached a configurable threshold and saved to disk.  i ended up using this to catch my "dog food thief" in the garage - Play by play frames of a mommy rat and 2 smaller ones. The next use for this project was after I set out a rat trap with cheese.

The Hook: "I wanted to test the limits of low-light computer vision, and I happened to have a pest problem in my garage with a mysterious dog food thief."

The Hack: "I stripped the IR filter off a USB camera I was writing DirectShow and TWAIN drivers for, soldered an IR emitter directly to the USB power line on the board, and wrote a quick C++ DLL to monitor the stream."

The Logic: "Instead of running heavy framework code, I just calculated the frame-to-frame pixel differentials. If the change delta crossed my threshold, it dumped the frames to disk."

The Payoff: "It worked flawlessly. I got a perfect, high-frame-rate, night-vision sequence of a mother rat and two babies raiding the food. I used the data to strategically place traps, proved my driver and algorithm stability under continuous load, and cleared out the garage."