## Testing

### Generic features:

#### Color Choices

    - Used [ColorSpace](https://mycolor.space/) to create a colour palette after selecting my base colour green present in the image borders. This green was chosen as an earthy tone to match the subject matter. Greens taken fromt he created palette were then used repeatadly throughout the site for continuity and aesthetics. I selected a light blue from a created palette to contrast strongly on hovered links to follow the accepted convention that the item would link elsewhere. I did NOT follow this rule on the 'JOIN US TODAY' link present on the home page as the text was instead white and the colour change was quite jarring. Instead I applied a drop shadow to the containing div element then an inner shadow when hovered to mimic a pressable button.

#### Header and Nav
    - Couple of different techniques used to try and center the DMDC logo in the Nav. First attempt was to use an <ul> element inside the <nav> element with the <nav> element set at a smaller width to work as a boundary for the links. The Home and Join <li> elements would then be targetted and floated left with Finds and About floated right. This would then create a gap in the center for the logo. Though this may have worked fine for a desktop site, I was concerned that applying a strict pixel dimention to the <Nav> element would cause issues when trying to make the site responsive.
[Tutorial followed](https://youtu.be/hp-LP8Nv18s) 

    I instead centered the logo using percentages to help with responsiveness and match my mobile wireframes. I then positioned the <a> nav links via display: 'flex' with CSS3 to create the desired effect.

#### Footer
    - Difficulty producing a footer that stayed in the correct place on all pages without individual page by page adjustment

### About Page
    - Creating the meeting info divs, because they were positioned using inline block they contained a 4px gap between divs which was related to the font-size for the page. To remove the gaps I had to set font-size to 0 for the parent div.
    - Inserting text into the parent divs for meeting and info moved the overall div position. This was remedied by inserting overflow:hidden into the CSS3.
    - Borders for div meeting blocks were not creating the desired effect as they'd double up between the divs (right 3px and left 3px creating a 6px border). Borders also didn't look as expected so internal borders were assigned the background colour with the parent meeting div being given a border instead to match other text elements on the page.

### Finds Page
    - I originally inserted the images through CSS3 as background images to the selected divs, however I changed the images to be in the HTML code to be able to apply an alt atribute.