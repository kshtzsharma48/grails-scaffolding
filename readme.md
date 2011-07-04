This is a sample project for prototyping changes to Grails scaffolding.

To build this project,
you must have the [grails-enhanced-scaffolding plugin](https://github.com/robfletcher/grails-enhanced-scaffolding)
in the same parent folder (it's used as an inline plugin).

# To-Do

## Core scaffolding

 * `rel="next|prev|first|last"` on pagination links

## Bugs

 * Autocompleted results need to re-position horizontally if window resized
 * Text in elements added by JS needs to be i18nized

## Appearance

 * Move mandatory indicator to right of form field (when not stacked)
 * Use :after to add mandatory indicator?

## Browser issues

 * Appears to be a double margin on left of button bar inputs in IE6 & 7
 * Fonts look terrible in IE8 (oddly they look OK in IE6 & IE7)
 * Left padding on buttons is wrong on iPhone (might just be xcode emulator)
 * Use `@media screen and (monochrome)` to optimise rendering on Kindle
 * Numeric inputs don't work for decimal values in webkit browsers

## Data format

 * date / time format for show & list pages

## Forms

 * use size attribute where appropriate
 * Radio groups for enums (use select when more than x values?)
 * Dates using type="date" with 3-field JS enhanced version? Datepicker?

## Enhanced experience

 * History manipulation breaks if you go back to the list page after paginating/sorting [GitHub](https://github.com/robfletcher/grails-scaffolding/issues/#issue/2)
 * Modal create/edit for related domain classes
 * Light-box show, edit, create direct from list page
 * Functional tests to ensure non-JS and JS versions work consistently
 * Autocomplete:
    * indicate that it's an autocompleter
    * open autocomplete with focus? Mouse double-click?
    * suppress remove button on autocomplete for mandatory many-to-one
    * autocomplete for enums & inList constraint?
 * FOUC prevention by fade-in with CSS transition
 * Slicker version of confirmation on delete
 * Use jQuery-UI slider if !Modernizr.inputs.range

## Navigation

 * Include nav using SiteMesh
 * All controllers in nav?
 * Primary & secondary nav for controllers / actions?
 * Highlight active state

## Mobile considerations

 * Test on iOS, Android, Blackberry, Kindle
 * Optimise inputs (e.g. not sure the autocomplete really works in iOS)

## Accessibility

## Integration

 * Use modernizr plugin
 * Declare separate resources for each jQuery plugin

## Misc

 * Get rid of inline script for delete buttons
 * Test the use of many-to-many on create as it might not work
 * Generate "edit this" links next to links to 1:m domains
 * Check that links to related objects are correct if the controller is named something other than the domain class name + 'Controller'
