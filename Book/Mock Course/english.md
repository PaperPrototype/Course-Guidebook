# Instructor Intro
Whenever people start doing something or using something in a certain way make it a feature. For example peopke were going to use our current courses as an example of how they should make a course. To better optimize their workflow we've made this "mock course." By making a mock course we can ensure that the course a teacher uses as an example explicitly shows how it explains itself and why.

The following are the 2 most important goals when making a course:

> Explain the problem really well so that the solutions becomes more obvious. A student should be able to say "Oh that makes sense!"

> Explain the implementation really well so that the student understands how it works. A student should say "Huh, that's cool."

Almost every guideline we give comes back to these 2 goals.

Anything in brackest "[]" are not part of the course but are comments made by the teaching team at crux3D. Anything in "()" is a comment for the student and *is* a part of the course.

The following Mock tutorial is from the course "Intro-Voxel-Terrain-Systems-in-Unity" on making a gradual planet orientation for gameObjects in Unity.

# Mock Intro
[We always start an explanation of a concept with something super simplified so that we can grow the concept later and show how it "really" works. This is so that the student doesn't get overwhelmed and give up because the inital explanation didn't make sense. We re-wrote the following papragraph 3 times until it made sense the first time someone read it. WE worte a rough version of the parapgragh and then improved it, don't worry about getting it perfect the first time, or you will never finish the course. The usage of the word "normalized" was explained on the spot. If we had explained it in another section before we would simply remind the student what "normalized" means by putting a synonym comment like "(between 0 and 0)."]

We want to gradually have the upDirection affect the players orientation. We will query the animation curve with a normalized distance from the planet (this is because an AnimationCurve only lets us ask it for normalized numbers). Then we use the number we get from the AnimationCurve(the number we get is also normalized) as a multiplier to affect the amount that the upDirection has on the player's up transform.

[We wrote the follwoing parargaph as a description for the artist. But it was so good that we added it to the course! We even used it to improve and re-write the above paragraph's explanation]

Here is a gif showing a distance number being used to query an animation curve to determine the affect of the upDirection vector on the player's up transform.

[We added a "TODO" after the picture as a reminder for the artist, myself, so that the writer could continue writing and not have to stop]

![gif showing a distance number being used to query an animation curve to determine the affect of the upDirection vector on the player's up transform]() TODO

[At this point we paused to continue working on the actual code and tutorial this mock course is based on. We purposefully made the mock course alongside a real world example, which is why we had to pause.]

# Instructor conclusion
Hey this is me the writer of this mock course. I took a pause to work on something else if you are reading this. I am not done writing the mock course. I 

