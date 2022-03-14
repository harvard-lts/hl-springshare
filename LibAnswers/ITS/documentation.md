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

Admin > FAQ Groups > Edit Group Settings of desired group > Look & Feel tab
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
* Placeholder text: 'Try "e-resources" or "linked data"'
* Button text: 'Search'

### Default form
Select a form that will be visible when no results are found in the search engine.

## Home Page customizations

Edit page title and description

Add box with 'Customize FAQ List' widget (leave 'Display box without header or borders' unchecked)
* Change title
* Group
* Type
* Number of items to show
* Show question's details field: 'no'

Create box with 'Customize rich text/html' widget (leave 'Display box without header or borders' unchecked)
* Copy and paste columns.html into the source

## FAQ Page customizations

Edit page title: ```<div>{{{question}}}</div>```

Leave description blank

Edit question box:
* Box title: ```<div>{{{question}}}</div>``` (leave 'Display box without header or borders' unchecked)
* FAQ Template: copy and paste faq-template.html

Add "Reuse box"
* Select box created using columns.html