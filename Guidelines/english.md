# Intro
These guidelines are guides and tips not a set of rules, so if you have a better way to do something, then do it. Generally these guides have been taken from people like Elon Musk ("The biggest problem with education is we don't know why we are learning sonething" --Elon Musk) or are a result of frustrations the author(s) experienced during education that the want fixed.

If a guideline is not clear or is redundant or hard to understand then make a new Issue so it can be fixed.


## COURSE_GUIDELINE_000
**WHY AM I LEARNING THIS? HOW IS THIS USEFUL?**

Make sure student knows why they are learning something and how it is useful. Start with a naive approach that lacks and then show them how the newer technique will help them out. Give an example as to how it is useful. If its not useful then why learn it? If you show someone the usefulness of something they'll want to learn to use it!

![Elon musk attacks the education system](https://www.youtube.com/watch?v=UVHPHNegJNc)


## COURSE_GUIDELINE_001
**BE THROUGH**

This is probably the most important part of teaching. Most courses or tutorials I have found online like to skip over things, or just not fully flesh out everything that you are doing. It is super important that you understand every concept and bit of the code, otherwise you won't be able to apply what you learned in your own projects, outside of the tutorials your not quite sure how to use it. Your following along with some code, and then the code gets explained. This for me was never enough, I needed pictures and better more thorough explanations. I needed to be able to start with a super simple version of this so and then work up to the more involved version withlots of other stuff going on. If you teach something on its own, and then use it in a more complex example alongside other stuff, you already know how it works, so the other stuff doesn't overhelm you.


## COURSE_GUIDELINE_002
**INTRODUCE CONCEPTS, EXPECT BEGINNERS, EXPLAIN JARGON**

When introducing a new concept don't use any jargon or techincal words. Instead use plain english and simple words. Be as concise as possible, while still being thorough. Make sure that it is well explained with physical examples. Don't be vague, and make sure that no reader is left scratching their heads. A short but sweet explanation that really hits the spot is worth taking the time to make (epecially for the student). I'm not saying sit there and write every word to be perfect, just if you think of a better explanation or find a way to explain it that really makes sense, then go back and redo your explanation. This is something we highly value at Nanite3D. Once the student understand it, tell them the techinical name of the concept. (Make sure to add this concept and its jargon (technical word) to the Notes!) From then on use the jargon / technical word when explaining things. This way students learn words and vocab as they go through the lectures.


## COURSE_GUIDELINE_003
**JUST THE FACTS**

No opinions. (If you want to explain your opinion then we highly recommend you make a blog post about it you can link to that blog post, try medium.com). Instead show both alternatives and working examples. This way the student see's technology and possiblility's, not potholes to be avoided.


## COURSE_GUIDELINE__004
**SOMETIMES SHORTER IS BETTER**

When explaining a concept ask yourself these questions.
 - Will the student be using this information
 - Is this the shortest simplest possible explenation, using pictures, that will get the concept accross and understood.
 - Am I babbling? Useless words put people to sleep.
 - Is this sentence hard to read? (If it is then plaese take the time to fix it!)
 You may rewrite a sentence several times but that is time saved for the student, as well as painful sentence structure that nobody wants to read.


## COURSE_GUIDELINE_005
**EXPERIENCE**

As stated before opinions aren't necessarily useful. This is not true of experience. Experience is **very** useful, as it takes years to learn certain things. By adding things you;ve learned from exerpience to a course, you are advancing the student by however many years it took you to learn that. Relaying experience is important but keep it short. Also you can link to blog posts for lengthy or in depth advice / opions / experience. Try medium.com for blogging its free and... very awesome.


## COURSE_GUIDELINE_006
**WRITE NOTES FOR STUDENTS**

Every time you introduce a new concept add it to the notes. Be super concise and add shortened examples from the lecture. Notes are for those needing a refresher. Notes should use jargon (technical words), as long as they are defined in the Vocab section of the notes and were discussed during the lecture. Notes should also include all struct types and programming language keywords used and their usage and definitions and what those types do, or how those keywords affect stuff.


## COURSE_GUIDELINE_007
**LEARN BY CONCEPT AND EXAMPLE**

Don't try to pre-explain vague ideas or concepts, this will lose the students interest and focus. Instead explain things as you have use them in a physical example, and be thorough! Use diagrams and examples before showing the code. This keeps students from getting bored. But also ensures they understand what you are teaching them.


## COURSE_GUIDELINE_008
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


## COURSE_GUIDELINE_009
**CLEAR COURSE PREREQUISITES**

When making a course it must have prerequisite courses going from beginner to your course. If there is not a fully fleshed out course path, then at least have courses planned to fill the gaps. Here at Nanite we try to focus on the core courses to get people up and running, so usually we will already have the appropriate prerequisite courses made for beginner subjects. Feel free to build courses on top of ours (on top meaning our courses are a prerequisite to yours), actually we HIGHLY encourage this!


## COURSE_GUIDELINE_010
**USE ENGLISH AS THE STANDARD**

When translating a course, use the english version as the standard for trnaslation. This is for a reason. English is taught in many schools. If your making a course in another language make sure to translate it into english. That way other trnaslations can be based on the english version.


## COURSE_GUIDELINE_011
**EXPLAIN THINGS AS MUCH AS POSSIBLE UP FRONT**

When explaining a concept don't graze over "irrelevant" stuff and say "we'll explain this a couple lectures", or "this will make sense later". Explain it! **Use pictures** (a pictures worth 1000 words)! Using pictures will reduce the number of words the student has to read, and it makes the explenation much easier to understand. 

The exception is when concept 1 cannot be understood until concept 2 is learned, but you have to use 2 first and then learn 1. One example is learning C syntax, you have to know what a function is before you can understand what `void` really means.

The goal is to prevent the student from using something without understanding it, leading to frustration. When someone understands something, using it becomes trivial (AKA easy).


## COURSE_GUIDELINE_012
**EXPLAIN THINGS WELL THE FIRST TIME**

Don't sacrifice readability for correctness. When explaining something don't give the formal definition and then explain what that definition means. Instead take time to come up with a good explanation that expects no previous knowledge, explain like your telling your grandma. The idea is to prevent giving an explanation that doesn't make sense to a beginner for them to later understand it. This leads to demotivation "I don't understand" or "That made no sense to me".


## COURSE_GUIDELINE_013
**TUTORIALS ARE FUNNER THAN EXCERCISES**

We've chosen **not** to have "exercises" for each lecture. Instead at the end of each lecture there are fun Tutorials (in the folder called tutorials) that act as "exercises" that students can do after finishing the lecture, but really they are optional and are meant to be fun.


## COURSE_GUIDELINE_014
**HOW TO GRADUALLY INTRUDUCE VOCABULAR USED IN THE INDUSTRY**

Since we are teaching lots of new concepts, we should also include vocabulary that the reader may not be aware of that may be used by other texts. If we were to just make a "vocab" section for each lecture that would get broing, instead when using a word that may not be known by others include the synonym that best describes the new word and put it in parenthesis. Then in the notes you can give its formal definition. This allows the student to continue reading without having to constantly refernce the notes for vocab you are using.