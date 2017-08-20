# bulma-switch
Bulma's extension to display checkbox as a toggle button

![Switch example](switch-example.png)

Usage
---

```html
<div class="switch">
  <input id="yes-no" type="checkbox" name="exampleSwitch">
  <label for="yes-no">Yes / No</label>
</div>
```

Modifiers
---
You can use following modifiers (in addition to Bulma's color modifiers):

Name | Description
-----|------------
is-outlined | No background - just borders
is-rounded | rounded borders
has-label-bottom | Display the label text at bottom

Variables
---
This extension uses Bulma's color modifiers and have the following variables

Name | Description | Default value    
-----|-------------|---------------
$switch-background | $grey-light
$switch-background-active | $primary
$switch-radius | $radius
$switch-margin | 1rem
$switch-paddle-background | $white
$switch-paddle-offset | 0.25rem
$switch-paddle-transition | all 0.25s ease-out

Demo
---
You can find a demo [here](https://codepen.io/wikiki/pen/ZJrPVq)

Integration
---
- Clone the [bulma repo](https://github.com/jgthms/bulma)
- Under the `sass` folder, create a new folder called `extensions`
- In this new folder, create a new file `switch.sass`
- Copy the code form the `bulma-switch repo`'s [switch.sass](https://github.com/Wikiki/bulma-switch/blob/master/switch.sass) file into your new file
- In the same folder create a new file `_all.sass` (this is not required, but will help when you add more extensions)
- In this file add this code:
```
@charset "utf-8"
@import "switch.sass"
```
At the end of the `bulma.sass` file, add this line: `@import "sass/extensions/_all"`

Now, you can just build the bulma project with `npm run build`, and the output will be available in the `css folder`.
