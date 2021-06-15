# Intro
This is how the big picture for making courses and teaching subjects (this is not for how to teach indiviudal concepts). The goal is to get students to understand something well.

## Use Informal Language
Informal language is easier to understand and follow, and won't scare beginners away.

## In context
When teaching a subject teach it in context of its application / use. This makes it more tangible and easier to grasp.

## Teach the core so the student can explore its application
Teach the core techniques without letting "nice features" get in the way. The student can add the feature themselves to work with the rest of the code in future lectures, and if you think they can't, then add a tutorial after a lecture to help them out. This makes teaching the core concepts easier without having to "fix it" to work with the cool feature. Its easier on the student and easier on you the teacher.

## Clear course prerequisites
When making a course it must have prerequisite courses going from beginner to your course. If there is not a fully fleshed out course path, then at least have courses planned to fill the gaps. Here at Nanite we try to focus on the core courses to get people up and running, so usually we will already have the appropriate prerequisite courses made for beginner subjects. Feel free to build courses on top of ours (on top meaning our courses are a prerequisite to yours), actually we HIGHLY encourage this!

## Teach with the end in mind
Teach with the future "advanced" topics in mind, not just the current topic, because, after all, you don't learn math simply for the sake of math, but to be able to understand topics that require a knowledge of math. 

For example when explaining a compiler show that it converts code to CPU word based instructions, that are saved as binary, and when you call a function it is a binary instrction refering to another binary instruction. So that later, in another course, when explaining FFI, you can say, "because all programming languages compile to the same format (binary), it is possible to call a function that was created in another programming language."

## Teach how others want to learn
example 1: A = Math, B = Rocket Science

When explaining something we tend to want to teach A before before teaching B because A will help our students understand B. The problem is that A will be boring without B. Because the student is unfamiliar with B they won't take the time to learn A and will probably forget A because they don't understand its relevance for B and the whole point in putting A before B becomes pointless.

Instead teach A in the context of B and once the student starts needing A. As a result the student will now want to learn A and no further motivation is needed.

Wouldn't it have been great if school was like this!
