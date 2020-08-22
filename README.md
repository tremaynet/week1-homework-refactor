README

Included: 
All source files (.css .html. .png, .jpg)
this README

Homework #05

List of design and Functional requirements:
1. Web accessibility 
2. Ensure people with scio-economic restrictions have access to their website
3. Help tp avoid litigation 

references used to support the refactoring effort:
 https://www.w3.org/WAI/fundamentals/accessibility-intro/ for information on Web Accessibility

Tools used:
ChromeVox Extension - Screen reader used to assist and validate this page is developed to support visually impaired users.  
Added the Reset CSS sytle sheet to the index.html file for this project to reduce browser inconsistencies. For detailed information please see:  https://meyerweb.com/eric/tools/css/reset/ for additional surronding the Reset CSS tool.
Alt text and Title applied to the folling images and figure classes:
    Index.htm 
        1. line 6 <link rel="stylesheet" href="./assets/css/reset.css">
        2. line 8 added a title that defines the services offered by Horeiseon
        3. line 32 <figure class="stockimage" title="Picture of Team Horiseon"></figure>
        4. line 37 <img src="./assets/images/search-engine-optimization.jpg" class="float-left" alt="Laptop notebook pencils coffee"/>
        5. line 44 <img src="./assets/images/online-reputation-management.jpg" class="float-left" alt="Human laptop phone"/>
        6. line 51 <img src="./assets/images/social-media-marketing.jpg" class="float-left" alt="Humans Collaborating Working Sharing Ideas"/>
        7. line 63 <img src="./assets/images/lead-generation.png" Alt="Lead Generation funnel icon"/>
        8. line 70 <img src="./assets/images/brand-awareness.png" alt="Lightbuld beacon discovery icon"/>
        9. line 77 <img src="./assets/images/cost-management.png" alt="Machine gear with icons"/>
        
4. Always leave the code you are editing a lotter cleaner than you found it
5. improve their codebase for long term sustainability
Method: #4 #5
Employed the use of semantic HTML to the existing code base and comments:
    Index.html 
        1. line 11 Replaced the original <div> tag with the <header> tag to identify the introductory contents (i.e.; Logo and heading elements.) 
        2. line 15 Replaced the <div> element on the original index.htm with the <nav> tag to group together the main navigation links aka internal links defined in lines 16, 19 and 22
        3. line 32 <div> tag was changed to the <figure> to identify content related to but separete from the main content flow.
        4. line 35 <div> replaced with <main> to group together the content in the main flow identified in lines 36 - 56 where the <section> tag was used to identify the related content relative to the main content. Additionally the use of the section <section> element is used for outline purposes and not for styling purposes. 
        5.Lines 36, 43 and 50 I removed the <div class> from the orignal configuration as a class and id properties were not needed to support the sites functionality. 
        6. line 37 I changed the class of float-right to float-left to align with line 37 and 51
        7.Line 60 change the <div> to <aside> as this is information that is related to but separate from the other content on the page
        8.lines 61 - 81 I replave the <div> with <section> to identify the information that is relative to the aside content
        9. line 85 replaced the <div> with the <footer> as it contain the Author and copyright related information
    
6. Ensure that all links are functioning correctly 
    1. Internal link on line 18, 21 and 24 are linked to the ids on line 36 and 50. The was tested locally and after being published to github

7. Clean up the CSS to make it more efficient
8. Consolidate CSS selectors and properties
    style.css #7 #8
        1.  line 27 changed the css selector from .header div to .header nav
        2.  line 35 changed the css selector from .header div ul to .header nav ul
        3.  line 35 changed the css selector from .header div ul to .header nav ul li
        4.  line 49 changed selector name to .stockimage
        5.  line 64, 73 and 77 change the consolidated all selectors and added each class to each selector and associated them with the appropriate ID this allowed for consoidation and makes the code more efficient 
        6. Removed selector .float-right based on #6 in the aformention sections
        7.  line 98 consolidated .benefit-lead, .benefit-brand, .benefit-cost into the same selector
        8. line 103 consolidated .benefit-lead h3, .benefit-brand h3, .benefit-cost h3 into the same selector
        9.  line 109 consolidated .benefit-lead img, .benefit-brand img, .benefit-cost img into the same selector
        10. lines 31, 68, 94, 122 the font families did not match and were not in the same order. I aligne all three to match
        11. line 115 re-ordered the p selector to be lower in order so that it would set the font size for the contents in the <main> and <aside>
        12. line 98 increased the margin-bottom to 32px to aling with main conent
        13. Reordered CSS to match the flow of the HTML file 


9. Organize the CSS selectors to follow the semantice structure of the HTML elements 
10. Included comments before each element or section of the page - see #4



