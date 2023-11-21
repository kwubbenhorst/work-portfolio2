# work-portfolio2
A professional portfolio showcasing my deployed webapps(copy of the kwubbenhorst-work-portfolio repo, updated for current use)

## Description:

This was a very personal project for me. As I try to launch a new career as a full stack developer I thought it would be fitting for the professional portfolio, which I will show to prospective employers, to be, itself, an exemplar of my web design. This simple layout presents the traditional sections of a portfolio of work: a short synoptic statement of what I am about (about me), a projects showcase (my work) and a section at the bottom with several options for how to reach me through email, phone, or social/professional media platforms (contact me). While the showcase currently only includes three projects, one of them still in the development phase, I anticipate that this section of the page will grow.  When there is too much content to view on the height of a single screen, then the navigational links at the top will be convenient as a way to click and be taken directly to the relevant section of the page. The fourth link in the navbar, CV, is to a pdf of my CV. The project images are also live links which will take someone viewing the page to the deployed projects at their external web addresses. In terms of the features built into the page, media queries have been added on the stylesheet so that the application is responsive to different viewport dimensions. Instead of using the traditional breakpoints of 992px, 768px and 576px, I found when using the inspect tool that most of the adjustments needed to be made at higher viewport widths, with the most wholesale changes happening at width: 1066px.  In the screenshots below, the first two images display the page at 1067px and 1066px respectively. The following three images are at the 576, 768 and 922px widths, to demonstrate that the app will look good on tablets, larger smartphones and smaller smartphones as well as the default laptop settings for which the page was originally coded. In future I will embrace mobile-first design.     

![At 576](https://github.com/kwubbenhorst/karlawubbenhorst-work-portfolio/assets/140316693/30b87bb9-495e-4c4b-b97c-f9cbd81fd812)
![At 768](https://github.com/kwubbenhorst/karlawubbenhorst-work-portfolio/assets/140316693/ce170aec-00d2-4800-9023-0a35012c45f2)
![At 992](https://github.com/kwubbenhorst/karlawubbenhorst-work-portfolio/assets/140316693/43eaf9c4-0b9c-4606-870f-b012f6fc7544)

In the version history of this webapp, there were two major iterations, the first had one major visual problem which was that the vertical lines separating the section heading from the section content were not aligned.  My original effort had too many containers and there was inherited styling that interfered with my ability to make each section look uniform.  In the second effort I restructured the html and completely rewrote the CSS, giving the sections I wanted to make uniform the same class name so that I could style them all together. It was not necessary to change all of the rules I had arrived at by a painstaking trial and error process to find the right properties to adjust and, based mostly on eyeballing, the right values to give them, but I did have to change all the selectors, because there were now fewer sections. I am now fairly happy with the appearance of the page. The quality of the profile picture is not high resolution, but this is the one recent picture I had of me that was easy to isolate from its background. Then in the Affinity Photo photoeditor I laid the white-background profile shot over a background image I found online when googling "blue fade to white wallpaper."  It is free from copyright but is also not high resolution, especially since I had to crop the section I used from a larger background slide that was in the other orientation. I merged these two images together in Affinity, then inserted them to the hero banner area of the page using a relative path url and the figure and figcaption tags. This was a different method for inserting image files and controlling size than was used for the image-links to the projects in the "my work" section. Both kinds of images (the image used as a background in css and the images linked to from an img src in html and made into cards with moveable headers) are given a description for accessibility by means of an alt description or hidden figcaption. I uploaded my hero banner image to the redketchup.io/color-picker in order to create the color palette for the page. This tool allows you to select areas of an uploaded image and discover their hexidecimal color values. These I then set as variables within the stylesheet so that, if, at a future point, I should find a more high resolution replacement for the hero banner image with different colors, I can merely update those values for easy maintenance of the page. 

While the hero banner is in low resolution, the source images for each card/link in the projects showcase varied widely.  The horiseon image was huge and needed to be reduced to a third of its size whereas the password generator image needed its size doubled. This is easy enough to do using Affinity Photo but the optimal size of images used on webpages is something I shall continue to read up. From what I have read so far, very high resolution images are not recommended because it hampers search engine optimization and increases the loading time for the page. Once I had my images linked in, I controlled their dimensions and positioning on the page by a variety of strategies: flexbox, relative and absolute positioning to make card headers into overlaid labels, and setting different values for margin and padding in the css box model. To help with responsiveness I used relative measurement units in some places but my preference is still for working in pixels, which I find more readily understandable. 

I found the use of a wire frame invaluable in breaking down the space so that I could conceive of how to divide it into sections when building the HTML. See my wire frame below:

![wire frame](https://github.com/kwubbenhorst/karlawubbenhorst-work-portfolio/assets/140316693/38dfd4a6-e2d9-4c23-b043-6b2ddbcb84a5)

The header with interior page navigation, the hero section (profile pic and job title), and the footer which comprises the "contact me" section with its external links, are fairly straightforward, but things got more complex in building the main section, particularly the projects showcase. While the category headings running down the left hand side of the page might have been conceived of as a sidebar, I thought it would be easier to conceive of the page as a series of rows, each with several subsections or containers. Originally I thought it should be possible to make the projects showcase one big flex container, arranging its three items using the flex-properties and values. I wanted the card for the horiseon project to be bigger than the cards for subsequent projects, and probably there is some way to do this using the flex and flex wrap properties, but I opted for the way which seemed to me easier, of just making a top row container for the single large card, and then arranging two cards side by side in the bottom row container.

As expressed above, I intend to add to the projects showcase section of this page as my portfolio grows. There could also be a section added in the future to display testimonials from satisfied clients. I will also want to update the substance of my cv which is linked to from the navbar but not very current. It was framed as a document to commend me to prospective employers in the teaching or ecclesiastical sectors.


## Installation

N/A

## Usage

The page is deployed and ready for use on the World Wide Web.  Please visit https://kwubbenhorst.github.io/karlawubbenhorst-work-portfolio 

## Credits

Karla Wubbenhorst was the sole creator of this web application showcasing her portfolio of work. Although the project was built from scratch there were various code snippets that were used as templates for different sections of the page.  For example the horiseon webpage that was originally created with code developed by Xamder Rapstine of Austin Texas http://www.rapstine.com, and George Yoo of Winter Springs, Florida https://www.linkedin.com/in/george-yoo/ provided the template for the header with sideways floating navigational links. The code from EdX bootcamp's module 2 exercise 6 (a product showcase with multiple cards), was consulted to help produce the body section. 

The images used on the page are from the following sources:
https://whatismyip.network/strong-password-generator/https://wallpapers.com/blue-fade
https://www.istockphoto.com/photo/young-man-discussing-market-research-with-colleagues-gm507959212-84975781?utm_source=unsplash&utm_medium=affiliate&utm_campaign=srp_photos_top&utm_content=https%3A%2F%2Funsplash.com%2Fs%2Fphotos%2Fmarketing-agency&utm_term=marketing+agency%3A%3A%3A and
https://unsplash.com/s/photos/marketing-agency

Colors were chosen using the Redketchup.io/color-picker tool.

The reset stylesheet was created by Richard Clark - http://richclarkdesign.com  Twitter: @rich_clark

## License

Licensed under the MIT license
