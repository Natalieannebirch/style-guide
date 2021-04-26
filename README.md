# CSS Style Guide

## Structure
Each CSS File should have a comment block at the top of the page containing simple project/file information such as the project name and when it was last updated, with a short description of the changes made. 

    /* -------------------------------------------------
    Project: Project Name

    Last Change: 4/25/2020 [mobile menu animations and transitions added]

    -----------------------------------------------------*/
Typography, Color Glossaries, and other comment reference are added to the top of the file after the project information.  
Divde code into groups as listed below. Add groups and dividers as needed.

1. Global Styles and Resetting
2. Text Sizes and Headings
3. Header 
4. Navigation
5. Body Elements as needed
6. Footer
7. Media Queries


## Selectors
Selectors should be on a single line, with a space after the last selector, followed by an opening brace. A selector block should end with a closing curly brace that is unindented and on a separate line. A blank line should be placed between each selector block. Short blocks of code should be on one line.

    .selector-a {
      display: flex
      color: #fff;
      background-color: #000;
    }
### Naming
Class selectors should always be used for css, ID attributes should only be used for JavaScript and PHP purposes.  Class Names should be in lowercase with a dash separating words. 

    .selector-name {
       css rules
    }

### Indenting
Selectors should only be indented when selecting a child element of the parent class. The number of indents should reflect the amount of child or nested elements. 

    .selector {
    }

    .selector p{
    } 

    .selector p span {
    }

With that being said, selectors should always be specific and classes should be used as often as possible. Nesting should never happen for more than three levels.

### Multiple Selectors 

When using multiple selectors, each selector should be on its own line ending in either a comma or an space and opening curly brace

    selector1,
    selector2,
    selector3 {
    }
    
## Properties
Properties should be in lowercase. Use hex colors and rgba() when opacity is needed. RGB should be avoided completely and hex colors should be shortened when able to. 

### Ordering 
Properties should be in a specific order to reflect meaningfulness and intent behind the declarations. The order is as follows:
- Display
- Positioning 
- Box Model ( margin, padding, content, etc.) 
- Colors
- Typography 
- Misc. 



## Commenting and Titling

### Comments
Comments should be easy to distiguish from code and used frequenty for changes, seperation, and general notes. Use a line length of dashes ( - )for opening and closing comment tags to make sure it is easily visible when scanning through code. Comment Reference Blocks should have a title, while general notes do not need one.
   
           
        /* ------------------------------------------------
            [Comment Title]
            
            This is a comment that is easy to see.
        ---------------------------------------------------- */
        
### Titling
Each Section as mentioned in the structure should have a title in a comment block. Titles should start with the $ character, and be in uppercase to make them easy to find.

        /* ------------------------------------------------
            $HEADER
        ---------------------------------------------------- */
        .style-1{
        }

## Fonts and Colors
Create a color glossary at the top of each file containing the project with their color codes and a basic definition of what they are used for.  
        
        /* ------------------------------------------------
            [Color Glossary]
            
            Light: #F2D8C9 - text, buttons

            Secondary-Light: #E3A083 - footer, text

            Dark: #A66257

            Dark Grey: #515151 - primary text color
        ---------------------------------------------------- */
Create a similar Typography glossary in the top of each file as well, with corrosponding text-sizes according to be used for headings, paragraphs, etc.

    /* -------------------------------------------------
      [Typography]

      Quicksand Regular, Quicksand Bold - Google Fonts

      Headings: 50px / 3.125 em decreasing 10px

      Body: 16px / 1em
    -----------------------------------------------------*/
    
  
