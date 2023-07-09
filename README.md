# Foodie Society

## Introduction

The Foodie Society is a website to help connect with the community united by their shared love and enthusiasm for all things food-related and is open to all like minded individuals.
The Foodie Society is a great resource for inspiration, recipes and tips and tricks that have been tested and are certified to satisfy your tastebuds and improve your cooking skills.

The Foodie Society will offer it's users following information: introduction and details about us, details about our gatherings, meetups and online calls, various recipes and contact information to get in touch and join our community.

## Wireframes

Created using [Balsamiq](https://balsamiq.com)

## About the build:

### index.html

I started the project and created all of the required pages: index.html, recipes.html, form.html, style.css, including the folders: assets containing css and images folder.
I created the structural layout for the home page:

1. At the top header with navigation bar containing all of the pages the project will have.
2. Hero image section that would contain the details so users would know what is the site for.
3. About section with couple of details explaining who we are and what are the benefits of joining.
4. Meetup and online chats section that will specify the times, dates and possible locations of gatherings.
5. Footer with all of the links for our social media sites and a direct link to a contact form.

Given that the site is food and food lover oriented, I have decided to gather couple of pictures connected to the topic. I checked and used [PixaBay](https://www.pixabay.com) and [Unsplash](https://www.unsplash.com) to get royalty free images.

After making a structural layout of the home page I started coding the site and I used previously learned topics and videos for support to locate certain coding styles. I also used ChatGPT to bounce the ideas around and for help checking if my colour pallete was sufficient enough and for couple of tips on how to construct some code to help me with the task **ie. how to align the image within the element** = actual code: **_display: block; margin-left: auto; margin-right: auto;_**

I made the basic header look and decided to style it later, once my hero image is in place. After adding the hero image I started with styling of the general look and feel of the site, even though I changed it along the way slightly. After succeeding with the header and hero image, I was creating the text for the hero image and ended up struggling slightly, but decided to look up and follow the instructions within the Love Running project, to use the general details and adjust my own changes and styles once I found my mistake. I forgot to set the **position** of the hero image-outer id to **relative**, which didn't allow for my text to align where I wanted it to.

For the about us section I decided to create two articles contained within the div elemeent to contain two paragrafs split by an image and to be centered and aligned with each other.

Next task is to create the meet up section. After choosing and adding an img file I set it as a background and added 5 divs to my meetups section to contain all of the details about our weekly meetups, online classes and exploring of restaurants and coffee houses.
_later_ I realised my links are not opening in a separate tab and that they do not contain explanation for the Screen Readers so I worked on adding the code by implementing: **target="\_blank" rel="noopener" aria-label="xyz(opens in a new tab)"**

While creating the footer. I was struggling with positioning of the social media links as they were automatically aligning to the right in reverse order. I was reserching the ways to reverse the list order and have found a solution on [StackOverflow](https://stackoverflow.com/questions/47031111/displaying-the-list-items-in-reverse-order-using-css) so I used the following code from there and modified it to my needs:
ul {
-moz-transform: rotate(180deg);
-webkit-transform: rotate(180deg);
transform: rotate(180deg);
}

ul > li {
-moz-transform: rotate(-180deg);
-webkit-transform: rotate(-180deg);
transform: rotate(-180deg);
display:inline-block;
}

### recipes.html

I have started the recipes.html by copying the source code from index.html to reuse the body, Header, Hero image and Footer section in the build of the second page of a site. I spent some time informing and making sure I can still reuse all of my elements and that everything is still funcioning, and it did.

I decided to use three recipes that have been in my family and that myself or my family members came up with. The first one is a pizza recipe that is my very own that I have been making for years. The burger recipe is something my husband came up with and perfected over the years.

## Troubleshooting

After couple of days of coding and doing final add ons onto the home page I have realized I haven't included aria-label for the navigation main logo and navigation menu. So I worked on adding all of them and making sure all links have a aria-label.
