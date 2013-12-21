Experimental ways to use the Scribus code

As I have announced at the end of the last year, in this first half of 2013 I've reduced my participation in the Scribus project to a minimum and I've invested my energy and time into thinking about what the future of publishing may be and what kind of free software should we develop.

It's hard to judge on something that has not happened yet and there is no doubt that I did not have the huge chance to have found the one true and only solution. But thourgh lot of reading and talking to people I think that I've found some key ideas on top of which I hope that I can 

- Nowadays, C++ is not the best language if you want to have a larger community of programmers contributing. It's complex, hard to "meistern" ("master"?) and the employment chances -- outside of the academic world -- are rather thin.
- Qt is a nice framework and it is evolving in a direction that matches our needs. It even makes C++ look like a better language.
- The Web is a nice platform, it's steadely evolving, but it does not look like that it's ready to be the main target for a publishing software. But we have to plan a tight interaction with Web technologies.
- It's important to create modular code, code that is simple to read. People should be able to experiment with it and it should be not too hard to integrate their results in our software.
- The code has to be there where the programmers are. Github is a nice place to store it.
- We need automatic testing and packaging.
- The infrastructure burden has to be reduced to a minimum.
- There is a multitude of sources and of targets (pictures, text, CMS, EPUB, PDF, ...). The software should interact in a flexible way with them. The publishing tool is not anymore the control tower ("swiss guide") that dictactes how the world around it interacts with it.
- The dynamics around the the mobile Apps are another source of inspiration: smaller tools that do one thing and do it well. People using them don't feel stupid, but empowered! What has still to be researched, is a way to get the Apps to share the content with each other.
- In gegensatz to many other communities, we have more than enough brilliant people wanting to take care of the UI and the user interaction, but we have way too few programmers wanting / being able to write code for Scribus.

And now that I've recognized this, what should I do?

I want to work on some experimental tools, starting with the the Scribus code and trying to glue things together.

The first step will be to take the Scribus code and pull out the relevant code to create a tool that converts .SLA files into PDFs from the command line and then extend it to also create EPUB files.

In parallel, I would like to try out the new QT Quick framework to create an interface for creating profiles that can be used for the PDF and EPUB export.

Then, there are some other tasks that I'd like to see realized and that you could help create:
- Setup a testing framework.
- Defining a new file format, an alternative to SLA that is easier to work with, to share, to check and to transform.
- Integrating the scripter engine (or another was to get commands executed on the files)

Everybody who wants to experiment with the ideas presented in this email (and other) is welcome to join!
