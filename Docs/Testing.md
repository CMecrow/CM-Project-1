## Testing

### Generic features:

#### Color Choices

    - Used [ColorSpace](https://mycolor.space/) to create a colour palette after selecting my base colour green present in the image borders. This green was chosen as an earthy tone to match the subject matter. Greens taken fromt he created palette were then used repeatadly throughout the site for continuity and aesthetics. I selected a light blue from a created palette to contrast strongly on hovered links to follow the accepted convention that the item would link elsewhere. I did NOT follow this rule on the 'JOIN US TODAY' link present on the home page as the text was instead white and the colour change was quite jarring. Instead I applied a drop shadow to the containing div element then an inner shadow when hovered to mimic a pressable button.

#### Header and Nav
    - Couple of different techniques used to try and center the DMDC logo in the Nav. First attempt was to use an <ul> element inside the <nav> element with the <nav> element set at a smaller width to work as a boundary for the links. The Home and Join <li> elements would then be targetted and floated left with Finds and About floated right. This would then create a gap in the center for the logo. Though this may have worked fine for a desktop site, I was concerned that applying a strict pixel dimention to the <Nav> element would cause issues when trying to make the site responsive.
[Tutorial followed](https://youtu.be/hp-LP8Nv18s) 

    I instead centered the logo using percentages to help with responsiveness and match my mobile wireframes. I then positioned the <a> nav links via display: 'flex' with CSS3 to create the desired effect.

