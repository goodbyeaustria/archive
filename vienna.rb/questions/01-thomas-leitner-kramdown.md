Welcome to the Q&A series. 

Today let's welcome Thomas Leitner. 
Thomas is the head of the computer group of the mathematics department 
of the University of Vienna (in Austria, Central Europe) 
and better known as the author of the kramdown library and tool - a fast, markdown-superset processor (in ruby) 
for converting plain old vanilla text into hypertext (powering GitHub Pages, Jekyll, and friends).


**Q: Can you tell us a little bit about yourself? How did you get started with Ruby?**

A: Ever since my parents got a computer when I was in middle school I was
fascinated by it. As this was pre-Internet (at least at the beginning)
I learned by watching my older brother use it and got the hang of it
quite fast.

The most interesting thing was programming which developed into one of
my favorite hobbies. First I used Basic and Pascal, later Delphi and in
2001 while studying Software Engineering I found Ruby and quickly fell
in love with it.

Though not perfect, Ruby is nearly perfect, at least for me, and all
the programming I do in my spare time is in Ruby nowadays.


**Q: Do you remember - how did you find out / get started with markdown?
Did you try out any alternatives e.g. textile, wiki text, etc.?**

A: I was creating a static website generator, webgen, back in 2003 and
didn't want to write the content in HTML. At first I used plain HTML
but later I discovered Textile and used it as main way for writing the
content.

However, I discovered Markdown and the Maruku library soon afterwards
and it seemed a much better language for the purpose than Textile. So
Textile was demoted and Markdown took the place as default markup
language.

**Q: How (and why) did you get started / end up writing your own
markdown converter, that is, kramdown?**

A: Maruku, the Markdown conversion library written in pure Ruby that I
used for webgen, wasn't maintained anymore and there still were many
bugs to be fixed.

I looked at the source of Maruku but soon decided that I didn't want to
maintain it because it wasn't easy to update or extend.

However, I really liked the additional features that Maruku brought to
the Markdown world (like inline attribute lists) and therefore did what
every hacker would do: Implement his/her own solution since no other
Ruby library had the same feature set.

So I started to lay out a simple, non-formal specification of what
kramdown should do for various elements and began implementing it. Once
I had the most important elements and the basic thing running, I put
the code on Github and released it.


**Q: Can you tell us some challenges you faced writing kramdown?**

A: Since Markdown doesn't have a real, formal specification, I had to pick
and choose features and edge case implementations from the available
libraries. And it wasn't always easy to decide what to use and what not
to use, and sometimes I implemented a certain feature in a completely
different way when it seemed the better solution.

Another challenge is that when you program in Ruby it is easy to
implement things in an ingenious way, like using meta programming and
such. However, after you program a long time in Ruby you realize that
most of the time you are better off avoiding these solutions.

**Q: Do you have any favorite markdown extensions e.g. todo
lists, meta data, emojis, auto links, etc. - or worst?**

A: My favorite extension to the original Markdown are the inline attribute
lists. These allow you to specify any attribute on any element, with
special shortcuts for classes and IDs.

This was also the reason why I really wanted to use Maruku instead of
other libraries such as BlueCloth, and the main reason why kramdown
came to be.


**Q: Any thoughts on adding / getting multi-line tables working in
kramdown - works great in wiki text e.g. wikipedia or something ;-) ?**


A: Maybe in version 2.0 but one of the goals of Markdown is that it should
be easy to read and write. So if a syntax doesn't feel to be Markdown-y
I probably won't include it.


**Q: What's next for kramdown? Any plans for 2.0?**

A: I consider kramdown a mature and stable library. If you read the
release announcements you will find that there have been regular
improvements and bug fixes but nothing really major. And I think that
is good for kramdown's users because they can depend on it and the
versioning scheme.

As for 2.0: Since this is a major release there will be breaking
changes, not just in the internal structure (I will probably remove
some of the meta programming stuff) but also in the syntax.

One thing that is sure to change is the current table syntax. Support
for strikethrough and superscripts/subscripts will also probably be
incorporated.

However, there is no date set for when 2.0 will be released or even
worked on. This depends on the amount of spare time I can dedicate to
the development of kramdown.

</>

Thanks for your time and answers and - of course - thanks for the great kramdown library and tools!


Links / References:

_kramdown & webgen_

- [kramdown Project](http://kramdown.gettalong.org) by Thomas Leitner - a fast markdown-superset converter in ruby (without any c-extensions)
- [Using Markdown with the kramdown Library and Tools](http://talks.gettalong.org/2016-02-vienna-html) by Thomas Leitner - talk slides (in HTML) from the Vienna.html meetup on Feb/23rd, 2016
- [webgen Project](http://webgen.gettalong.org) by Thomas Leitner - a static (web)site builder / generator in ruby

_Markdown_

- [Learn Markdown in 60 Seconds @ CommonMark](http://commonmark.org/help)
- [Learn Markdown in 10 Minutes (Tutorial) @ CommonMark](http://commonmark.org/help/tutorial)

_Textile_

- [Textile Project](https://github.com/textile) - another plain text-style markup language
- [Textile Article @ Wikipedia](https://en.wikipedia.org/wiki/Textile_(markup_language))

_Miscellaneous_

- ["Old" Maruku Project @ RubyForge](http://maruku.rubyforge.org) - a markdown-superset interpreter in ruby with inline attribute lists, tables, etc.
- ["Old" BlueCloth Project](http://deveiate.org/projects/BlueCloth) - the first markdown library for ruby (started as a direct port of the Markdown.pl script in perl)
