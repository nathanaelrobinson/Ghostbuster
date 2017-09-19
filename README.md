# Ghostbuster
This is the script I used to brute force find the percentage chance that the Ghostbusters from the FiveThirtyEight weekly Riddler Express Question blow up the world when they cross their proton beams at a campfire while shooting ghosts.

Not spending much time on usability but if you want test it you can import the entire file and run ghostbusters(iterations) with the number of iterations you'd like. The script returns an array of the moving averages for each iteration of the test, which are also saved as x, and y so that you can easily plot them to see the average converge.

Over 5000 iterations or so it seems to converge at 48.5%.

This assumes the campfire attendees are randomly distributed at 18degree increments around a unit circle campfire. The script randomly chooses four locations for our two ghostbusters and two ghosts. It then finds the locations on the unit circle that they would be seated and the equations of the lines that would be emitted from their proton beams. The intersection of the proton beam lines is calculated and if that point lies within the unit circle then we confirm that the world is destroyed.

Note, there is no case for the scenario when the lines are parallel so answer may be off.
