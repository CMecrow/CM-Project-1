# DMDC - Danebury Metal Detecting Club
Danebury Metal Detecting Club, abbreviated to DMDC, have commissioned a website to be made to help them recruit more members and provide information about the club. The site is targetted towards individuals who may be interested in joining the club for recruitment purposes and also toward existing members, providing information about their weekly meet ups.

User experience considerations available [here](https://github.com/CMecrow/CM-Project-1/blob/main/docs/DMDC_UX_1.pdf).
Initial wireframe concepts available [here](https://github.com/CMecrow/CM-Project-1/blob/main/docs/DMDC_Wireframes.pdf)

![https://imgur.com/cAij1Cz](https://i.imgur.com/cAij1Cz.jpg "Site responsiveness")

---

## Features
### - Navigation Bar
- Features on all 4 pages, the full responsive navigation bar includes links to the Home page (Index), Join Us page, Online Finds Table page and About Us page and is identical in each page to allow for easy navigation
- Navigation bar features a central DMDC logo, enhancing club identity and offering a recognisable symbol for the user. This also functions as another link back to the home page.
- Page links are positioned symmetrically, 2 on each side of the logo
- Links are concise and one word for aesthetics and ease of use
- Simple font and colour choice for clarity and accessibility
![https://imgur.com/VZtGwRi](https://i.imgur.com/VZtGwRi.jpg "Nav bar")
### - Hero Image on each page
- Visual display to promote a positive emotional response from the user
- Helps identify the site's content and solidify the identity of the club itself
- Displays a visual of what the user can expect to come across while a member of the DMDC
- Hero image is accompanied by emotive Headline message on the main page, providing brief information about the club, embedding it in the local area
- Priority again sustained with a visible bright 'JOIN US TODAY' link to the Join page
![https://imgur.com/HmUw3Y7](https://i.imgur.com/HmUw3Y7.jpg "Hero image")
### - Online Finds Table
- Layout is mirrored from the 'About Us' page across the top
- Title identifying the page 'Online Finds Table' under the hero image
- This is included as the page isn't an expected page on a website
- Includes three most recent finds of note from members of the club, along with accompanying information: Find title, Historical date, Item description, Finder's name and Find date
- This page is designed to peak the interest of a prospective member, and also as a point for existing members to have their great finds highlighted.
![https://imgur.com/JW808tK](https://i.imgur.com/JW808tK.jpg "Finds table")
### - About Us Page
- Mirrors layout of the Online Finds Table across the top half of the page
- Includes meetings information, displayed through a split image 4x identical sizing, facilitating one of the high priority site goals.
- Brief club information in the centre of the page as this is the main focus. Minimal text as with the rest of the site, also contains a contact email.
- Google maps embedded at the bottom right to display the meetings location to prospective members
- This page is the main information point for users, and also fills an expected convention of a club or group website.
![https://i.imgur.com/rbaeJvq](https://i.imgur.com/rbaeJvq.jpg "About page")
### - Sign Up Page
- This page will allow the user to sign up to the DMDC, declaring their interest and giving the club a point of contact to send over meeting information. The user will be required to submit their name, email address and experience via text inputs.
- This page was the main project goal of the website, to provide an area for new members to sign up to the DMDC. I chose the below image specifically as it was high definition, like all other large images across the site, and also fitted the theme nicely. The image was not too busy in terms of colour or content and because the main focus was actually blurred, the metal detectorist in the grass, I felt that it would not detract from the sign up form.
![https://imgur.com/nQCY0NQ](https://i.imgur.com/5Mcy1rK.jpg "Join page")
### - The Footer
- The footer section includes links to the relevant social media pages for the DMDC, they will open in a new tab, contain an aria-label for accessibility, as well as rel="noopener" for added security. These links will work towards the original goals of conveying club information and offering potential members extra ways to connect with the club.
![https://i.imgur.com/nQCY0NQ](https://i.imgur.com/nQCY0NQ.jpg "Footer")

---

## Future Features

### - Future Feature Idea
- A page where members could pay their membership fees online. This could also branch out to provide a site for members to order or reserve club merchandise.
  - This concept falls outside of the scope of the first iteration of the site. Both in terms of time investment and knowledge of the developer. It could feasibly be introduced a few months after first release, once members have got used to the layout and nature of the site in its current form.

- Creation of a forum / chatroom for members and prospective members
  - As with the above, this concept would require a large investment of time and outside knowledge to implement. Both ideas would be useful and relevant for a site such as this and would provide the site with more interaction from users, and could provide another stream of income for the club.

---

## Testing

Separate testing file linked [Here.](https://github.com/CMecrow/CM-Project-1/blob/main/docs/Testing.md)

### Validator Testing
#### HTML - 
When passing through HTML validator - [W3C validator](https://validator.w3.org/nu/) there are 2 areas related to the 'join' page, namely the lack of a 'method' or 'action' value in the sign up form. This was a conscious decision to avoid any site errors or crashes when a submission was attempted. Were the site to go live, this would need amending as a first priority. This is mentioned in more detail in the testing document.
#### CSS -
No errors were returned when passing through the official [(Jigsaw) validator](https://jigsaw.w3.org/css-validator/)
### Accessibility
I confirmed the colors and fonts chosen are easy to read and accessible by running it through lighthouse in devtools.

![https://imgur.com/d81MrCC](https://imgur.com/d81MrCC.jpg "Lighthouse rating")

### Unfixed Bugs

Discussed on [Testing page.](https://github.com/CMecrow/CM-Project-1/blob/main/docs/Testing.md)

---

## Deployment
  
- The site was deployed to GitHub pages. The steps to deploy are as follows:
  - In the GitHub repository, navigate to the Settings tab
  - From the source section drop-down menu, select the Master / Main Branch
  - Once the master or main branch has been selected, the page will automatically be refreshed with a detailed ribbon display to indicate the successful deployment.
The live link can be found [here.](https://cmecrow.github.io/CM-Project-1/index.html)

---

## Credits

### Content

Instruction on how to embed a google map without using Javascript where possible was found [here](https://blog.duda.co/responsive-google-maps-for-your-website)
The icons in the footer were taken from [Font Awesome](https://fontawesome.com/)
Further tutorials used are detailed in the [Testing page.](https://github.com/CMecrow/CM-Project-1/blob/main/docs/Testing.md)

The footer HTML and meeting information CSS / HTML were based on those covered in the CI [Love Running project.](https://github.com/CMecrow/love-running)

### Media

Images used are not copyright free as they need to pertain to the 'DMDC', a fictional metal detecting club created for the TV show 'The Detectorists'. I also had great difficulty locating appropriate images via copyright free sites, so had to look elsewhere.

Homepage: Hero image taken from [Amazon Prime](https://www.primevideo.com/detail/Detectorists-BBC-Series/0U8H58N2QNJJEJVNO91MDGUPVT)

About: Image taken from [TheTVDB.com](https://thetvdb.com/series/detectorists), Meeting image taken from [pexels.com](https://www.pexels.com/photo/green-grass-field-1574547/)

Finds: Image taken from [Thecustardtv.com](https://www.thecustardtv.com/2017/12/detectorists-well-miss-this-gentle.html)

Find One image taken from [ashmolean.org](https://www.ashmolean.org/alfred-jewel#/) Text from same source.

Find Two image taken from [etsy.com](https://www.etsy.com/listing/209330555/4-collectable-victorian-and-edwardian) Text taken from [compassrosedesign.com](https://www.compassrosedesign.com/pages/history-of-buttons)

Find Three image taken from [vcoins.com](https://www.vcoins.com/en/stores/educational_coin_company/55/product/great_britain_medalets_victorian_and_edwardian_a_lot_of_7_items/1151252/Default.aspx) Text taken from [logicmgmt.com](https://logicmgmt.com/1876/living/money.htm)

Join Us: Image taken from [mattiasnyberg.com](http://mattiasnyberg.com/portfolio/detectorists)
