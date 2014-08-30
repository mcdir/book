
## 2. b2/Cafelog

Just over a year before Matt and Mike took to the internet, in a small apartment above a bar in Corsica, Michel Valdrighi wrote a blog post. The self-titled "only blogger in Corsica" used a creaking dial-up AOL connection that disconnected every thirty minutes. He shared his apartment with his cats, No Name and Gribouille, who perched on a windowsill that looked out over a high drop and [whose antics he captured on his blog](http://zengun.org/weblog/archives/2000/12/post1447/). Like many bloggers, Michel captured minor incidents in his life, using his blog to write about not only his cats, but his job, his colleagues, technology, and neopets.

Like many bloggers before him, he had experimented with different web publishing platforms - he started out with HTML before moving on to Blogger. And, like many bloggers, he found the Blogger wasn’t as full-functioned as he wanted. It didn’t have a built-in comment system, for example. Michel signed up for two different commenting services, both of which disappeared along with all of the comments and discussions on his blog. Blogger was also plagued by stability issues. A favorite joke amongst bloggers was that Blogger was “sometimes up. 

At that time, Michel was learning PHP, both in his spare time and in his job. PHP is a server side scripting language: it is used to retrieve information from a database and display it in a browser. Unlike a language like Perl, PHP is relatively easy to learn, making it a useful tool for people who want to start hacking about on some software. One of Michel’s first PHP projects was a dictionary for the preservation of the Corsican language: this experience taught him that he could use PHP to manipulate data, inspiring him to build his own blogging script. Iin June 2001, [Michel started development of b2](http://zengun.org/weblog/archives/2001/06/post1958/)[^fn-1], a "PHP+MySQL alternative to Blogger and Greymatter." He wrote:

> Not much new ideas in it, but it will feature stuff like a built-in comment system, good users management (with complete profile etc), user-avatars (got piccies ?), multiple ways of archiving your blog (even post by post if you like to do a kind of journal) (SIC).

> The installation will be easy, just edit a config file, upload everything and launch the install script. And there you go, but you’d like an admin control panel? It will be there, packed with options.

The PHP and MySQL combination was a good alternative to other contemporary blogging platforms. When a person visits a PHP/MySQL website, the script runs and the PHP retrieves information from the database. A platform like Movable Type rebuilt the page every time someone left a comment or edited the page, making for slow page-load times. b2 was touted as an easy-to-use, speedy weblogging tool. "You type something and hit "blog this" and in the next second it's on your page(s)," [reads the sidebar of cafelog.com](http://cafelog.com/). It goes on, "Pages are generated dynamically from the MySQL database, so no clumsy 'rebuilding' is involved. It also means faster search/display capabilities, and the ability to serve your news in different 'templates' without any hassle." 

These features were part of the reason that Matt, Mike, and so many other bloggers used the software. But Michel admits to being novice developer, learning PHP and MySQL while building the precursor to one of the most widely-used blogging and CMS platforms in use today. He [recalls now](http://wordpress.tv/2012/02/27/les-origines-de-wordpress-la-naissance-de-b2cafelog/) that as a fledgling PHP coder he didn’t always do things the right way:

> When you look at WordPress's code and think 'Wow, that's weird, why did they do that this way?', well often that's because they kept doing things the way they were done in b2, and I sucked at PHP.

Michel started out by scratching his own itch. “Scratching your own itch”, is a phrase often thrown around in FOSS development. It means to create software that solves a problem for yourself. In his book, _The Cathedral and the Bazaar_, Eric Raymond [writes that](http://www.catb.org/esr/writings/homesteading/cathedral-bazaar/ar01s02.html) “Every good work of software starts by scratching a developer's personal itch.”

Michel’s focus was on creating a blogging tool, as opposed to a CMS. The early b2 features reflect the aim of creating a frictionless way for people to blog. Early enhancements made writing easier. [AutoBR](http://cafelog.com/index.php?p=19&c=1), was added, for example, to add a <br/> tag every time a writer hits enter to create a new line. Other early features include, an option that allows users to [set their own timezone](http://cafelog.com/index.php?p=22&c=1), [a basic templating system](http://cafelog.com/index.php?p=24&c=1), an [options](http://cafelog.com/index.php?p=39&c=1) page, [archives](http://cafelog.com/index.php?p=45&c=1), and [comments](http://cafelog.com/index.php?p=46&c=1).

Michel was concerned with making b2 as usable as possible for everyone, whether they be an experienced developer or a writer with little technical experience who just wanted to publish their content online. In a an early version of UX personas, he [writes about “Joe Newbie”](http://cafelog.com/index.php?p=30&c=1), a fictional figure who should be able to easily publish their blog. This ideal of making software easy for anyone to use permeated the b2 community and would eventually become a core ideal in WordPress’ own philosophy.

By the end of June 2001, Michel was [ready to say goodbye to Blogger](http://zengun.org/weblog/archives/2001/06/post1909/), and move his blog to b2. It was the first website to run on the code that would become WordPress, grandfather to millions of websites and blogs. He set up a website, and, a few days after migrating his own blog, [he released the first version of b2](http://cafelog.com/index.php?p=60&c=1). It didn’t take others long to follow suit: a few days later [a second site was running b2](http://zengun.org/weblog/archives/2001/07/post270/), the [personal weblog of a schoolboy called Russell](http://web.archive.org/web/20020718211541/http://russell.bustakartoon.com/).

Cafelog.com was a gathering place for a fledgling b2 community. Michel allowed people to register for the blog and once he trusted them, he would enhance their privileges, allowing them to post on the blog and even become admins. Their first posts usually involved a "Woo hoo" and a [plug for their own website](http://cafelog.com/index.php?p=21&c=1). These sorts of "[shameless plugs](http://www.cafelog.com/index.php?p=29&c=1)" were often the only posts that people actually made on the blog, a useful trick for getting some linkback love and traffic to their personal blog.

Development didn’t always go smoothly, although solving problems would lead to refinements in the platform. Brigitte Eaton, who ran a site called [Eatonweb](http://portal.eatonweb.com/), was the first prominent b2 user. Eatonweb is a hand-maintained list of blogs, which was a go-to place for discovering new blogs until the number of blogs exploded and hand maintaining a list became untenable. Hand-maintained link lists were eventually superseded by the ubiquitous blogroll and services like Technorati which started ranking blogs according to incoming links. Brigitte Eaton wrote a lot of content, publishing to her blog regularly. When she imported her blog into b2 she found that the more posts she added, the slower the blog got. At that time, Michel did not know how to write code for retrieving months from the archives. His code parsed through every post on the blog to query whether the post had changed and then display it. For blogs with large amounts of posts, this meant a huge workload on the server, quickly slowing down the website.

Although b2 did not have an establish developer infrastructure, it was open for contributions. The first major code contribution to the project was [pingback functionality](http://cafelog.com/index.php?p=490&c=1), from a developer called [Axis Thoreau](http://web.archive.org/web/20020921055340/http://mort.mine.nu:8080/b2/), who went by the handle Mort. [^fn-2] Similar linkback functionality, called trackback, was included in Movable Type. Michel had included a version of this in b2. He [used the introduction](http://zengun.org/weblog/archives/2002/08/trackback-in-b2/) to trackback on the Movable Type website, and looked at the Perl code to see the data that was being passed to the trackback URL. Trackback is a ping sent from the original author’s site to a site they’ve written about, when a hyperlink is included. Unlike pingbacks, trackbacks are manual so the original author has to choose to send the trackback, and can edit the excerpt sent. Trackbacks are much more susceptible to spam than pingbacks. Spam pings are pings sent from spam blogs to get links on other websites. Whereas pingbacks ping back to the original site to verify that it is not spam, the same checks are not carried out by trackback.

As b2 expanded, the community followed suit. b2 largely remained Michel’s pet project but there was a community of users and developers on the forums. The forums became a haven for people asking for help with the software. The most popular were the installation, templating, and how to discussion forums, but there were also forums just for general chatter about the software and about blogging. Developers helped each other out with hacks for b2, and it was on the b2 forums that the early WordPress developers had their first interactions.



Outside the b2 community, the software came in for criticism. Michel's lack of coding experience showed, especially to experienced developers. One blogger, Jim Reverend, wrote a post titled ["Cafelog: A Look at Bad Code"](http://revjim.net/2002/12/21/cafelog-a-look-at-bad-code/). In it Jim bemoans poor code quality in publicly released software, particularly b2. He criticizes the software for both its lack of features [^fn-3] and its poor coding practices. 

Michel's lack of PHP experience meant that he wrote inefficient code and used techniques counter-intuitive to a more experienced coder. Michel's code was that of a developer learning PHP. Rather than taking a modular approach to solve a logic problem, the code grew organically, written as Michel thought about it. Code wasn't so much a tool to solve a problem, but a tool to get the newest feature on the screen. This created multiple code interdependencies which could cause problems for developers new to the project. A line of code would change, and break something that appeared unrelated. For Reverend, this type of "dirty code" was unforgivable; "What I do have a problem with," he writes, "is my inability to use his code (without extensive reading and rewriting) to implement my own features." A cornerstone of open source software is to write extensible code. If code is written in a stream-of-consciousness fashion, lacking in best practices, it can be difficult for other developers to extend.

It wasn't all bad, and in the context of WordPress the code quality could even be seen as a benefit. In a follow-up article, [Reverend concedes](http://revjim.net/2003/01/03/cafelog-a-few-more-thoughts/) that there are some benefits to such poorly written code:

> While programmers like myself start convulsing when we have to wade through such code, less experienced programmers actually like it, because it is easier for them to work with. Because the "template functions" are in the global namespace, they work anywhere. Because the data returned by the database is in a global variable, you don’t have to use any tricks to get at it. It makes extending, enhancing, and modifying the code easier for newbies.

Michel's inexperience gave the code a level of simplicity that made it easy for other novice developers to understand. Whereas a more experienced developer might write complex code, Michel would take the simplest route to solve a problem. "In a way it was beautiful because it was so simple," says developer Alex King, [alexkingorg](http://profiles.wordpress.org/alexkingorg/), "It wasn't elegant but it was very straightforward and very accessible. For someone who didn't have a lot of development experience coming in - like me - it was very comfortable understanding what was going on."


The article also highlights another important aspect - people liked using b2. It allowed them to publish to their blog without any hassle. "If you are a user of this product," writes Reverend, "please don’t tell me about how cool it is, or about how well it works. If you read a site powered by this engine, please don’t tell me about how easy you find it to use."
 But people did find it easy to use. To users it didn't matter what was going on under the hood. It may have had its problems but it was a frictionless way of getting content online. Where users went, developers followed; even better if those users were novice developers themselves, fumbling round at the edges of PHP, learning what they could do with code, what new functionality they could add to their website, and share with other users. Even in these very early days, b2's development demonstrated the schism between developer-focused development and user-focused development. On the one hand a focus on logical, beautifully written code, on the other a focus on features that users wanted.

___


The software was distributed, but it took some time before Michel decided which license to distribute it with. He spent a lot of time prevaricating over his choice of license. The free software movement was relatively young and many large projects had their own license terms (such as Apache, PHP, X.Org). Michel felt that until he chose a license he would distribute it with his copyright. 

On the b2 blog, it's possible to follow the progress of the appearance of the GPL in b2. In August 2001, Michel made a brief statement on cafelog.com, telling people that they could use his code provided he was given credit for it, stating explicitly that "b2 isn't released under the GPL yet." People were starting to take notice of b2 and within a few months they were passing it off as their own. In October, a Norwegian agency claimed to own the copyright to b2 and Michel was forced to contact the Norwegian copyright agency. In the discussion around this incident, Michel made a statement that came as close to a license as he'd got so far:

> You can use b2 for free, even if your site is of commercial nature. You're welcomed to buy me items from my Amazon.com wishlist if you're going to make much money from your b2-powered site or if you just like b2.

> You can edit b2's source code.

> You can re-distribute a modified or original version of b2. In no way your modifications make you author or co-author of the modified version, I'll remain b2's sole author and copyright holder.

> Any help is welcomed. Feel free to submit fixes and enhancements, they might get in b2's code and your name or email address will be there as credit in the source code.

> I guess this makes a b2 license for now.

b2 continued to be released under this slapdash license until Michel realised that b2 needed an official license so he started looking in earnest. It was important to Michel that b2 remain free, even if he stopped working on the project himself, or if someone else took the code and used it for their own project, so he rejected the MIT/BSD licenses and their derivatives. The PHP license was a BSD derivative which he also rejected because it had clauses saying that redistribution had to include an acknowledgement of the original project. He recalls now that "at the end of that elimination process, GPL remained. It helped that there were already some projects using it, as I didn't want the code to end up abandoned and forgotten because of the choice of an exotic license." 




 Michel's choice of license was prescient. With a GPL license, a piece of software can be forked, modified, and redistributed. In FOSS projects, this doesn’t happen regularly, but it can save software from disappearing completely if development stops. This is what happened with b2.

All was going well until May 2002 when [Michel lost his job](http://zengun.org/weblog/archives/2002/05/jobless/). In the months following, he continued to keep up development on b2, but he [struggled with depression and health issues](http://zengun.org/weblog/archives/2002/08/back/), had his [electricity cut off](http://zengun.org/weblog/archives/2002/08/they-cut-my-arms/), [moved house](http://zengun.org/weblog/archives/2002/08/its-that-time-of-the-year-again/), and [struggled to find a job](http://zengun.org/weblog/archives/2002/10/untidy/). With so much going on his life, Michel eventually disappeared. He [posted about spam in December 2002](http://zengun.org/weblog/archives/2002/12/spam-the-blogosphere/) and didn’t post on his personal blog throughout 2004.

The users of b2 were without a lead developer. There was no one steering the project, making fixes, or adding new features. People were concerned about Michel - they liked him and were worried about what had happened to him. In March 2003, a [discussion thread started on cafelog.com](http://cafelog.com/index.php?p=499&c=1), asking about Michel’s whereabouts. Michel’s sister, Senia, posted that he was well and that he was looking for a job. She promised to ask him to connect to IRC and MSN. The responses to Senia were mixed.

One commenter said:

> Please pass on to Michel that not only has he created a really nice piece of software, but he has also inadvertently built a community […] of people, a sort of commonwealth on the blogosphere. I don't know him the slightest bit, but I wish him well and hope that any soul searching or vision quest (or vision exodus?!) he has embarked on helps him find what he needs. Yet also allows him to tie up any loose ends that he leaves behind.

Others had concerns about their own projects:

> Anyone heard from Michel yet? His last post was 6 weeks ago. I want to install and promote b2 in two projects (one affiliated with a UN women's project).. but I am nervous about doing so if there will be no developer support available. I am sure he knows that b2 is including in the Fantastico auto-installer bundled with the cPanel virtual hosting tool. I want to write an blogging article for hosting clients. Michel? You going to be around?

Michel never went back to b2 with the same gusto with which he had started and eventually the stagnation of the software made it unusable. But the GPL license meant that neither the code nor the community had to disappear. Developers, familiar names from the b2 community forums, forked the software. While b2 itself did not continue, it was the platform that connected Mike and Matt, and the software that would provide the groundwork for the new WordPress platform. With its simple PHP and focus on usability and ease of use, b2 contained the incipient ideals that would be at the heart of WordPress. But first, the software had to be forked, and, as bloggers are wont to do, they took to their blogs to do it.


[^fn-1] The name b2 is a combination of the word “blog” and “Song 2” by the British band Blur, which Michel was listening to on repeat. He combined them to make “blog2”, then “blogger2”, until he got to b2. b2 also was known as Cafelog, which was the name Michel planned to give to the 1.0 series. There were no b2 domains available, and the name was too short for a project on Sourceforge.

[^fn-2]Pingback is a linkback method which authors use to request notifications when someone links to their website. An author writes a post on their blog that links to a post elsewhere. The original site sends a XML-RPC request and when the mentioned site receives the notification signal, it goes back to the original site to check for the link. If it exists then the pingback is recorded. A blogging system can then automatically publish a list of links in the comment section of the post, or wherever the developer wants to place it.

[^fn-3] Particular problems that the article calls out are: that b2  didn't cache calls to the database so when there was a new visit from a user, the page had to be loaded from the database and server, slowing down the website. Also the lack of flexibility in the templating system and the lack of cruft-free URLS (known in WordPress lingo now as "pretty permalinks"). 