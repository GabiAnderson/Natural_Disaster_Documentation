# Guide: Using Common UI

*Written by: Marissa Angell*

<br>

Table of Contents

- [Quick Reference](#quick-reference)
- [Styling Text](#styling-text)
- [Styling Buttons](#styling-buttons)

<br>



## Quick Reference

Check below for common use cases to know what type of asset to create/use:

| Scenario                                                     | What to Do                                                   |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| I would like to change what the text looks like on a page or button. | 1. Follow the steps under [Styling Text](#styling-text) to create a new TextStyle asset<br />2. Apply the style to a Common Text Block widget. |
| I would like to change the colors/images used for a text-only button for its various states (normal/selected/pressed). | 1. Follow the steps under [Styling Buttons](#styling-buttons) to create a new ButtonStyle asset<br />2. Apply the style to a UI_Default_Button widget. |
| I would like to add another element inside of a button (ex: an image), or attach additional data/variables to a button widget. |                                                              |





## Styling Text

### Steps

| Step Description                                             | Image                                                        |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| 1. Create a new blueprint class with a parent class of `CommonTextStyle`. <br /><br />When naming your new class, use the prefix `TextStyle_` (ex: `TextStyle_Scrapbook_Header`) | ![StylingText-1](images/StylingText-1.png)                   |
| 2. Edit the fields on your new `TextStyle` asset. <br /><br />Usually, you'll just want to change the `Font Family`, `Size`, and `Color` fields, but you can also do things like add an outline or drop shadow here if desired. | ![](images/StylingText-2.png)                                |
| 2.5. Replace your UI element with a CommonUI element.<br /><br />`TextStyle` assets only work with CommonUI classes, such as the `Common Text` widget. If the text you are wanting to change does not derive from one of those classes, then you will need to replace it. <br /><br />This can be done by right clicking the widget in the Hierarchy panel, hovering over "Replace with...", and selecting the proper class. If the proper class isn't one of the options, it can help to click on the class in the Palette panel first - it should then show up at the top of the list (this process is shown in the image). | ![](images/StylingText-2.5.png)                              |
| 3. Apply the style to your text.<br /><br />If your text element derives from a CommonUI class, you should see a `Style` field in the widget's Details panel. To apply your new style, simply select it from the dropdown for the field. The new style should then be automatically applied to the text. | ![](images/StylingText-3-1.png)<br />![](images/StylingText-3-2.png) |

<br>



## Styling Buttons

### Steps

| Step Description                                             | Image                            |
| ------------------------------------------------------------ | -------------------------------- |
| 1. Create a new blueprint class with a parent class of `CommonButtonStyle`. <br /><br />When naming your new class, use the prefix `ButtonStyle_` (ex: `ButtonStyle_Scrapbook`) | ![](images/StylingButtons-1.png) |
| 2. Edit the fields on your new `ButtonStyle` asset.<br /><br />Note: due to a quirk in how the class is implemented, the `TextStyle` fields here *<u>do not work</u>*. <br /><br />The workaround for this is adding an exposed field in the button widget itself, which has been done in the `UI_Default_Button` widget class. | ![](images/StylingButtons-2.png) |
| 3. Create a new button widget (or replace an existing one)<br /><br />Drag a button that derives from CommonUI's button class from the palette window onto the canvas. For the vast majority of cases, `UI_Default_Button` is the one that you'll want to use. <br /><br />If you need to replace an existing button, see step 2.5 of [Styling Text](#styling-text) for a short tutorial on how to replace widgets. | ![](images/StylingButtons-3.png) |
| 4. Apply the style to your button.<br /><br />If the button derives from CommonUI's button class, you should see a `Style` field. To apply your new style, simply select it from the field's dropdown.<br /><br />If you're using `UI_Default_Button`, you should also see a Text Style field, which is used as a workaround for the quirk discussed in step 2. Use this field to change the `TextStyle` asset that is applied to the button. | ![](images/StylingButtons-4.png) |

<br>





## Creating a New Button Widget

### Preface

If you are trying to create a button that just has a text label on it, but that uses different colors or has a different text font or background image, then you should refer to the [Styling Text](#styling-text) and [Styling Buttons](#styling-buttons) sections of this guide.  

You should only need to create a new button widget if you need a button that either:

- Will have something **other than just text** on it
- Needs to **store its own variables**

If one or both of those statements apply, then you should create a new button. For an example of a case in which this would apply, see the widget `UI_Scrapbook_Character_Button` in the folder `/Core/UI/Scrapbook/`, which fits both of the criteria above.





### Steps (Coming Soon)

| Step Description | Image |
| ---------------- | ----- |
|                  |       |
|                  |       |
|                  |       |
|                  |       |

<br>

















