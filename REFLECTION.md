# Reflection – Daily Schedule Simulator

## What was your approach to designing the schedule?
I picked six activities that cover a full day, from waking up in the morning to winding down at night, so the simulation reads like an actual day instead of a random list of things. I used real parts of my routine like making coffee, doing work, and walking my dog to make it personal instead of generic.

## What was one challenge or unexpected behavior you encountered?
When I first added the setTimeout calls, I realized the delays don't stack on top of each other. I assumed each timeout would wait until the previous one finished, but they all actually start counting from the same starting point when the script runs. I had to space out the numbers myself (1000, 2500, 4000, etc.) instead of using something like 1500 for every single one.

## What does this assignment teach you about async code?
A regular script runs top to bottom immediately, line by line, with no waiting. With setTimeout, the code moves on right away and the delayed functions get scheduled to run later, out of order with the rest of the script. This assignment showed me that async code is about scheduling things to happen in the future, not about pausing the whole program.

## What creative element did you add?
I added a randomMood function that picks a random emoji from a list of moods (happy, sleepy, tired, calm, excited) and appends it to each activity. Every time the page refreshes, the moods are different, so no two runs of the simulation feel exactly the same.

## How does this project simulate or differ from real-world schedules?
It captures the general shape of a real day, morning to night, but real schedules don't run on fixed timers. Real life has interruptions, activities that run long or get skipped, and things that happen at unpredictable times. This simulation is fixed and repeats the same way every time (aside from the mood twist), while a real day never plays out identically twice.