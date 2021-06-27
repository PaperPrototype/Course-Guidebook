# Intro
These guidlines are a set of problems students encounter when trying to learn, and the methods for teaching that prevent those problems. 
They are also a result of frustrations the author(s) or students experienced during learning.

"The biggest problem with education is we don't know why we are learning something" --Elon Musk [Elon Musk attacks the education system](https://www.youtube.com/watch?v=UVHPHNegJNc)

If a guideline is not clear or is redundant or hard to understand then we would love it if you make a new Issue so it can be fixed.


## DETAIL_GUIDELINE_000
**WHY AM I LEARNING THIS? HOW IS THIS USEFUL?**

Make sure student knows why they are learning something and how it is useful. You can do this by teaching something in context of its application / use. Teach in a way so that the student makes the to why something is useful. Don't just tell the student that they will need to know this information (which is what most books do). 

For things that are complex that the student will not want to learn, start with a simple naive example then show them how the newer complex technique will help them out. 

If you teach a student how to do rotations in 2D using plain math without matrixes and then transition to using a matrix to do the math, then they'll see how matrixes help, they'll go "oh, matrixes are a different way of laying out the numbers". Now they understand how it is useful. If its not useful then why learn it? If you show someone the usefulness of something they'll want to learn to use it!

The goal is to get the student to see the problems that the pioneers saw, and then help them build the solutions that the pioneers made.

![Elon musk attacks the education system](https://www.youtube.com/watch?v=UVHPHNegJNc)


## DETAIL_GUIDELINE_001
**GIVE THE REASON FOR A DECISION**

When you decide to do something make sure you give a reason. THis helps convince others of you decision and prevents you from making bad decisions because you are willing to question yourself. Again this also forces you to answer the why behind everything.

You will notice all of the guidlines here explain themselves and their reasons. This is a way of finding error through "first principles", always asking the why, until you find a fundamental truth about something. And then building on top of those fundamental concepts proving our concepts (or disproving them).


## DETAIL_GUIDELINE_002
**BE THROUGH AND DETAILED INCREMENTALLY**

This is probably the most important part of teaching. Most courses or tutorials I have found online like to skip over the a technique they are using, or just not fully flesh it out. It is super important that you understand every concept and bit of code, otherwise you won't be able to apply what you learned to your own projects (outside of the tutorials your not quite sure how to use it). I needed to be able to start with a super simple version of the technique and then work towards using it. If you teach something on its own, **and then** have them use alongside other stuff, they will already know how it works, so the other stuff doesn't overhelm them.


## DETAIL_GUIDELINE_003
**INTRODUCE CONCEPTS, EXPECT BEGINNERS, EXPLAIN JARGON**

When introducing a new concept don't use any jargon or techincal words. Instead use plain english and simple words. Try to be concise and waste as little time as possible by using pictures rather than trying to describe it! Make sure that it is well explained with physical examples. Don't be vague, and make sure that no reader is left scratching their heads. A short but sweet explanation with picutres that really hits the spot is worth taking the time to make (epecially for the student). You shouldn't sit there and write every word to be perfect because then your would never finish, so if you think of a better explanation or find a way to explain it that really makes sense, then go back and redo your explanation. This is something we highly value at Nanite3D. Once the student understand it, tell them the techinical name of the concept. (Make sure to add this concept and its jargon (technical word) to the Notes!) From then on use the jargon / technical word when explaining things. This way students learn words and vocab as they go through the lectures.


## DETAIL_GUIDELINE_004
**STUDENTS DON'T KNOW ANYTHING OUTSIDE OF PRE-REQUISITES**
Don't expect students to know anything outside of the pre-requisite courses. If you are going to use an `IEnumerator` but `IEnumerator`'s are not explained in a pre-requisite course then take the time to explain them. This creates courses that are made for fast and optimized courses, because you learn information as you need it. This prevents from having to have long exhaustive pre-requisite courses that cover every possible thing you might need to know.

At the same time this keeps with DETAIL_GUIDELINE_000, since the student will know "why" they are learning something, rather than shoving a ton of infromation that "they will need to know". Nobody likes to learn a ton of information "they will need to know", we natrually want the information to come as we need it, this is much funner and results in less time wasted.

## DETAIL_GUIDELINE_005
**JUST THE FACTS**

No opinions. (If you want to explain your opinion then we highly recommend you make a blog post about it you can link to that blog post, try medium.com). Instead show both alternatives and working examples. This way the student see's technology and possiblility's, not potholes to be avoided.


## DETAIL_GUIDELINE_006
**SHORTER IS BETTER**

When explaining a concept ask yourself these questions.
 - Will the student be using this information
 - Is this the shortest simplest possible explenation, using pictures, that will get the concept accross and understood.
 - Am I babbling? Useless words put people to sleep.
 - Is this sentence hard to read? (If it is then plaese take the time to fix it!)
 You may rewrite a sentence several times but that is time saved for the student, as well as painful sentence structure that nobody wants to read.


## DETAIL_GUIDELINE_007
**EXPERIENCE**

As stated before opinions aren't necessarily useful. This is not true of experience. Experience is **very** useful, as it takes years to learn certain things. By adding things you;ve learned from exerpience to a course, you are advancing the student by however many years it took you to learn that. Relaying experience is important but keep it short. Also you can link to blog posts for lengthy or in depth advice / opions / experience. Try medium.com for blogging its free and... very awesome.


## DETAIL_GUIDELINE_008
**WRITE NOTES FOR STUDENTS**

Every time you introduce a new concept add it to the notes. Be super concise and add shortened examples from the lecture. Notes are for those needing a refresher. Notes should use jargon (technical words), as long as they are defined in the Vocab section of the notes and were discussed during the lecture. Notes should also include all struct types and programming language keywords used and their usage and definitions and what those types do, or how those keywords affect stuff.


## DETAIL_GUIDELINE_009
**LEARN BY CONCEPT AND EXAMPLE**

Don't try to pre-explain vague ideas or concepts, this will lose the students interest and focus. Instead explain things as you have use them in a physical example, and be thorough! Use diagrams and teach the concept before showing them the code. Then when they use the code it makes sense. This keeps students from getting bored. But also ensures they understand what you are teaching them.


## DETAIL_GUIDELINE_010
**CODE SNIPPETS**

Any code snippets shown need to be in context. It can be confusing when you don't tell the student where that snippet is supposed to go. Also make sure to add `// ... snipping irrelevant code ... //` where code that has already been written is. For example

```
        m_vertices = new NativeArray<Vector3>(24 * Data.chunkSize * Data.chunkSize * Data.chunkSize / 2, Allocator.Temp);
        m_triangles = new NativeArray<int>(36 * Data.chunkSize * Data.chunkSize * Data.chunkSize / 2, Allocator.Temp);
```

can be confusing compared to 

```
    private void Start()
    {
        m_vertices = new NativeArray<Vector3>(24 * Data.chunkSize * Data.chunkSize * Data.chunkSize / 2, Allocator.Temp);
        m_triangles = new NativeArray<int>(36 * Data.chunkSize * Data.chunkSize * Data.chunkSize / 2, Allocator.Temp);
    
        // ... snipping irrelevant code ... //
    }
```

The exception to the rule is when showing code that has already been shown, but that has only changed slightly.


## DETAIL_GUIDELINE_011
**USE ENGLISH AS THE STANDARD**

When translating a course, use the english version as the standard for trnaslation. This is for a reason. English is taught in many schools. If your making a course in another language make sure to translate it into english. That way other trnaslations can be based on the english version.


## DETAIL_GUIDELINE_012
**USE PICTURES AND DIAGRAMS**

A good diagram or picture can save you 2 pages worth of explaining. This is better for you and the student. And it improves the reading time for the student. 

Also simple diagrams are easy to understand (when explained), and are in most cases much easier to understand than purely written explanations.


## DETAIL_GUIDELINE_013
**DON'T NAME IT TILL YOU'VE EXPLAINED IT**

When you say something like "The magnitude of a vector is the length of the distance it covers relative to its coordinate space." Maybe you can see the problem. In describing the magnitude of a vector, for those who already know what the magnitude of a vector is, the explanation will make sense. But for a complete beginner you've essentially wasted your time.

How so? When a word is used that the studetn doesn't understand,in my experience, their brain immediately stops comprehending what you saying, and stops proceesing the meaning of what you are saying.

The way I solve this is to not include any words the student doesn't already know when describing the definition of something. As an example from the Voxel Terrain course

> When the the distance from the origin (aka `Vector3(0, 0, 0)`) of a vector to the "pointy end" of that vector is 1, we say that the vector is a "Unit Vector" (check the notes of this lecture for definitions of all the vocab and techy words). The distance from the center of our normals `Vector3(0, 0, 0)` to its end `Vector3(0, 0, 1)` is obviously 1, so we are fine.

Then after I've defined it I give it a name.

(I actually re-wrote the explanation after having written this)


## DETAIL_GUIDELINE_013
**EXPLAIN THINGS WELL THE FIRST TIME**

Don't sacrifice readability for correctness. When explaining something don't give the formal definition and then explain what that definition means. Instead take time to come up with a good explanation that expects no previous knowledge, explain like your telling your grandma. The idea is to prevent giving an explanation that doesn't make sense to a beginner for them to later understand it. This leads to demotivation "I don't understand" or "That made no sense to me".

The goal is to prevent the student from using something without understanding it, leading to frustration. 

When someone understands how something works, using it becomes trivial (AKA easy).


## DETAIL_GUIDELINE_014
**USE TUTORIALS NOT EXCERCISES**

Only teach concepts in the lectures and leave the experimentation to the student and tutorials. If you include a section on "How to make a cool shader effect" with what the student has learned you're taking their time up for experimentation and making them do what you think would be cool. Instead if you think the student might want to do something cool with what they've learned create a tutorial that can be taken after the lecture is over.


## DETAIL_GUIDELINE_015
**HOW TO GRADUALLY INTRUDUCE VOCABULAR USED IN THE INDUSTRY**

Since we are teaching lots of new concepts, we should also include vocabulary that the reader may not be aware of that may be used by other texts. 

If ew jsut start using the vocab and the make a "vocab" section for each lecture that would get broing and frustrating for the student. 

Instead when intriducing a concept use the plain english example with analogous words, that can transition to the "correct" word easily.

You can also include a synonym for a technical word (in parenthesis) to help the student better understand a new word. It is alsoa good idea to repet the technical words synonym a couple times and not expect the student to immediately be able to use the word. THis helps the student get used to using the word without overwhelming them.

In the notes of a lecture give all the vocabulary and their formal definition, as well as an explanation of the word. This helps the student when they forgot the meaning of a word. Also if you don't they will probably look it up on Google, which may give them the wrong definition of a word since, for example, the word "vertex" can also mean "	The highest point; the apex or summit." or "The highest point of the skull."
