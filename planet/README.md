# Planet Vienna.rb

Web feed list and configuration for the [Planet Vienna.rb](http://viennarb.herokuapp.com)
and [Planet Friends of Vienna.rb](http://viennarb.herokuapp.com/viennarbfriends) news website / pages.


---

**Aside - What's a Planet?**

See the [Open Street Maps Blogs](https://blogs.openstreetmap.org) page
as another real world (planet) example
or the [Planet Pluto Documentation](http://feedreader.github.io) that runs (auto-builds/generates) both. 

Or see the talk notes titled "[New Horizons - Build Your Own (Static) Planet News Website w/ Pluto (and Ruby)](https://github.com/geraldb/talks/blob/master/planet.md)".

---



Note: All web feeds including the web feed lists (that is, [viennarb.ini](viennarb.ini) and [viennarb-friends.ini](viennarb-friends.ini))
get auto-updated (fetched) once a day (that is, every 24 hours).


[Vienna.rb Feeds](#viennarb-feeds) •
[Friends of Vienna.rb Feeds](#friends-of-viennarb-feeds) •
[How To Add Your Feed](#how-to-add-your-feed)


## Vienna.rb Web Feeds

- **Vienna.rb News** (web: [vienna-rb.at](http://vienna-rb.at) [:mega:](http://vienna-rb.at/atom.xml))
- **Vienna.rb Meetups** (meetup: [vienna-rb](http://www.meetup.com/vienna-rb) [:mega:](http://www.meetup.com/vienna-rb/events/rss/vienna.rb/))

<!--
  # [viennarbmeetuprsvps]
  #  title = Vienna.rb Meetups RSVPs
  #  link  = http://www.meetup.com/vienna-rb
  #  feed  = http://www.meetup.com/vienna-rb/rsvps/rss/vienna.rb/ 
 -->


### More Ruby Meetups Nearby 

<!--
  #  - www.rubyslava.sk  - no public news blog (no feed)
  #  twitter ->  twitter.com/rubyslava
 -->

- **Rubyslava  - Bratislava.rb Meetups** (lanyrd: [rubyslava](http://lanyrd.com/series/rubyslava) [:mega:](http://lanyrd.com/series/rubyslava/feed/))



## Friends of Vienna.rb Feeds

[Co-Working](#co-working)  • 
[More Meetups](#more-meetups)  • 
[More (Un)Conferences / Camps / etc.](#more-unconferences--camps--etc)  • 
[Companies](#companies)


### Co-Working

- **sektor5 News** (web: [sektor5.at/blog](http://www.sektor5.at/blog/) [:mega:](http://www.sektor5.at/blog/feed/))


### More Meetups

- **Vienna PyLadies Meetup** (meetup: [PyLadies-Vienna](http://www.meetup.com/PyLadies-Vienna) [:mega:](http://www.meetup.com/PyLadies-Vienna/events/rss/PyLadies-Vienna/))
- **Vienna Python Meetup** (meetup: [PYUGAT](http://www.meetup.com/PYUGAT) [:mega:](http://www.meetup.com/PYUGAT/events/rss/PYUGAT/))
- **Vienna Django Meetup** (meetup: [Django-Friends-Vienna](http://www.meetup.com/Django-Friends-Vienna) [:mega:](
http://www.meetup.com/Django-Friends-Vienna/events/rss/Django-Friends-Vienna/))
- **Vienna PHP Meetup** (meetup: [viennaphp](http://www.meetup.com/viennaphp) [:mega:](http://www.meetup.com/viennaphp/events/rss/viennaphp/))


### More (Un)Conferences / Camps / etc.

- **WordCamp Vienna** (web: [vienna.wordcamp.org](http://2015.vienna.wordcamp.org) [:mega:](http://2015.vienna.wordcamp.org/feed/))
- **Linuxwochen Österreich** (web: [linuxwochen.at](http://linuxwochen.at) [:mega:](http://www.linuxwochen.at/atom/)) (FREE)


### Companies

- **Codeship - Continuous Integration 'n' Continuous Deployment** (web: [blog.codeship.io](http://blog.codeship.io) [:mega:](http://blog.codeship.io/feed))


<!--
   "old" feed ids - add/keep - why? why not??

_#viennarb_
_#viennarbmeetup_
 _#rubyslavaevents_
 
 _#sektor5_
 
 _#pyladiesvienna_
 _#pyugat_
 _#djangofriendsvienna_
 _#viennaphp_
 _#viennawordpresscamp_
 _#linuxwochenat_
 _#codeship_
-->


## How To Add Your Web Feed

Step 1: Add your web feed to the web feed list. It's as easy as 1-2-3. 

1. The blog/site title    =>  `**Floor Drees**`
2. The blog/site link     =>  `[1stfloorgraphics.nl/blog](http://www.1stfloorgraphics.nl/blog)`
3. The blog/site web feed =>  `[mega:](http://www.1stfloorgraphics.nl/blog/feed/)`

That's all. All together now in one line:

~~~
- **Floor Drees**  (web: [1stfloorgraphics.nl/blog](http://www.1stfloorgraphics.nl/blog)
                        [mega:](http://www.1stfloorgraphics.nl/blog/feed/))
~~~

Resulting in:

- **Floor Drees**  (web: [1stfloorgraphics.nl/blog](http://www.1stfloorgraphics.nl/blog)
                        [:mega:](http://www.1stfloorgraphics.nl/blog/feed/))


Note: This one line list entry will (auto-)generate a planet configuration entry in [viennarb.ini](viennarb.ini) or [viennarb-friends.ini](viennarb-friends.ini). Example:

~~~
[floor]
  title  = Floor Drees
  link   = http://www.1stfloorgraphics.nl/blog
  feed   = http://www.1stfloorgraphics.nl/blog/feed/
~~~

Step 2: There's no Step 2 ;-)

That's it. Wait for the next auto-update (max. 24 hours). Welcome on Planet Vienna.rb.


## Powered by Pluto

Planet Vienna.rb is powered by the [pluto machinery](https://github.com/feedreader).
