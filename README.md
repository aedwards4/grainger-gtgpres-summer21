# Grainger GTG Final Presentation
## Web app made with Svelte, HTML, and CSS

I utilized what I learned during my Summer with Grainger to create a website for my final presentation, which was showcased at an event open to all GTG (Grainger Technology Group) members before the end of my internship.

## Summary of Presentation

### About Me
- 5th year senior at Illinois Tech, graduating May 2022 with both my Bachelor's and Master's degrees in Computer Science
- Originally from New Orleans, moved to Chicago in 2019
- When not working or studying, I enjoy cooking, traveling, biking around the city, or sitting by the river with a good book 

### My Team - Core Engineering Experience

We are an enablement team, which means we provide tools and reusable patterns to other product engineer teams so that they may focus on the needs of their customers within their domain.  - Our work largely contributes to a consistent, seamless experience for our end customers.

We accomplish our goal a few different ways:
1. We provide an Experience System Framework with the Experience System Generator and Starter Kit. 

2. We provide a design system publication which contains detailed documentation for each of our components. Each component page provides details for that component and serves to educate those who plan to use it.

3. Finally, we provide an Experience System Strategy and Architecture through the shell app.


### My Experience
During my time here at Grainger, I have completed a few technical tasks and networked with other teams.

Some of my technical tasks include:
- Adding to the Design System Publication
- Making small changes to components in the Experience System
- Working with Google's Lighthouse dependency and thoroughly researching about accessibility in design

In the design system publication, I have added component pages for the Checkboxes and Text Inputs. To do this, I leveraged a custom Svelte component I made that has the potential to be used in future pages as well. 

My work in the design system is important because consistency is key. When customers are visiting our website, consistent design and components helps us to tell a story which ultimately develops trust with the customer. The only way to maintain this consistency is by providing a design system that outlines in detail how to use these components. 

As more and more teams will start using them, they need a place to get them and to learn about them. That is where my work comes in. The only way teams will know how to use checkboxes and text inputs in their work is by visiting the pages I deployed to the design system.

My work in the experience system mainly involved updating the styling of components to match design standards. I was able to correct the off-center check in the Checkbox and increase the border of a Text Input variation. Although these changes are not complex, they are still important for consistency and use. Our team cannot make anyone to use these components, but it is more likely that they will if they look good and function well. If these components look broken, in the case of the off-center checkbox, for example, people won't use them, which can have a domino effect that affects consistency in our website and ultimately our customer's perception of us as a company. 

Also, my changes were sent out to those teams who are currently using those components. So even though they were small, they had a widespread impact across several teams.

Finally, and possibly most importantly, I spent alot of time with Lighthouse and learning about accessibility in web design. Lighthouse is a dependency made by Google that assigns scores and tracks metrics for performance, accessibility, best practices, and SEO. 

While these numbers are of great importance in tracking our progress and making improvements, it is what they represent that matters most. Performance and accessibility are wildly important to our user's experience. Here you can see an example lighthouse report:

- Time to first contentful paint tells us how long it takes for the user to actually see something. You can think of it as how quickly we communicate to the user that the website is working and loading.

- Time to Largest Contentful Paint is similar, but represents how long it takes for the user to see the largest content on the page

- Time to Interactive is extremely important because it is the time it takes for the user to be able to interact with our website, whether that be through text inputs, buttons, etc. This is so important because users are highly likely to navigate away from a website if they cannot interact with it within 5 seconds. So it is crucial to keep this time as low as possible.

Accessibility was a prominent theme in the learning I did while I was here. Coming into my internship, all I knew about web development came from various YouTube videos, which never spoke about accessibility once. I had no idea how my code and design might be affecting those using aids such as screen readers. 

I started out here learning Svelte, which interestingly enough promotes accessibility through small features such as requiring an alt tag on an image element. I then took the time to learn about semantic HTML, which is crucial in providing a seamless experience for those using screen readers, and but also has the added benefit of improving SEO too. And I was actually able to implement a lot of what I learned in building this website for my presentation. 

I also learned that performance and accessibility are closely related when it comes to the devices people are using and the cost of Javascript. As of recent, the web is largely accessed via mobile phone as opposed to a desktop or laptop. Although iPhones and Samsung phones seem to be most popular, I was surprised to find that median to lower end phones are much more prevalent, so it is important to consider things such as CPU availability and performance when deciding to utilize lots of Javascript on a website, as it can serve as a huge bottleneck. I came to understand the concept of "HTML first", which means we try to accomplish all that we can through HTML and CSS alone in order to promote accessibility to our websites.

The other half of my experience this Summer was networking with several teams within GTG. I was grateful to have the opportunity to meet so many new people while learning about Grainger Technology Group and the tech industry as a whole. 

This was of great value to me because I never understood what exactly a day in the life looked like for someone working in tech. So many people took the time to show me their work and processes, which really helped me gain a better understanding of how this industry works and even helped me find new things I may be interested in pursuing. 

I also found networking to be a great opportunity to develop professionally. I am typically a shy person and struggle to reach out or speak up, so I appreciated the chance to work on this skill while I was here.

