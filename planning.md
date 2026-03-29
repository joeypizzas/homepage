# Homepage planning

## Does your program have a user interface? What will it look like? What functionality will the interface have?

- Focus is just layout. There's a UI, but no interaction component.
- Three main sections to the page:
  - About.
  - Projects.
  - Contact section.
- Color palette is pizza focused. See CSS file.
- Pizza images from chatGPT image generation.
- Github icon from https://devicon.dev/.
- Phone, email, and external link SVGs from: https://pictogrammers.com/library/mdi/

## How do you plan to design the application state?

- N/A

## How do you plan to organize your project files?

- Simple. HTML and CSS files, nothing else.

## How do you plan to design your UI?

- Flex box on main container and oriented for columns.
- About:
  - Web:
    - Flexbox with image and about section, no gap.
    - Largest width version of the image. No art direction.
    - Absolute positioning to put text on top of the pizza image.
    - About has top/bottom padding to make it take up less veritcal space than image.
    - About uses flexbox columns for info.
    - ::before pseudo-element on the section using clippath to cropped background swoosh.
  - Tablet:
    - Two column version of css grid to better adjust placement of each element.
    - Most difficult piece is the name bleed and description wrapping.
    - Medium width version of the image, no art direction.
    - Steeper vertical swoosh on the ::before psuedo-element.
  - Mobile:
    - Flexbox with column direction.
    - Smallest width version of image. No art direction.
    - Absolute positioning again for name on top of pizza image.
    - Steepest vertical swoosh on the ::before pseudo-element. Behind only the pizza image.
- Projects:
  - Flexbox with columns for title and then card area.
  - Card area uses css grid with golden responsive layout for cards that is naturally responsive.
  - Cards themselves are the same on each viewport size. Pretty simple use of flexbox.
  - Section is otherwise naturally responsive across all three viewport sizes.
- Contact:
  - Flexbox for info and landscrape image portions.
  - Info uses flexbox columns, pretty straightforward.
  - Only difference for tablet is smaller width AND cropped portrait image.
  - For mobile:
    - Further cropped and smaller width image.
    - Flex box columns with image on bottom.
    - Some padding adjustments for image so no background color is visible.
    - Github icon is now centered, maybe? Depends on how it looks.
