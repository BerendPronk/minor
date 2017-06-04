# Critical Convenience
Unlike what most people think, screen readers are not only used by the blind. People with partial sightness and people with severe forms of autism or dyslexia are in need of a screen reader as well. This increases the amount of users that need assistance when navigating the web. Therefore it's crucial that developers need to know more about the story behind screen readers, and how to build for it in particular.

However, screen readers are not the only piece of medium that should be considered when talking about accessibility on the web. Besides the visually impaired, there are also users of the web with loss of their sense of hearing, or who are having motor impairments and need to use an eye-tracker to make use of the web. Even users with a temporary disability (e.g. a broken arm) are in a desperate need of web accessibility *(The A11y Project, 2011)*.

## History
Using the web is easy, and is becoming easier for everyone, one would say. Though it has not always been that way. As mentioned in the introduction of this article, there is a large audience developers need to set their mind to when creating websites and applications. It's as if this group has been overlooked since the dawn of the web, and something needs to be done about it. Hence the title of this piece: *Critical Convenience*.

The truth is: Accessibility on the web isn't a new principle or guideline. It began to take shape in the early days of the web, in the fall of 1996, roughly five years after the World Wide Web was launched. The idea started with a newsletter from the creator of the web, Tim Berners-Lee, himself:

```
3. Disabilities and the Web  
by Tim Berners-Lee

The emergence of the World Wide Web has made it possible for individuals with appropriate computer and telecommunications equipment to interact as never before. It presents new challenges and new hopes to people with disabilities.

As part of its commitment to realize the full potential of the Web, the Consortium has been promoting a high degree of usability for disabled people, by following the development and encourage an ongoing discussion in the area. This limited involvement has been to host as a catalytic nucleus the disabilities page (linked from our home page). W3C thanks Michael G. Paciello for his efforts in maintaining this page.

Michael has proposed that a more extensive project be started, if there is sufficient provision of resources and enthusiasm by Consortium Members. Please indicate your organization's opinion on this matter with a mail to disability-response@w3.org

- Should W3C resources be spent on this?
- Would your organization possibly be prepared to provide effort, or funds, or to match funds from other sponsors?
```
*(DanielD, 2009)*

Not much later the Web Accessibility Initiative (WAI) was officially launched, bringing accessibility standards to HTML forever, only to improve in later versions of the markup language. With the release of HTML5 in october 2014, a large array of new tags was added, all of which have their own semantic value and emphasis. This 'new' HTML-standard is supported by all modern webbrowsers, meaning everyone can benefit from it's positive traits. 

## Accessibility Tree
Now on to a more technical view on the main topic. Webbrowsers 'read' an HTML-webpage from top to bottom, and generate a DOM Tree from what it has read. Only grabbing the nodes the document consists of and creating connections between these nodes based on the relation (parent/child) each element has with one another.

But there is also another kind of tree the webbrowser generates, the Accessibility Tree. Similar to the DOM tree, the Accessibility Tree is a rendered list of nodes on the document the browser read. However, this time all the nodes with properties bound to them are set as metadata, for screen readers and other accessibility software to use. This means the software can distinguish which element is currently selected, which hyperlink is given in the `href`-attribute, or whether a checkbox box is active or not.

The Accessibility Tree is a key factor in making the web usable for everyone.

## ARIA
In Q1 of 2014, the World Wide Web Consortium published a the WAI-ARIA as a web standard. This is short for "Web Accessibility Initiative - Accessible Rich Internet Applications". It features multiple attributes to provide semantic values to HTML-elements that are in need of them, for instance: ARIA-attributes make it possible for a `<div>` to be recognized as a `<button>` element by screen readers. But do not be fooled by its magic, developers should **never** use ARIA as a replacement for already existing elements with plenty of semantic value.

The example with the button will not provide the element with the technical aspects a normal button has, like focusability or an automatic click handler. For this to work, keyboard navigation has to be implemented, whilst a simple `<button>` element would've done that in the first place.

So what are good cases for ARIA use, exactly? While screen readers should have enough data from the Accessibility Tree already, there are events that can occur when the user interacts with elements. The available attribute can make sense of certain things that are not native to HTML. The information exposed can range from something as simple as telling a screen reader that activating a link or button just showed or hid more items, to widgets as complex as whole menu systems or hierarchical tree views *(Marco, 2014)*.

## The A11y Project
In order to help struggling developers with creating accessibile websites, the A11y Project has been created.
The name 'A11y' is short for saying 'Accessibility'. The number eleven stands for all the characters between the 'A' and the 'y' of the word. The organisation consists of multiple developers who want to help their fellow colleagues by sharing everything they know on the topic. Mainly with the following three principle in mind:
- **Digestible.** They strive to feature short, digestible pieces of content.
- **Up-to-date.** The project is hosted on Github so information can be current with the latest standards.
- **Forgiving.** People make mistakes and web accessibility is hard, so they seek to be encouraging.

*(The A11y Project, 2013)*

If you are a developer, and want to know more about developing with accessibility in mind; do checkout the webseries of 'A11ycasts' made by Rob Dodson for Google Chrome. As of the time this article is being written, a set of 18 short videos have been uploaded to the A11ycasts series. They are easy to follow and are full of information about accessibility on the web.

## References
**The A11Y Project. (2013). MYTH: Accessibility is 'blind people'.**  
*http://a11yproject.com/posts/myth-accessibility-is-blind-people/*

**DanielD. (2009). WAI early days.**  
*https://www.w3.org/WAI/history*

**Marco. (2014). What is WAI-ARIA, what does it do for me, and what not?**  
*https://www.marcozehe.de/2014/03/27/what-is-wai-aria-what-does-it-do-for-me-and-what-not/*

**The A11y Project. (2013). Accessibility is hard :(.**  
*http://a11yproject.com/about.html*

**Rob Dodson. (2016). Introducing A11ycasts! -- A11ycasts #01.**  
*https://www.youtube.com/watch?v=HtTyRajRuyY*
