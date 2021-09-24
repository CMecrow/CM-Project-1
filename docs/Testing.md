## Testing

### Generic features:

#### Color Choices

    - Used the below site to create a colour palette after selecting my base colour green present in the image borders. This green was chosen as an earthy tone to match the subject matter. Greens taken from the created palette were then used repeatedly throughout the site for continuity and aesthetics. I selected a light blue from a created palette to contrast strongly on hovered links to follow the accepted convention that the item would link elsewhere. I did NOT follow this rule on the 'JOIN US TODAY' link present on the home page as the text was instead white and the colour change was quite jarring. Instead I applied a drop shadow to the containing div element then an inner shadow when hovered to mimic a press-able button. Because the colour hex codes were taken from a palette, they were not easily recited from memory so I created variables for them instead. This would be a benefit should the client wish to change the colour scheme of the site at a later date.
[ColorSpace](https://mycolor.space/)
[Variable tutorial](https://www.w3schools.com/css/css3_variables.asp)

#### Header and Nav
    - Couple of different techniques used to try and centre the DMDC logo in the Nav. First attempt was to use an <ul> element inside the <nav> element with the <nav> element set at a smaller width to work as a boundary for the links. The Home and Join <li> elements would then be targetted and floated left with Finds and About floated right. This would then create a gap in the centre for the logo. Though this may have worked fine for a desktop site, I was concerned that applying a strict pixel dimension to the <Nav> element would cause issues when trying to make the site responsive.
[Tutorial followed](https://youtu.be/hp-LP8Nv18s) 

    I instead centred the logo using percentages to help with responsiveness and match my mobile wireframes. I then positioned the <a> nav links via display: 'flex' with CSS3 to create the desired effect.
[Tutorial followed](https://www.w3schools.com/css/css3_variables.asp)

#### Footer
    - Difficulty producing a footer that stayed in the correct place on all pages without individual page by page adjustment, notice separate positioning on home and join page compared to about and finds.

#### CSS Measurements
    - When building the site I relied heavily on pixel measurements. I leaned towards pixels as whenever I tried to use %'s I ran into problems with positioning which was a difficulty throughout. Now looking back at the completed site, it would have been greatly beneficial to have persisted with % measurements rather than pixels, it would have made the site more easily responsive and more flexible overall. Though I could have gone back through the whole site and reconfigured measurements to %'s / em / rem, I was concerned about making such large changes, it was an area I didn't feel as comfortable with, and I was concerned about the time investment it would require at this point. I did try to adjust positioning at various points but found changing from px measurements to percentages more often than not knocked things off centre / out of alignment. This is an area I'd like to learn more about in the future.

### About Page
    - Creating the meeting info divs, because they were positioned using inline block they contained a 4px gap between divs which was related to the font-size for the page. To remove the gaps I had to set font-size to 0 for the parent div.
    - Inserting text into the parent divs for meeting and info moved the overall div position. This was remedied by inserting overflow:hidden into the CSS3.
    - Borders for div meeting blocks were not creating the desired effect as they'd double up between the divs (right 3px and left 3px creating a 6px border). Borders also didn't look as expected so internal borders were assigned the background colour with the parent meeting div being given a border instead to match other text elements on the page.
    - I'd previously placed the font-awesome logos in the meeting info in h2 and h3 tags for some simple easy styling. However they've now been changed to divs as the heading tags didn't make sense semantically.
    - I had real issue centring the 'info' box and had tried to do so via pixels and padding, however I then realised it could be simply done by placing all three divs (meetings, info and map) into a parent div with text-align: center, then applying margin: 0 auto to the info div.

### Finds Page
    - I originally inserted the images through CSS3 as background images to the selected divs, however I changed the images to be in the HTML code to be able to apply an alt attribute.
    - I changed the alignment of find2 and find3 divs using the same technique as the about page, placing all three divs into a parent div with text-align: center.

### Join Page
    - In original wireframes I had the radio button to the left of the label text, while I could find available solutions to this, they would not be fitting in level with the rest of my code so this was a change I stuck with.
    - I was satisfied at first with the misaligned input boxes and radio buttons but then decided to try to reformat them to get the labels aligned vertically, as well as the input boxes. The best solution I found for this is linked below. It involved formatting the form into a table through CSS. Although this achieved my goal to begin with, it meant the radio buttons were difficult to realign as they were now trying to fit into the table structure. Because of this, I reformatted them into another text input which won't affect functionality, and gives a wider scope for answers.
    - The new table format did however give me an issue with the submit button. To get around this I enclosed the other aspects of the form in a div, then had the join button in a separate div to help with positioning, and breaking it out of the table structure.
    - There was another problem that assigning width in %s wasn't giving the desired effect relating to the labels and inputs. This may have been due to the new table formatting, with the %s now relating to cell sizes. Though using pixels worked fine. It should not affect the responsiveness of the site as the text box will fit within the smallest view size.
    - I made the button much bigger than first planned on the wireframes as it was the main goal of the website, recruiting more members.
    - I also had the text box and form situated to the left of the page. However I was concerned that the image behind would then draw the eye and take precedence so I relocated the form to the centre of the screen.
    - I avoided including a method or action attribute in the form element for multiple reasons. Firstly to avoid any errors when running the site. Secondly if some sort of form dump was included, completion of the form could easily then take the user away from the page, requiring the user to then use the browser back buttons, something that's implicitly avoided in UX. The site would then also be reliable on the assigned form dump site, and should that site change then the user could easily encounter error pages. Because of this the form is not functional in this state. Were it to be deploted as a form with a method and action attribute, something would need to be added to display that details had been submitted successfully to the user.
[CSS Table Stackoverflow](https://stackoverflow.com/questions/4309950/how-to-align-input-forms-in-html)

### Image Choice
    - All large images across the site were chosen for their size and HD quality. They matched the individual themes of the pages:
        - The home page image is impactful and immediately displays to the user the content of the website, and offers an image of two of the club members, personalising the   club with a picturesque and emotive background.
        - The join page carries on the colour and content theme of wide open spaces and fields, without distracting from the overlaying content.
        - The finds page displays another two club members, out on a dig, displaying one of their finds.
        - The about page shows a picture of all club members, again offering the personal side of the club.

### Site Responsiveness

    #### Media Queries selection
    - < 1900px, chosen because of the about and finds page. Not enough space across for 3x horizontal divs. 
    - < 900px, chosen because nav begins to clash with title text. Finds page also altered to provide more spacing around images and text.
    - < 710px, chosen because of 'join us' text box, begins to get cramped.
    - < 650px, chosen because find page needs condensing to stack images and text on top of each other.
    - < 540px, chosen to condense nav menu and Join us form. Meeting information also beginning to spill out
    - < 420px, chosen as logo in nav beginning to be too big, so is scaled down. Text boxes on Home page require repositioning, text on join page requires resizing

    - Working on the about page was tricky as I'd had difficulty getting them centred and aligned already and had used pixel measurements for diameter rather than percentages. I could format the main 2 divs of Meetings and Info to fill the width at 100%, however the meeting information, situated inside the meeting div would not centre with the display and position styling I was applying. When looking for a fix I stumbled on the below Stackoverflow and used the align-items and justify-content while changing the parent div's display to flex to reach the goal.
[Stackoverflow centering](https://stackoverflow.com/questions/4980525/css-center-display-inline-block)

    - The finds page follows a similar structural change, instead of displaying all three top finds horizontally, they are now displayed vertically and centrally aligned. There was scope for 2 to be displayed side by side on a tablet but as there was only three in total, this would have looked strange structurally. This is a feature that could be added when more finds are implemented onto the website.

    - Title was chosen to be hidden when below 900 pixels as the club name 'DMDC' is still visible on central logo, and stacking elements in the header would have looked worse than omitting the title.

    - The logo size shrink was done because it had a set width and height so it become overbearing on smaller screens. It did however still need to be present as on a smaller display the 'DMDC' title had already been removed, so some branding would have to remain.

    - One aspect that was ignored at this stage was viewing the website on larger devices with a higher resolution. When doing so currently the website appears sparce and the large images do not fill their assigned borders because of their pixel measurements. This could be an area to explore should the project be revisited but it was considered a large time investment for minimal benefit at this point.

### Lighthouse testing
When running the deployed page through Lighthouse, the performance score sits at 74. This originally came through at mid 60s which was something I was keen to improve. The biggest change came when changing the file type of the large images on the site from .jpeg to .webp. The images kept their quality but were less demanding to load. Although images are already all made to size, they could potentially be further compressed should load times become an issue on the page. Not all images were converted to webp as they were already small in size. This could be another change to speed up the performance if required.
![https://i.imgur.com/fQKvMiW](https://i.imgur.com/fQKvMiW.jpg "Lighthouse rating")

### Future changes
As mentioned previously, relying upon pixel measurements did cause issues further down the line, such as site responsiveness. There was an option for me to go back and change all relevant pixel measurements to percentages / em / rem, however I was very conscious of the reward compared to time invested. This reversion would have been a very large undertaking on this project for a very small visual pay off so I decided it was not worth completing at this point. In a similar vein, I created more css rules and html classes for choices such as text styling, borders and image sizing to reduce duplicated lines of code. There was scope to take this further and aim to reduce any duplicated lines of code but again I had to consider the overall pay-off compared to time invested, and as such I decided it wasn't worth undertaking at this time.