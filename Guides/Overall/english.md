# Intro
This is how the big picture for making courses and teaching subjects (this is not for how to teach indiviudal concepts). The goal is to get students to understand something well.


## Teach through convincing people
This is because when you are teaching you are "working to convincing someones mind about how something works" -- Me. 

If your mind can't connect the dots (aka be convinced) then you will have a hard time understanding something.

I think this is how people naturally **want** to learn but I may be wrong. Why do it the way people "want" to learn? If we take it back to first principles and look at a baby... actually a toddler you will notice they always ask "Why". (<-- See what I did there! I answered the "why") 


# Review and Repetition makes it stick (but don't bore them)
When doing a tutorial or writing a course it is really good to re-explain information even if the student "should have already learned this in another course". This helps since a student may have forgotten that information and a student may have just decided to skip the pre-requsites and dive right in. We are making courses for students, and so we should make the courses for what students "tend to do", and not what students "should have done".

Even if the student does already understand something, reviewing it in the context of what you are teaching will grow a students depth of understanding of it (in that context rather than just the general understanding). 

It also helps to review stuff as it further ensures nobody is left behind! I try to always add a comment with parenthesis (like this) re-defining a student of a concept we covered previously just in case they forgot.

IGNORE THIS:
	We will be making this format the standard for every lecture / section / tutorial we make. You can make this more obvious by writing "problem/goal:" in front of the explenation of the problem/goal at hand. And then writing "solution:" in front of the explanation of the solution. Then writing "implementation:" in front of the implementation. Then "Why:" when explaning why you did something a certain way.

	The order of ""question/problem, answer/solution/concept, implementation, and why" will vary. For example "why" may come after the "answer/solution/concept".

	(I have yet to prove/figure out why this format for teaching is better than other formats)


## The end goal is what they are here for!
Start teaching with the end goal. Don't cover the elementary stuff in preparation from its future application, teach the elemetary stuff in the trenches as you are trying to achieve the end goal. This keeps peoples

As an example take a "Intro to Rendering" course. You state the objective as "how do we get 3D picture on a 2D screen?". Proceed to immediately start making a simple 3D renderer, then explain the dot product and use it. Then explain *basic vectors*, and use *basic vectors* to skew the visuals being rendered.


## Use Informal Language
Informal language is easier to understand and follow, and won't scare beginners away.


## Teach the core so the student can explore its application
Teach the core techniques without letting "nice features" get in the way. The student can add the feature themselves to work with the rest of the code in future lectures, and if you think they can't, then add a tutorial after a lecture to help them out. This makes teaching the core concepts easier without having to "fix it" to work with the cool feature. Its easier on the student and easier on you the teacher.


## Clear course prerequisites
When making a course it must have prerequisite courses going from beginner to your course. If there is not a fully fleshed out course path, then at least have courses planned to fill the gaps. Here we value getting people up and running, so usually we will already have the appropriate core prerequisite courses made for beginner subjects. Feel free to build courses on top of ours. "on top" meaning our courses are a prerequisite to yours, actually we HIGHLY encourage this!


## Teach with the end in mind
Teach with the future "advanced" topics in mind, not just the current topic, because, after all, you don't learn math simply for the sake of math, but to be able to understand topics that require a knowledge of math. 

For example when explaining a compiler show that it converts code to CPU word based instructions, that are saved as binary, and when you call a function it is a binary instrction refering to another binary instruction. So that later, in another course, when explaining FFI, you can say, "because all programming languages compile to the same format (binary), it is possible to call a function that was created in another programming language."


## Teach how others want to learn
example 1: replace A with "Math", and B with Rocket Science

When explaining something we tend to want to teach A before before teaching B because A will help our students understand B. The problem is that A will be boring without B. Because the student is unfamiliar with B they won't take the time to learn A and will probably forget A because they don't understand its relevance for B and the whole point in putting A before B becomes pointless.

Instead teach A in the context of B and once the student starts needing A. As a result the student will now want to learn A and no further motivation is needed.

Wouldn't it have been great if school was like this!


# Have beginners teach beginners and experts teach experts
A pattern I have seen is when a highly adavanced teacher teaches a book or concept they skip over the beginner concepts and spend very little time on them. As a result beginners are foten left in the dust and give up.

But, when a beginner teaches something they focus highly on the beginner concepts and really put it well in a way that other beginners can understand.

So our idea is to have beginners be taught by experts, and then ghave those beginners teach the beginner courses. THen for highly advanced courses the experts can teach them.


# GET TO THE POINT!
People usually don't enjoy reading your opinion or thoughts "bla bla bla" (unless they are useful). Especially in a course where they are looking for information and knowledge. When writing a learning resource always think about what the student will find useful. Get to the point and teach them what they came for.


# A reason for eveything
There should be a reason for everything. You want to make sure you are doing things that will improve the quality of what you are teaching. You can't imporve quality without knowing why you are explaining something in a certain way. THe best way to find a good explanation is to sit with a student as they read your explanation and ask them if it made sense, and if it didn't then explain it to them until they understnad, through this process you will find a good explanation.

It is important to always give a reason for everything because we will be able to finding our own error's in logic or what we are teaching / explaining and correct them. 


# Everything is gradual
Take things gradually. An occuring pattern in software (and in life it seems) is that change is the only constant. So when writing your course don't try worry about a "final" version as there will never be a final version (or maybe there will be...). Just start writing the course and working on it, it will take shape as you go. THe best way to shape a course is to observe students taking it (in person) and finding where they are getting stuck. Try offering the course for free to your friends (or evne pay them to take it).


# Personal or not ("I" or "we")
Do students take advice more if it is personal from you?
Do students learn better if we use the personal grammar?

Proofs: (This will help us answer the question, feel free to contrib)
Advice is more likely tp be listened to when coming from a person we trust.
Advice is more likely tp be listened to when it is given on a personal level.

Ultimately is the course "better" if we use persoanl or inpersonal speach.

I have yet to figure this out.


# Contribute to Wikipedia
If I link to a Wkipedia resource I find it good to contribute to it and make sure it is a not a bad or incorrect explanation, since, it's likely the student will be reading that WIkipedia article.


# Inspire students
Most people who get into game development did so because of a video game they played. If we inspire our students with epic demos of some technology, it's likely they will want to make it. When they find out that there is a course on how to make it, my guess is, they ewil