# Game UI Export Guide

This is a guide for UI/UX Artists and Designers when they need to send their exported files to the programmers that need to implement them in game.

Most of the things you will find here might seem "common sense" but it has happened before that my common sense and your common sense are not exactly aligned.

# Resolutions and Aspect Ratios

## Glosary
- **Aspect Ratio**: written as `W:H` means how wide is something compared to it's height.
- **Orientation**: Portrait or Landscape.
    - **Portrait**: An aspect ratio that is taller than wider. e.g. `9:16`, `9:18.5`, `3:4` (The second number is always larger)
    - **Landscape**: An aspect ratio that is wider than taller. e.g. `16:9`, `18.5:9`, `4:3` (The first number is always larger)
    - **Square aspect ratios will be considered both Portrait and Landscape at the same time** (`1:1`)
- **Resolution**: written as `WxH` means the amount of pixels something has.
- **to scale something**: when this guide says that something will be scaled, assume it will be scaled uniformly, respecting the original aspect ratio.
    - **scale to fit**: when something is scaled to fit it will cover as much as possible without cropping content, in other words no content will bleed out of the target.
    - **scale to fill**: when something is scaled to fill it will cover the target but some cropping or bleeding can occur if the aspect ratio isn't the same.
- **to stretch something**: when this guide says that something will be stretched, it will be scaled without respecting the original aspect ratio.
- **Responsive Design**: This will also encompass "fluid" designs. The content is meant to "flow" and use effectively as much of the screen as possible. Mostly based on "flexboxes" similar to web design. e.g. An inventory grid will have more or less columns depending on the width of the device.
- **Adaptive Design**: The content will change its shape to accomodate for certain aspect ratios. Mostly used for games that should support both landscape and portrait aspect ratios. e.g. On landscape buttons are on a sidebar while on portrait the same functionality is now in a bottom tool bar.
    - **Aspect ratio Breaks**: The limit on which the content will change shape.
- **Fixed Design**: Content that is designed with a "desired" or "perfect" resolution in mind. This can only be scaled. While this might be the easiest way to design and code UI, it will provide a less user-friendly experience across diferent devices (for example, buttons too small to be pressed on a mobile device or buttons that are comically large on a computer screen)

## Guidelines

- Ideally the entire project should have a consistent "desired" resolution. This will avoid some assets looking pixelated for no reason.
    - If the UI is designed in a vector based program (e.g. Illustrator, Figma), this can be fixed during export, but on raster based programs (e.g. Photoshop) this must be considered from the start.
- You can mix Responsive, Adaptative and Fixed design, but you must explain where to use each.
    - For Responsive designs include the "ideal" case along with the limits for the worst case scenarios. e.g. the inventory grid is meant to have more or less columns depending on the width of the screen _but must never have less than 3 nor more than 6 columns_.
    - For Adaptative designs include the aspect ratio breaks and mockups on how each break should look like.
    - For Fixed Designs please state the "ideal" or "desired" resolution. (Hopefully the same for the entire project) 

# Mockups

## Glosary
- **Full Mockup**: A static visual representation of how the final screen should look.
    - **Partial Mockup**: An isolated example of how a single element should look.
- **Animation Storyboard**: A static visual representation of how the design should animate. Comic book style frames, arrows and annotations can be used.
- **Placeholder**: Any non-final piece of content.
    - **Placeholder Marker**: A way to clearly mark a piece as a placeholder and not meant to be reproduced in the final design. e.g. "Lorem Ipsum" will be always considered placeholder.
- **Redlines**: (also "Redlining") is marking up a UI design mockup by adding red lines indicating spacing and sizing of design elements.

## Guidelines
- Any placeholder item shown in a mockup must be obviously a placeholder. While "Lorem Ipsum" will be always considered a placeholder, for images consider having the word "placeholder" somewhere in de design.
- For Responsive designs include mockups for the ideal case and the edge/worst cases
- For Adaptative designs include mockups for all breaks
- Animations must be explained or showcased in animation storyboards if the animation is too complex.
- When sending subtle corrections of a mockup, please include another mockup with markups explaining what changed. 

# Text and Fonts

## Glosary
- Kerning
- Alternates
    - Ligatures
- Font File
- (Sans) Serif
- Grunge
- Type Modification

# Colors

## Glosary
- **RGB**: Short for "Red" "Green" and "Blue". References a color by their color values ranging from 0 to 255.
- **Hex Color**: The RGB color expressed in hexadecimal format, usually with a `#` or `0x` at the beginning. The values range is from `00` to `FF` per color.
- **Alpha**: The opacity for a color

# Assets

## Glosary
- **Editable**: The raw source files used to make the design.
- **Exported**: The hand-off content that will be integrated in the game.
- 

## Editables

## Exported

### Buttons

### Frames

### Stuff