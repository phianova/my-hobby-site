# my-hobby-site
This is a repository for a practice website built around a hobby or interest - I chose New Zealand birds. This was created for an assignment of The Developer Academy's web development bootcamp.

# Brief
The elements I had to include were:
1. *A Home page that introduces the site.*
2. *A minimum of three additional pages.*
3. *A consistent navigation structure for all pages of the site*
4. *A coherent design for all the pages of the site.*
<!-- 5. *CSS styling and / or layout stored in external stylesheets*  - we were asked to use Tailwind instead.-->
6. *Pictures that have appropriate alt text.*

# Site design
I began by creating a template in Figma (available at https://www.figma.com/file/m6GLzA0mg3C7gSkDkiSeQo/My-hobby-site-design?type=design&node-id=0%3A1&mode=design&t=7kDaYsMNgYAeOhIy-1).

I created my homepage first so that it could be used as the template for the other pages to keep the style consistent.

I used two pre-created Tailwind components for this project - a navbar and a footer.

    Navbar: 
    https://tailwindui.com/components/application-ui/navigation/navbars#component-70a9bdf83ef2c8568c5cddf6c39c2331 (the free one)

    Footer: 
    https://tailwindcomponents.com/component/footer-2

I significantly modified these to meet my needs as I didn't need this level of complexity.

I wanted a consistent colour scheme across the site so I decided to stick to Tailwind's greens and oranges, using different shades and opacities to achieve different effects. I kept the main text black and the sidebar text white for clarity, ensuring adequate contrast.

# Site features

I wanted to include an image gallery, which I initially tried to achieve using flex but ended up using grid so as to be able to easily make the content stack on mobile devices by changing the column structure.

I used a sidebar for navigation within the page, turning on smooth scrolling to avoid having it jump too fast between items when used.

I tried to make everything as responsive as possible, amending font sizes and the page structure for smaller devices and making sure everything still looked proportionate on larger screens.

I tried to create an interactive feel by making all links either change colour, translate slightly upwards, or change background colour when hovered over. 

I created tabs and buttons on the Resources page to make what would have been just a list of links look a bit more interesting. 

# Issues I encountered and troubleshooting

I wanted a semi-opaque background image so it didn't take too much attention away from the content. I didn't realise neither Tailwind nor CSS supported this. I found a suggestion online of using a translucent overlay so I created a <div> with an opacity of 30 and that worked really well.

Another thing I learnt was that you can't apply hover:transforms to items that aren't inline. I fixed this by applying a class of "inline-block" to my sidebar items that I wanted to translate upwards on hovering.

I struggled with Git for a while as I'd accidentally forgotten to check out a new branch I used. I didn't quite manage to find the solution so with some help from Alfie I learnt how to use "git log" to find the hash ID of my commit and then "git cherry-pick <ID>" to specifically pick out the commit I wanted to pull over to the correct branch.

I also found I was having issues making fonts responsive as every time I merged a branch and opened it in GH pages the fonts seemed really small...this was in fact because I was zoomed out in my browser. Felt silly but important to learn I guess!
