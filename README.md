# P-10 Menu for ES-DE

This is a tranlation of the Playchoice-10 menu interface for ES-DE.

My work focused on tranlating the layout so that it could be buildable in the theme engine for ES-DE.  Please refer to the `Changes Made` section below for additional details.

The original version of the UI can be found as part of the Playchoice-10 arcade hardware.

## Changes Made

- Used screenshots of Playchoice-10 menu to approximate the components that would be used build a theme compatible with ES-DE.
- Changed the helpsystem to ES-DE's native component and created a layout that tries to evoke the original helpsystem design (sadly it can't be a 1:1 translation due to differences in the theme engines)
- Added icons and badges specific to ES-DE functionality
- Created a custom set of pixel icons for the helpsystem
- Added a framework for adding additional color schemes

## **Preview**

<img src="https://github.com/user-attachments/assets/111926a1-2ff1-4fb8-b184-b8f975000d8a">

## **Configuration Options**

The theme has a simple set of options that can be changed directly from the UI Settings menu of ES-DE 

### **Variants:**

- `Theme Variant` - sets the color scheme that is used for the overall theme on all views.
   - `List` - The default variant.  A simple list.
   - `List + Boxart` - Adds the display of boxart+video to the list
 
| List | List + Boxart |
|----|----|
| ![List](https://github.com/user-attachments/assets/d6538d34-8f87-4a9b-b7ac-3dd60f57edd1) | ![List + Boxart](https://github.com/user-attachments/assets/d2b27ac6-7fa4-4009-8aa3-1060ba0873ad) |

### **Color Schemes:**

- `Theme Color Scheme` - sets the color scheme that is used for the overall theme on all views.
 
| Playchoice | Light Blue | Capcom Purple |
|----|----|----|
| <img src="https://github.com/user-attachments/assets/111926a1-2ff1-4fb8-b184-b8f975000d8a"> | <img src="https://github.com/user-attachments/assets/1ccef710-6178-43b6-9d8e-9769cb82240b"> | <img src="https://github.com/user-attachments/assets/57f4d03e-36c5-4e27-9c14-780d97c56e7e"> |

| Dark Tan | OLED | Light |
|----|----|----|
| <img src="https://github.com/user-attachments/assets/8f577b07-fbca-4f6a-81a0-524aa95e8cff"> | <img src="https://github.com/user-attachments/assets/f316036e-95f9-4586-b163-3409355f7732"> | <img src="https://github.com/user-attachments/assets/33fe0d65-a959-44f1-ab73-53d5b69bc804"> |

You can also create your own custom color scheme by following the instructions under "[Creating your own color scheme](#creating-your-own-color-scheme)"

### **Aspect Ratios:**

- `Theme Aspect Ratio` - sets the aspect ratio to match your display. This should happen automatically but can also be set manually if needed.
   - Supported Aspect Ratios:
   - `16:9`
   - `16:10`
   - `4:3`
   - `1:1`
   - `3:2`
   - `19.5:9`
 
## Additional Notes

### **Creating your own color scheme:**

1) In the resources folder you will find a template file called [colors-custom.xml](https://github.com/anthonycaccese/p-10-menu-es-de/blob/main/resources/colors-custom.xml)

2) Make a folder named `theme-customizations` and place a copy of the `colors-custom.xml` file inside that folder.  The folder structure should look like this when you are done:
   ```
   /ES-DE/themes/p-10-menu-es-de/theme-customizations/colors-custom.xml
   ```
   *Note: This structure should allow you to continue to get updates for the theme from the theme downloader while also retaining your customizations.*

3) Edit the properites in `colors-custom.xml` to create your custom color scheme
    
4) Set the `Theme Color Scheme` in ES-DE's UI Settings menu to `Custom` and you should see your custom color scheme display.  If you see an error check that the paths discussed above are correct and then check that the values you added for each property are correct and well formatted.

If you make a custom color scheme and are comfortable with sharing I would love to check it out 😊
- Please feel free to create an issue in this repo called `Custom Color Scheme: [Name of your Color Scheme]`
- Include the values you used for the properties above (xml is preferred), the background image and fonts you added (if any) and a screenshot of what it looks like.

## **Credits:**

- The included font is called ["A Goblin Appears!"](https://www.dafont.com/a-goblin-appears.font)
