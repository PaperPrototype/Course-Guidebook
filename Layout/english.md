AHH! This needs updated, as I have learned much about teaching since the original writing of this particular piece of text.

# Course Types
We separate courses into 2 types, one being an intro course covering the most generic basics, then outro courses covering the specifics that serve as more of a reference + exhaustive dropbox for knowledge. This makes the initial courses smaller and more modular, while being WAY less boring. I found that having one MONOLITHIC "book" as I found this simply didn't work well for me.


### Intro Course
A knowledge course should be designed to teach a student concepts and then let them explore those concepts in their own projects through optional tutorials. These courses should not be made of one large project, instead they should use the smallest and simplest "micro projcts" that teaches new concept(s). This ensures the concepts you need to teach don't have to become specialized or bogged down by the specifics of the "cool large project" you are doing.

Intro courses should be short. You can achieve this and guideline 000 (teaching how it works not how to use it) by litterally following guideline 000! When you teac hsomeone how something works, you have less to explain in terms of how to use it, and the explanation of how to use it becomes very obvious.

### Outro course
I'm thinking these courses should start where the intro course left off. I (currently) don't see a problem in making outro courses extensive and detailed, as the intro course should have done pretty good at introducing things, so the basics are out of the way and you can focus on the nuances.

### Tutorial Course
(This is my idea of the word "tutorial" in context to courses I make... which, as with most things, can change over time)

A tutorial course would proabably come after an intro course. A tutorial course would teach you how to apply what you learned from an intro course to a specific project, like say making a planetary terrain. Although honestly if the knowledge has already been layed out in an intro course then I can see tutorial courses being quite short! As such I find it is feasible to simply include these as mini courses that come in the form of "tutorials" after each lecture in an intro course.

By this point you can guess that a tutorial course would probably not have much to teach the student besides a few naunces of applying their knowledge to a specific project.

I can see a tutorial course teaching the student how to make one large cool project like a specific popular renderer from a game they love, or making an AI physics system, or making minecraft! These courses are meant to be fun! They will inevitably have to teach some concepts, but currently it seems, that it would be better if these courses were to come after a knowledge intro course and simply apply what the student already knows and show them how to use it to make, for example, a planet (using what they learned from an intro voxel systems course). As such, Tutorial courses must always have a pre-requisite knowledge course, or, another Tutorials course.

Tutorial courses won't teach people much, so really we should focus on making knowledge courses. This also conforms with the ideas in guideline 000.

# Layout
Knowlwdge courses should only teach the core basics, not all the naunces and details (otherwise we will kill the beginner, and any potential interest they may have by overwhelming them). This makes knowledge courses shorter and prevents having monolithic courses. This happened with [The Rust Book](https://doc.rust-lang.org/stable/book/). 

Don't overwelhm the student with all the nuances, just teach them the concepts, they can learn the nuances later.

The following can be ignored. As it is just me thinking / ranting:

To solve this we create intro (or Knowledge) courses, that only teaches the core and simple stuff, nothing fancy, with side tutorials after each lecture to keep the student entertained with the knowledge they've learned, and satisfy their natural want for applying their newly aquired skill to some cool project (like making a small planet using voxels).

Then after the intro courses we can have outro (or Tutorial) courses, that, take the knowledge of the student and apply it to a very specific project. This way students don't get bored by a course that tries to teach "everything" because most of the time a student is interested in a specific thing, that they will use for their own project.

We make sure to teach the student the more complex stuff and all the specifics in the TUtorial courses. We are able to keep their attention because they are making an awesome project, and they already know all the basics, so we can get straight to the complex and specifics and get them over with relatively quickly. This also allows many, many, outro or Tutorial courses to be made after an intro course, giving lots of possibilities to the teacher. Whereas if we just made one monolithic generic course, you have to cut away and try and reach a larger audience, making the course longer and more boring for the students.

This keeps the intro (aka knolwedge) courses fresh, small, and easily finishable. Which sadly is **not** how THe Rust Book stayed.

INFO: {
    4342 5660 1026 3118

    05/25

    248
}

json format with types?
- lightweight (compact less text)
- simple (easy + fast to parse)
- fast (simple = fast to parse, less branch prediction for CPU (guessing which if statement is correct to gain faster performance))
- types (hints for parser, parser gives back binary (TODO = figure out data structure) with types)
- not require or care about indentation (like C)

```
type "float3" = {x:float y:float z:float};
# shorter
type "float3" = {x, y, z:float };
# alternative
key "float3" = { x, y, z:float };

# alternative (no spaces, without `;`)
key"float3"={x,y,z:float}

# shortest i could think of
"float3"={x,y,z:float}

"info" = {
    "player" = {
        "pos" = float3{10, 10, 10}, <- do we really need the comma `,`?
        "rot" = float3{10, 10, 10},
        "basis" = {
            "right" = float3{1,0,0}, <- basis vector
            "up" = float3{0,1,0},
        }
    }
}

idea -> attributes. Use `()` for attributes

useful for the parser to return a specific data structure? telling an archetype apart from something else?... nvm, this is a bad idea, this is essentially another way of telling a type :/
- as a result of this I figured that..
    - we should provide a way of defining a data strucutre so the parser knows what data structure to give back?
    - or maybe... the data strucutre is being turned into json, so just use type hints for converting back into the data structure?

more Database ECS styled?

# attribute using parenthesis `()`?
"archetype1"(archetype) = 
{
    # 2d array using square brackets `[]`?
    "positions"[2, 4] = 
    {
        {
            float3{0,0,0}, float3{0,0,0}, float3{0,0,0}, float3{0,0,0}, 
        },
        {
            float3{0,0,0}, float3{0,0,0}, float3{0,0,0}, float3{0,0,0}, 
        }
    },
    # or without telling size of array + type hinting before hand?
    "positions"[,]:float3 = 
    {
        {
            {0,0,0}
        },
        {
            {0,0,0}, {0,0,0}, {0,0,0}, {0,0,0}, {0,0,0}, 
        }
    }

    # or with inline type?
    "positions"[,]:{x,y,z:float} = 
    {
        {
            {0,0,0}
        },
        {
            {0,0,0}, {0,0,0}, {0,0,0}, {0,0,0}, {0,0,0}, 
        }
    }

    # struct of float arrays (instead of array of float3 structs)
    "positions"[3,]:float = 
    {
        {0,1,0.34,0}, <- X
        {0,3,4   ,0}, <- Y
        {1,2,4   ,4}  <- Z
    }
}

what about telling the parser before hand that the following will be like a 2D array (or 3D or 4D array) == faster? (will it be faster? rather than guessing / not knowing before hand?) Also telling the size of the array (before hand) == faster?


This is format is obviously not looking *simple*. The idea is to push this to an extreme, watch it explode, then build a btter solution from what we learned.


Only basic types: (shorter = faster parsing + more compact)
- i16
- i32
- i64
- f32 (float)
- f64 (double)
- "" = string or key
- {} = struct or object or array

arrays are denoted by `"key"[]`

we put a comma to dneote another dimenstion in the array, for example `[,]` is a 2d array, wjhile `[,,]` is a 3d array, and `[,,,]` is a 4d array.

we don't use the square brackets `[]` around an array! We use {} around the items in an array.

TODO: the only primitive data structures
- use `[]` for arrays!
- use `{}` for structs, but also for objects?

CURRENT FORMAT:
"key":type/hint/attribute = {} or []

EXAMPLE:
"players":archetype = 
{
    "positions":[]float3 = 
    [
        {10, 1, 2},
        {3, 4, 2},
        {1, 2, 4}
    ],

    # alt, struct of arrays (notice the "float3[]" vs "[]float3" the order we put them in matters!) #
    "positions":float3[] =
    {
        [0, 0, 1], # x #
        [1, 0, 3], # y #
        [1, 2, 3] # z #
    }
}

reuse previous data structres? link them together?

EXAMPLE:

"players":archetype = 
{
    # archetype info for all player entities?
}
"enemeies":archetype =
{

}

"world" = 
{
    # links to other predefined data structures, using referential key name?
    "players":link = "players",
    "enemies":link = "enemies"
}

The goal is for the above to translate directly to an in memory data structure, passed to you by the parser

TODO
- translate types from json back into programming languages types? How will the programer know the type we are giving them? Should the programmer pre-define the types (and their "text" based names?) so that the parser can know how to return the json types?
NOTE: the above is not actually json I am just calling it that. Even if it never translates to real world use case I will continue to use this to describe my data structures


IDEA: alternative possible hints

"players":archetype/gameobject =
{
    "components":[]component
}

remember {} = struct

IDEA: inheritance through wrapping? How to translate to binary?

Unknown type length (in bytes) can be solved through extra struct with unsigned long to tell the length

struct {
    unsigned long size;
    void* data; // pointer to the start of the data ("void*" is a pointer to an unknown type)
}

Now solve the inheritance for components.

# define component parent type
"component" = 
{
    unsigned long size;
    void* data;
}


NeVerMind: trying an ECS style approach rather than gameobjects, pointers are terrible! I can't define where a pointer will be in a text file data format! So i resorted to using an index into an array os components of that specific type. Still have the problem of accessing the component arrays through something (the problem being I can't hold an array of arrays, each sub array being of a different type... oh wait I just showed the solution above... oh right, i forgot that won't work... :P)

"position":[3]float = def; # defining not setting?

"players":archetype/gameobject =
{
    "components":[]component =
    [
        {
            size = 32 * 3
            data:int = 1212 <- lookup table index to "positions" array
        }
    ]
}

"positions":[]positions = 
[
    [0, 0, 0]
]

TRYING A DIFFERENT FORMAT:

"entities":[,]int =
[
    # format = [archetype, component index, component index, component index]
    [0, 1] # entity number 1
]

# what component array to look at (aka what type of component), this is not the index into the component array
"archetype1":[]int = [0, 1, 2]

# linked list of all components
"components":[]component =
[
    {
        # sizeof float3
        type_size:long = 4 * 3,
        # array of float3 structs
        component_array =
        [
            {0, 0, 0}, {2, 2, 4}
        ]
    }
]
```