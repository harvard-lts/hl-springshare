# Initial Setup

## 1. Include styles

### If want styles to change system-wide:

#### Admin > System Settings > Look & Feel
* Custom JS/CSS: copy and paste in styles from 'style.css'
* Custom Header Code: copy and paste in new html from 'header.html'
* Custom Footer Code: copy and paste in new html from 'footer.html'

#### Admin > FAQ Groups > Edit Group Settings of desired group > Look & Feel dropdown
* Include system-level JS/CSS code on this group's pages: Yes
* Include system-level Header code on this group's pages: Yes
* Include system-level Footer code on this group's pages: Yes

### If only want styles to change for specific group(s):

Admin > FAQ Groups > Edit Group Settings of desired group > Look & Feel dropdown
* Include system-level JS/CSS code on this group's pages: No
* Include system-level Header code on this group's pages: No
* Include system-level Footer code on this group's pages: No
* Custom JS/CSS: copy and paste in styles from 'style.css'
* Custom Header Code: copy and paste in new html from 'header.html'
* Custom Footer Code: copy and paste in new html from 'footer.html'

## 2. Pages tab configuration
Admin > FAQ Groups > Edit Group Settings of desired group > Pages tab

*Check box that says "Use advanced customization options"*

### Search Layout

"Traditional (LibAnswers-only results)"

### Colors

* Box Header Background Color: #FFFFFF
* Box Header Color Color: #FFFFFF
* Box Header Text Color: #1E1E1E
* Box Header Link Color: #0579B8
* Box Header Active Link Color: #0579B8

### Default search box

* Group content to search: 'Default'
* Form Label: 'Ask Another Question'
* Placeholder text: ['Try "EXAMPLE SEARCH TERM 1" or "EXAMPLE SEARCH TERM 2"']
* Button text: 'Search'

### Default form
Select a form that will be visible when no results are found in the search engine.

## 3. Home Page customizations

Edit page title and description

Add box with 'Customize FAQ List' widget (leave 'Display box without header or borders' unchecked)
* Change title -- "More Help"
* Group
* Type -- Custom FAQ entries list
* List FAQ IDs you want to display
* Show question's details field: 'no'

Create box with 'Customize rich text/html' widget (leave 'Display box without header or borders' checked)
* Box title -- Can't find what you're looking for?
* Rich text in box -- "
Can't Find What You're Looking For?
We are here to help! Please submit a ticket to request help. The support desk is staffed during regular business hours (Monday – Friday, 9 am to 5 pm).
"

Create box with 'Question Form' (leave 'Display box without header or borders' checked)
* Box title -- "Embedded question form"
* Question Form -- select "LTS General"

## 4. FAQ Page customizations

Edit page title: ```<div>{{{question}}}</div>```

Leave description blank

Edit question box:
* Box title: ```<div>{{{question}}}</div>``` (leave 'Display box without header or borders' unchecked)
* FAQ Template: copy and paste faq-template.html

Add "Reuse box":
* Select box created for home page "Can't find what you're looking for?" blurb

Add "Contact info box":
* Type of contact -- Question form link
* Icon -- Use Upload image link to select 'link-out-icon_resized.png' icon from folder "Shared Library > LTS"
* Link text -- "Submit a help request to LTS Support"
* Queue -- LTS General

## 5. Single Search Page customizations

Edit page title: "Search Results" (leave 'Display box without header or borders' checked)

Add "Reuse box":
* Select box created for home page "Can't find what you're looking for?" blurb

Add "Reuse box":
* Select box created for FAQ page contact info link to help form

## 6. Considerations if using this as a guide for a different LibAnswers instance
Review the custom.css file to find references to unique IDs and classes. These will have to be replaced with the IDs and classes that appear in your instance. I would suggest using find & replace with this.
