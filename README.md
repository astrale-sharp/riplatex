# What is this project?
Welcome to riplatex, a delightful language to make beautiful documents (pdf). 

# Why this project?
Picture the scene, you're a teacher and you have to craft beautiful documents to your students so they will
be happy and think you're a good teacher.

You might stumble upon the few different free software out there that tackle that problem.
- Libreoffice ? This is nice enough, but making beautiful documents is very time consuming,
you might need to solve the same problems over and over again.
- Inkscape ? The resulting documents are  absolutely beautiful but you have to edit one page at a time
and there is no support whatsoever to make multiple pdf pages at once (that I am aware of) plus the text support
is not magical right now.
- Latex ? Latex makes a lot of promises that are very good to hear, separation of the layout logic and the content (see ../separation_layout_content.md for details), the power of a full programming language, beautiful math support (which it delivers). That being said.. working with latex can be quite challenging and frustrating.. So much so that it makes sense to develop a new programming language entirely, [more on that below](#why-the-name?)

Inspired by rust and elm, riplatex aims to provide the definite solution for making beautiful pdf documents. For this it needs to be :
- Delightful : 
    - beautiful and helpful error messages
    - IDE friendly, autocompletion should just work
    - Easy to read, easy to write : the code should describe the document wanted and there should be no surprises
    - Fearless to refactor/ toy with
- Easily extensible: 
    - It should be easy and painless to build on top of a library already made,
    without risks of weird bugs and so on.
    - When you find a library, the documentation should contain multiple simple example that illustrate 
    how you should use the library and are **guaranteed to compile!**. 
- Powerful and expressive: It should be easy to write logic, layout contents and have good results.
- Minimal, Simple so it is advanced fast to a working point and a community can be happy, hyped and make the most useful package and the most delightful documents.
- Sensible default.
- If it compiles on your machine, it should compile on every machine.
- Battery included (a binary that takes care of package import, organizing src/, formatting, compiling etc )
It makes a lot of sense to me that riplatex needs to be strongly typed and fully functional.



# How far done?
Not far at all, I haven't written a single line of code yet!
It's my first big project with lot of ambition so don't expect anything soon!

# Why the name?
Latex can be.. quite frustrating to learn... A lot of example out there simply won't compile with your latex compiler
or on your computer and you won't know why.
Every time you set out to use a new package, the documentation is rarely easy to understand, when it contains examples they often won't compile.
It is not possible to know where a variable comes from in latex which makes the IDE experience less than optimal.

It is often possible to write some Latex code that has no meaning but the error message you get can be really hard to understand, even when the fix is easy.

Packages in latex are written in TeX and are very very very hard to read.

That being said, a lot of work has gone into Latex and a heavy number of project wouldn't switch to riplatex
even if it was an attractive alternative, that is okay. I just aim to do something simple on more modern basis 
so new project might be delightful to 

In a lot of ways riplatex aim's to replace latex by being modern, 
delightful and aiming to do the same or better than latex does.

# Contributing
Contributions, ideas and PR's are very welcome in general!

I won't be able to do a project like that on my own!

I am not a native english speaker, do not hesitate to forward PR that correct the sentences of this README.md, it is the most important part of this project!

The project being at a very early stage, there is much reflection going on about the design 
of the future language. You can help by opening issues with your ideas or desires for what a language like that should look like, feel like, the features it should have etc. Ideas of library for the language etc.

Share ideas, research that you find interesting on the subject on the issue side!

When the project is a little more advanced I'll be open to PR's containing actual code as well!