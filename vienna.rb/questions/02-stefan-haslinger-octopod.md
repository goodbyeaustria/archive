Welcome to the Q&A series. 

Today let's welcome Stefan Haslinger - a freelancer and podcaster
from Vienna (in Austria, Central Europe) and author of Octopod - a free jekyll static (web)site builder extension 
(theme and scripts) that lets you publish your own radio shows in minutes.


**Q: Can you tell us a little bit about yourself?**

A: Originally trained as high school teacher in physics and mathematics
I seem to switch jobs roughly every five years. I worked at
the Vienna University of Technology as science collaborator, then high school
teacher, did IT administration and staff training at the local
observatories in Vienna, taught as lecturer at a local college and worked 
at a local stainless steel retailer in their IT-SAP
department. Finally in 2011 I founded my own company where I have been
coding web applications mostly in Ruby on Rails.
If you're interested in details have a glance at my
[curriculum vitae](https://www.informatom.com/cv/) or my [Informatom](https://informatom.com) company website.


**Q: How did you get started with podcasting?**

A: I have been listening to podcasts for ages - I started with «The Linux
Show» probably around 1998 when the term podcast was not even a thing.
I started podcasting in August 2013 with [«Layer
8»](https://layer8.informatom.com/) but didn't keep up for longer
than three episodes.

I really got into podcasting again last year joining the
[«Biertaucher»](http://biertaucher.at) regulars in fall 2015 with their
episode #225 and have stayed with them until now. «Biertaucher» is a
Viennese nerd podcast where everybody is allowed to join in at the public
recording session. We will be recording episode #274 tomorrow so I can
celebrate my fiftiest podcast with them soon.

In March 2016 together with Anna Geiger we started
[«Aua-Uff-Code!»](https://aua-uff-co.de/) - a podcast on coding and
learning to code. We have recorded eleven episodes so far and we are still
digging it!

**Q: Do you remember - how did you find out/ get started with Jekyll?
Did you try out any alternatives static (web) site builders e.g.
Middleman, Nanoc, etc.?**

A: Hm, it has probably been one of your (Gerald!) talks on Jekyll where I
really got interested. Github support drew me in and after I
looked a little bit at Octopress - which seemed to be unmaintained then - and Middleman 
I made my bets on Jekyll.
I had to play also a little bit with Nikola but this was only a side
project where all other folks where dedicated Python people. I did
quite a lot in Python when I was a high school teacher.

**Q: Jekyll and Podcasting - How (and why) did you get started / end up writing your own Jekyll
Podcasting extension (Octopod)?**

A: Well, I haven't written the original Octopod setup and theme. I just picked it up from
Arne Eilermann (aka [@pattex](http://twitter.com/pattex)) in a rather
unmaintained state this spring  when searching for something
to host «Aua-Uff-Code!« with.
I had written a full blown content management system with podcasting support before,
[Mercator](https://github.com/informatom/mercator), that is part of a
guided selling system. But I wanted something more light weight. So I
searched for a Jekyll plugin and found Octopod.
I updated it to use the lasted version of all the components used, added
some more (like the [Bootflat](http://bootflat.github.io/) theme) and
started using it. I changed the code structure a little bit - it
is now a gem with an installer script to make setup a matter of a minute.


**Q: Can you highlight some of the great Octopod features / goodies?**

A: Ha - I'm lazy here and cite our own [Octopod website](https://jekyll-octopod.github.io):

* iTunes-ready paged episode feeds for different file formats (e.g. mp3, ogg, m4a)
* a ready to use Bootflat and Twitter Bootstrap-based, responsive (i.e. mobile friendly) layout modifiable to your heart's desire
* Flattr support on the website and in the episode feed
* Twitter integration on the website
* comments via Disqus
* Podlove Web Player in it’s current version 3.0.
* Static player pages that are embeddable in iframes for your other or affiliates' sites
* Podlove Alternate Feeds
* Podlove Simple Chapters
* Podlove Subscribe Button for easy podcast subscription on any operating system, including mobile phones
* https compatibility
* Google search integration
* Easy show notes creation

Btw., the [Octopod website](https://jekyll-octopod.github.io)
eats its own dogfood - it's a Github Pages site using
Jekyll and Jekyll-Octopod itself.

**Q: Can you tell us some challenges you faced writing / updating Octopod?**

A: I wasn't familiar with Liquid so this was probably the biggest hurdle
as I assumed more similarities between Ruby and Liquid than there are.
Liquid is the templating language used by Jekyll and it should make
things easier for designers (but honestly I think it's the other way
round) and knowing what I know now I'm not sure if I wouldn't start
writing my own plugin but for Middleman because Middleman's templating
language Embeded Ruby (ERB) feels more natural to me (having a Ruby on Rails background).

**Q: How do you handle the upload / sync of the big media files (audio recordings)?**

A: We include a small script that uses Rsync for syncing the files to the
server and I haven't seen any issues with that up to now.
But you do not have to use Rsync - any upload mechanism that you prefer works
fine - just transfer all of the files in the `_site` folder to your
server or web space as you would do it with any other Jekyll site.
Rsync supports delta updates and reconnects on partial uploads but I
don't see a need for them here as podcast episodes once they are
produced typically don't change any more. So regarding them it's really
more an upload and not so much a syncing issue.

**Q: What's next for Octopod? Any plans for the future?**

A: Well, there are - as in any projects - some bugs we have already
identified that need to be fixed.
Regarding new features: Currently Bootstrap and Bootflat are included as
compiled static assets. We have a test setup where we have included
them as SCSS and it works fine so far. That means that
you can tweak the theme using the literally hundreds of configuration
variables of Bootstrap and Bootflat.
This will make tweaking the look and feel of the site quick and easy.

Depending on the future of Flattr we maybe have to support another
crowd funding platform. Patreon seems to get quite a lot of attention
from podcasters currently.

We also need better tagging and categorization support and there are
feature requests on ogg-only sites (currently we need an mp3 asset for
each podcast as well for the Podlove Webplayer) and external audio hosting.
The feed should also be enriched with additional data (e.g an image on
episode level).

**Q: Can you highlight some Podcasts using Octopod?**

A: Besides the two ones mentioned above [«Aua-Uff-Code!»](https://aua-uff-co.de/) 
and [«Layer8»](https://layer8.informatom.com/) I know of
[«Lieblings-Plätzchen»](http://lieblings-plaetzchen.com/) where Jana Wiese
interviews people on their favourite places. (Btw., she is also helping
us a lot finding bugs and suggesting new improvements.)

And there is [«Einmal mit Profis arbeiten»](https://1mpa.chaostreff.at/),
the techno podcast network from Salzburg.

There are probably more because of bug reports and feature requests
from other people, but I don't know their podcasts. Maybe I should
encourage people to tell me about them and put the podcasts on the
website :-) Rubygems speaks of 4000 downloads - so maybe 1% of them is
actually using it?

**Q: Any tips on getting started with Octopod?**

A: Getting started is quite easy as the docs on the Ocotopod site are extensive:
Start with the [first
page](https://jekyll-octopod.github.io/prerequisites/), have your site
running at the third one and get an jekyll-octopod expert yourself
reaching page 11  :-).

**Q: Any else you want to tell the world / our readers?**

A: In case you visit or are already close to Vienna, Austria, you can find
me at the local Ruby groups.

And yes, I would like to pitch my new [Panoptikum](https://www.panoptikum.io) project - it's a brand new
podcast discovery and community site I'm building.

Thanks for having me and keep up the good work!

</>

Thanks for your time and answers and - of course - thanks for the great Octopod theme and scripts!

