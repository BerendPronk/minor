# 5 Levels of Ignorance in Modern Web Development
Despite the fact of me not being a professional web developer yet, I do have a fair share of knowledge on the topic. In this article, I want to mention the annoyance of sophisticated web developers — about what they know — compared to the ignorance of the new and unexperienced.  
Please do not be offended by any of the claims I make. My intentions are just to inform you with topics that need improvement.

## Design — Don't follow the rules
I myself am a graduated graphic designer that progressively made a turn towards web development, with web design being a main focus.  
One thing that drew my attention when entering this business, is the amount of rules that so called 'web designers' apply when producing a styleguide, architecture or layout. Design isn't something one can be taught, it must be learned via experience in the field, by learning from your own mistakes.

When a set of rules is applied (i.e. a maximum allowed width of paragraphs, or that every colour contrast must exceed a 4.5-rating on [Lea Verou's Constrast Ratio Check](http://leaverou.github.io/contrast-ratio/)) the designer isn't left with much freedom. Sure, there are times where a maximum paragraph width is needed and where a high contrast is existential, but it depends very much on the context the designer is given per objective.

## (JavaScript) Frameworks — Redundancy achieved 
Starting developers immediately want to get to the good stuff when making web applications, meaning they will set their focus to choosing a framework or library that's suitable for development. Most of the work will be handled by the chosen bundle of code, this way. Though this approach seems quite reasonable, however, it's not. By assigning tasks to a third party framework/library, the developer is not really paying attention on the stuff he/she is creating. Sooner or later this will cause troubles, in which the developer doesn't know how to proceed or fix even the most basic thing.

It's far better for starting developers to learn vanilla JavaScript, to eventually reach a point where he/she doesn't even consider using a framework/library, because it's contextually more efficient to use less code for the job in question. There will never be a usecase where the entirety of the framework/library will be used.  
Whether the developer called to focus on an object-oriented or a functional approach, vanilla code is more efficient, effective and scalable per case. This especially applies in the long run, where maintenance issues a decade later can be resolved more quickly with vanilla code compared to framework/library code.

*"If you can't do it without tools, you're not a web developer."* (Peter Paul Koch, 2017).

## Performance — Every millisecond counts
With the introduction of fiber networks and the new 4G mobile standard, one should expect that the overall internet speed is exponentially increased, and it is, though not everywhere. It's a common misconception that speedy internet is the norm around the globe, or even thirty minutes from my hometown; one that I personally fell for as well.  
Fiber networks are not integrated fully, yet. As of 2016, only 11% of the total percentage of bandwidth subscriptions in the United States were from fiber networks (Felix Richter, 2016). With mobile devices, the same can be applied: Not everyone has the opportunity to enjoy the speed that comes with a 4G network, some have to browse with 3G or even 2G connections. Even some (public) Wi-Fi networks can perform poorly.

Every developer should keep performance in mind. It doesn't necessarily have to be the top priority at the kick-off, but it's nice to consider doing so anyway. Procrastinating on tasks like this mean the problems stack up while the project is getting bigger and bigger.  
Really, a developer who's not paying attention to performance could result in a company's downfall, since the expected amount of customers can drop when people decide to close the website before it finished loading.

## Accessibility — Countless disabilities
Another major part of development, besides performance, is accessibility; to think about all the possible users a website/application will have. And I don't mean different genders or age groups, but the differences in the capabilities they have, or rather, what kind of disabilities they share. I can assure you it's a lot; too many, in fact, to name them all.

Naming all disabilities is not important, though it is necessary to mention that all of the people who are unfortunate enough to deal with one, should be able to use the website/application as intended. This translates to blind users being able to listen to the content, images included, and users navigating with the TAB key to be able to reach every nook and corner of the website/application.

The W3C conducted special guidlines, called: The Web Content Accessibility Guidelines (WCAG), and the second installment of these guidelines was officially announced in december of 2008 (W3C, 2008). The main guidelines are as follows:

- **Principle 1:** Perceivable - Information and user interface components must be presentable to users in ways they can perceive.

- **Principle 2:** Operable - User interface components and navigation must be operable.

- **Principle 3:** Understandable - Information and the operation of user interface must be understandable.

- **Principle 4:** Robust - Content must be robust enough that it can be interpreted reliably by a wide variety of user agents, including assistive technologies.

A full list of the WCAG 2.0 guidelines can be found on the [W3C website](https://www.w3.org/TR/WCAG/#guidelines).

## Progressive Enhancement — Not everyone runs the latest software 
With the disabled and impatient tackled, all user experience flaws a website/application can have should be solved, right? No, unfortunately there is another principle developers need to acknowledge: Users with outdated software, mainly webbrowsers. The innovations in web technology come and go as we speak, some of which are very nifty to be used in a developer's next project. But these new technologies are only supported by the newest browser versions, if one is lucky.  
Browser developers continuously race against these innovations to keep up with the demand of the public and to stay ahead of their competition. Though it is good to see that they are innovating and are not falling behind, in contrast to the older browsers around.

A lot of internet users put little to no effort in keeping their browsers up to date. Modern web browsers update automatically, but this wasn't the case with many of the mainstream browsers, like Internet Explorer, unfortunately. And because Microsoft, since the dawn of the web, has dominated the PC market, a lot of people use their default web browser Internet Explorer.  
It's good to see that the tables have turned, and that the majority of users upgraded to a automatic-updating browser like Chrome, which is approaching the 60% of the total market share, as of May 2017 (Netmarketshare.com, 2017).

Despite the rise in browser upgrades, many people still use outdated browsers as their default. They withhold on the great features the web has to offer. Some would say they are ignorant, and that it's their own fault if they do miss out. But that should not be the case. These users need to be able to experience websites/applications as they're inteded to. While certain interactions may recede, the content should be reachable in any way.  
This all means that developers should progressively enhance the application, keeping their entire group of users in mind at all costs. Maybe some day this will be an obsolete problem, but untill then, developers are obliged to translate a design in a usable product for every browser.

## Resources
Lea Verou. (2012). *Contrast Ratio*.  
http://leaverou.github.io/contrast-ratio

Peter Paul Koch. (2017). *Choosing the web's future*.  
https://quirksmode.org/presentations/Spring2017/goingwrong_vanlanschot.pdf

Felix Richter. (2016). *The U.S. Lags Behind in Fiber Adoption*.  
https://www.statista.com/chart/4392/fiber-adoption-in-oecd-countries/

W3C. (2008). *W3C Web Standard Defines Accessibility for Next Generation Web*.  
https://www.w3.org/2008/12/wcag20-pressrelease.html

Netmarketshare.com. (2017). *Desktop Top Browser Share Trend*.  
https://www.netmarketshare.com/
