# Screens

<blockquote>
<strong>Summary</strong>: Screens are the primary building block of the app. Almost all pages will be made from a screen.
</blockquote>

## Overview
### Components
Components represent the individual parts that can populate your screen. They can be layout components like columns and paddings, or interactable components like buttons and text.<br>
[Learn More](././overview/screens/components/index)

### Layout
There are two layout styles you can choose for your screen. Be sure to set the layout type if needed and follow the following guidelines.
#### Regular
Screens are made up of a list of rows. When a screen is loaded it makes a call to the server for data based on the url passed in. Each entry in the data returned duplicates the set of rows. This leads to a list of cards representing each card representing a lsit or rows filled by one data entry.

#### Freeform
This option allows you to set the visuals to whatever you want intstead of the card list version of regular. This is achieved by only using the first Row of the primary rows list. This row will be treated as if it is a container you can define any visual structure you want in as if it was a normal flutter container.
## Tutorial
If you would like to learn how to create a basic screen. Please check out the following tutorial.<br>
[Create a Screen Tutorial](./tutorials/create_a_screen/index)

## Additional Settings 
### Additional Settings
<pre>
    - <strong>setType</strong>: PageTypes
        - <strong>regular</strong>: Uses multiple predefined rows that repeat a set of data
        - <strong>freeform</strong>: Only uses the first row so you have more control over layout
    - <strong>setPageIcon</strong>: MaterialIconsEnum
    - <strong>setVisibility</strong>: If visibility false, don't show on front pages rotation
    - <strong>setSelectable</strong>: allows card to be selectable
    - <strong>setUpdatable</strong>: adds an update timer to regular pages
</pre>