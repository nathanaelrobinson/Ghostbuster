# Ghostbuster
This is the script I used to iteratively find the percentage chance that the Ghostbusters from the FiveThirtyEight weekly Riddler Express Question blow up the world when they cross their proton beams at a campfire while shooting ghosts hidden amongst them.

Not spending much time on usability but if you want test it you can import the entire file and run ghostbusters_continuous(iterations) or ghostbusters_discrete(interations) with the number of iterations you'd like. The script returns an array of the moving averages for each iteration of the test, which are also saved as x, and y so that you can easily plot them to see the average converge.

Over 5000 iterations or so it seems to converge at 33.3%.

Due to an argument with my roomate over whether the fact that there are 20 distinct locations among the circle will influence the end probability we test both cases. The continous case randomly samples 4 locations along a unit circle and creates two particle beams and finds if those intersect. The discrete case randomly chooses 20 locations along a circle and then chooses 4 of those locations without replacement for the ghosts and ghostbusters.

As I expected (take that Brett!) the number of people around the fire doesn't matter as it boils down to 4 random locations around the circle and the final percentage appears to converge at ~33.3% or a 1/3 chance that the earth will be destroyed by our intrepid ghostbusters.
