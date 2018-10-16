# Pale

A website for my band "pale".

This is a hub for all things going on with pale and is to be used as a major part of our branding. Use of monochrome and monospace to portray the themes that are in our music on our website.

A bit of background regarding pale. Pale itself is still within its forming period of time, we have written 4, 4 track eps which form one album, or cycle, and are about to head into the studio to record. We are building up a portfolio of all forms of media (artwork, videos, photoshoots, music), and the website will evolve with our progress. However, as a collective band we had decide to present pale to the world differently. Our bleak sound is a stark contrast to the mainstream, with social media and ontap information ruling day to day life, we believe presenting ourselves within this world differently. This has led to design choice of having minimalist information regarding the band compared to other band websites. "Less is more," was a key factor in the writing of the album, and I have brought that ethos into the build of this website.

We currently have not gone public with the band, we haven't played a single show or have any form of social media. Because of this, some of the content within the page is "not live," for example, the footer social media links do not lead to social media, as we currently do not have any and the upcoming shows section are fake shows, with the links leading back to the page. However I have built the website with the content in mind, and have cloned the repo to keep it updated post submitting.
 
## UX

This website is the key for all information regarding pale and making sure users of all types can access our content and contact us easily, while still experiencing something very on brand for pale. 

The users can be broken down into 3 major groups, Potential fans, Loyal fans and promoters. 

User Stories:

User 1
Potential fan Saw us at a live show and wanted to check out music to share on his social media. Found the website through a social media link. Short attention span so the first image would need to be striking. Watches half the video, wants to leave with some content to remember us by.

User 2
Promoter. Always looking for new bands, but has no time to be wasted. Wants to find band information and contact details. Needs quick access to contact information

User 3
Loyal Fan. Access website through a search engine or direct link. Wants to find out as much information as possible. Likely to spend longer than any other user on the website.

To facilitate all different user types the website needs to have a clear easy to use navbar, strong imagery and access to music/video. 

In design terms, pale portrays sorrow in its music and how we present ourselves, and this is a key element in the design process. We have chosen to have no logo, and use a strong monospaced font throughout the page, using blacks and greys to create space around the artwork.

I created wireframes and have included this within a Folder. Inside the wireframe folder there is a seperate wireframe for each page, including the basic navbar and social media links on every page. This was useful in my dev process as it was a point of reference and kept the UX in mind.

## Features

### Existing Features

Navbar - Fixed top navbav so the user has access to all pages of the website. This includes a transition of ease-in-out which adds a positive user response. Upon collapse this falls into a simple dropdown menu.

Video Lander - Autoplaying muted video upon landing on index page. This is to draw the eye yet be non intrusive via being muted. This is hidden on XS due to iframe mobile browser security.

Music Player - Within the Media page there are playable songs with the option to download. No autoplay to let the user define their own experience 

Footer - At the bottom of every page so users can direct to social media with ease. This also includes the same ease-in-out transition as the navbar, giving the same user journey.

Gigs - Upcoming gigs including location, time and a link to purchase tickets

Contact form - Simple page with bootstrap contact form. I used the grid system and custom styling to manipulate the bootstrap base form.

### Features Left to Implement

Artwork - Within the media page a dedicated artwork section (Each song in cycle 1 has its own piece of artwork)

Mailing List

## Technologies Used

In this section, you should mention all of the languages, frameworks, libraries, and any other tools that you have used to construct this project. For each, provide its name, a link to its official site and a short sentence of why it was used.

- HTML5/CSS3
    - The project uses HTML5/CSS3 To build and style.
- [Bootstrap v3.3.7](https://getbootstrap.com/docs/3.3/)
    - The project uses Bootstraps grid system and inbuilt components to further style.
- [Font Awesome](https://fontawesome.com/)
    - The project uses Font Awesome for social logos
- [Google fonts](https://fonts.google.com/)
    - The project uses Google fonts for fonts
- [JQuery](https://jquery.com)
    - The project uses **JQuery** to simplify DOM manipulation.


## Testing

My first test was to test all my code by running it through the W3C validator (https://validator.w3.org/), to check for syntax errors. 

I then created a tick grid to test features on different browsers and sizes (wireframes/Testing.png) This made it easier for me to stay on top of the testing as I achieved it. 

I followed the following test process, and will also discuss any issues arisen.

Navbar:

1. Open any page
2. If on desktop, check ease-in-out transition works
3. Go to the navbar and click home. Verify it takes the user to home.
4. Click about and verify that user is taken to about.
5. Repeat process jumping from all pages to all pages.

Navbar Collapse:
1. Open on Android device.
2. "Burger menu" icon appears. 
3. Go to home page, verify user is taken to home.
4. Go to about, verify this also.
5. Repeat process jumping from all pages.
6. Repeat on ios device.

Gigs:

1. Open index page
2. Scroll to the bottom
3. Click on “tickets” link (Current code has href="#" with the intent to link up to ticket website when it is live)

Video Lander:

The video lander feature took the most time to implement, as it through up issues. Hosting the video on youtube and using an iFrame embedded the video into the background styling, however it wouldn't autoplay, or play at all. However, this was solved but adding "&mute=1" at the end of the iframe link. Muting an iframe allows autoplay, which is perfect as the background video muted fits into the minimalist UX design of the band. 

However, iFrames do not autoplay on mobile browsers, and the iframe is hidden behind a foreground (for the parallax effect) so the user could not play the video. To solve this, it is hidden at the xs bootstrap breakpoint.

Contact form:
1. Go to the "Contact" page
2. Try to submit the empty form and verify that an error message about the required fields appears
3. Try to submit the form with an invalid email address and verify that a relevant error message appears
3. Try to submit the form with an valid email address and no content within message and verify that a relevant error message appears.
4. Try to submit the form with all inputs valid and verify that a success message appears.

Footer:
1. Scroll to the bottom on any page
2. If on desktop, check ease-in-out transition works
3. Go on Twitter icon and verify that it leads back to index. (Current code has href="#" with the intent to link up social media when it is live)
4. Repeat process with youtube and instagram links.
5. Repeat steps 1-3 on all pages.

Responsive Design/Mobile First:

As I have used the Bootstrap grid system throughout this process, I have been able to approach the website with a mobile first UX in mind. To achieve this, I used http://buildbootstrap.com/ as part of my dev process to help initial build the grid. However this did also come with some issues, mostly images breaking the breakpoints while stacking up.
To get around this, I used the Responsive tool within Google dev tools to collapse my website to as low as 320px and make sure the images didn't push the website beyond its width.

## Deployment

I used github through the dev process, and have pushed it using GitHub Pages. I have pushed it using the master branch.

## Credits

### Content & Media

- All music, artwork and media are property of pale and all permissions are required to use. 

### Acknowledgements

- I received inspiration for this project from The Bronx (https://thebronxxx.com/) Mariachi El Bronx (https://mariachielbronx.com/) and Comeback Kid (http://www.comeback-kid.com/)


