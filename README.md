Useful Info:

1. clip-path maker:

bennettfeely.com

2. rgba(0.9), linear-gradient, background-position

3. set center:

 top: 40%;
 left: 50%;
 transform: translate(-50%, -50%);
 
4. use keyframe to define animations:

@keyframes moveInLeft {
    0% {
        opacity: 0;
        transform: translateX(-100px) rotate(-50deg);
    }
    80% {
        transform: translateX(20px);
    }
    100% {
        opacity:1;
        transform: translate(0);
    }
}

animation:moveInLeft;
animation-duration: 1s;
animation-delay: 1s;

backface-visibility: hidden; // used to avoid shake

5. Three Important Element
    a. responsive design: fluid layouts, meida queries, responsive images, correct units, desktop-first vs mobile-first
    b. maintanable and scalable code: clean, easy to understand, reusable
    c. web performance: less http requests, less ocde, compress code, use a css preprocessor, less images, compress images.
    
6. What happens to css when we load up a webpage?

img s1.png

7. How CSS Value Are Processed?

Each property has an initial value, used if nothing is declared.
Browsers specify a root font-size for each page,
Percetages and relative values are always concerted to pixels.
Percentages are mesured relative to their parent's font-size, if used to specify font-size.
Percentages are mesured relative to their parent's widthm, if used to specify lengths,
em are measured relative to their parent font-size, if used to specify font-size.
em are measured relative to the current font-size, if used to specify lengths.
rem are always measured relative to the documents' root font-size.
vh and vw are simply percentage measurements of the viewport's height and width.



img s2.jpg

img s3.jpg
      
img s4.jgp

Inheritance passes the values for some specific properties from parents to childer.
Properties related to text are inherited: font-family, font-size, color, etc
The computed value of a property is what gets inherited, not the declared value.
Inheritance of a property only works if no one declares a value for that property.
The inherit keyword forces inheritance on a certain property. 
The inherit keyword resets a property to its initial value.


8. Different between block, inline-block, inline?

img s5.jpg
img s6.jpg

9. 7-1 pattern?

img s7.jpg   BEM notation

10. SASS

img s8.jpg

Variables: for reusable values such as colors, font-sizes, spacing, etc
nesting: to nest selectors inside of one another, allowing us to write less code.
operators: for mathematical operations right inside of CSS.
partials and imports: to write CSS in different files and importing them all into one single file;
Mixins: to write reusable pieces of CSS code;
Functions: similar to mixins, with the difference that they produce a value that can than be used;
Extends: to make different selectors inherit declarations that are common to all of them.

img s9.jpg

11. 