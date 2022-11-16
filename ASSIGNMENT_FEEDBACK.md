Hi David and, of course, Cava!

Nice work! As you can see below you've nailed most requirements - there's one or two small things in the code or design that could be fixed up but as far as the code itself goes you've shown you know what you are doing.

The big issue wih the assignment as it is is the organisation of the CSS files - I've made a lengthy comment about it below and made some suggestions about how to fix it. It's mainly a case of creating new files, copy and pasting and removing duplicate code.

In summary: you've certianly shown the understanding and skills to recieve a Godkänt grade with the assignment as it is right now, but unfortunatley the CSS organisation was a requirement for a VG grade. I would like you to re-organise the CSS similarly to what I suggest below, and re-submit (ie push to guthub and tell me you want me to have another look).

If you are happy with a Godkänt grade you can leave it as it is, but it would be good for your knowledge & planning of future products to see what you can do in terms of organising those CSS files. Let me know what you want to do - and there's no time limit on any refactoring, so don't feel any pressure to get it back to me tomorrow.

*************************************

CRITERIA FOR GRADING

*************************************

GODKÄNT:
-------------------------------------

3 separate pages: ✅

A header with a page title on every page: ✅

A navigational menu every page with links to the other pages: ✅
  "My Work" doesn't link anywhere, could it be removed? Because it doesn't go any when you click on it in mobile with a screen of 375px the styling appears broken

Contact form:
    Email: ✅
    Message: ✅
    Required: ✅
    Mail to: ✅
      The message should also be required

RWD:
    Desktop: ✅
    Mobile: ✅ ❌
    Check the contact page on a mobile - the form is a bit too skinny for entering info

External CSS: ✅

-------------------------------------

VÄLGODKÄNT:
-------------------------------------

Current page indication in the menu: ❌
Add an 'active' class or something similar to the relevant menu item for each page and give it some styling

Responsive Image: ✅

RWD:
  Media Query: ✅
  Flex/Grid: ✅

Separate CSS: ❌
  Lines 0 - 77 in both files are the same, and the #1 rule in coding is don't repeat yourself. 

  Since the header & menu are the same for all 3 pages I suggest making a separate header.css with all the relevant code in it.

  Same with the footer - a separate footer.css will mean you only write the code once.

  I would also separate home page & contact styles - eg index.html doesn't have a "contact-container" so it doesn't need the styling for it.

  I would also place common styling like html, body .grid-container and the .cols - the styling that every page uses - into a "layout.css" or something similar.

  So something like:
    header.css
    layout.css
    footer.css
    about.css
    contact.css
    home.css
  
  Then import which of those a specific page needs in the head section. It's a lot better for a page to use 3 or 4 small files rather than 1 big one - easier to find things and great practice for more advanced programming languages like React JS where everything is compartmentalised into separate files.

  Directories inside projects should always be written in lower case. eg html or images. If you ever need 2 words or more in a file name always use a bindestreck . eg hompage-and-contact.css

  Semantic: ✅

Semantic Element naming: ✅

Code Style:
  HTML: ✅
  CSS: ✅
   A few empty lines and a missing indent spacee, but veery well done and easy to read