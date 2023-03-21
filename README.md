# Colors Library 
The css color library contains about css colors along with their color shades which can be applied on texts, backgrounds, element borders and outlines using predefined utility classes. Several utility classes are used to apply this colors for hover and non-hover effects. Other relative utility classes are used to apply color opacity or used in color mixing. The 
specified colors along with opacity controller classes both provide the ability to generate new colors through 
color layers.

#### Color Definition Classes
Colors are defined based on two main formats

   + Color shades specified with ```-d```, ```-dd``` for darker colors 
   + Color opacity specified with color shade suffixed with ```o-``` 

#### Color Application Classes
Colors can be applied for: 

   + Backgrounds specified with  ```bc-```, ```bch-```, ```bco-``` and ```bho-```   
   + Texts specified with  ```c-```,  ```ch-```, ```co-``` and ```ch-```
   + Borders specified with  ```bd-```, ```bdh-```, ```bdo-``` and ```bdho-```
   + Outlines specified with  ```oc-```, ```oh-```, ```oco-```, ```oho-```

    ##### Text Colors 
    Text colors can be applied with the ```c-``` class or ```ch-``` color hover class followed by any of the supported color names (e.g c-red). However, color effects are applied based on hover and opacity level. The ```co-``` and ```cho``` classes apply color based on color opacity level and color hover opacity level respectively. While ```co-``` will apply opacity for ```c-``` utility group, the ```cho``` applied opacity for 
    ```ch``` hover utility group.

    ##### Background Colors 
    Similarly to text colors, background colors can be applied with the ```bc-``` or ```bch-``` background color hover class followed by any of the supported color names. However, background color effects are applied based on hover and opacity level. The ```bch-```, ```bco-``` ```bho-``` classes apply color based on color hover effect, color opacity level and color hover opacity level respectively. 

    + Dark mode background color overlays can be specified with the ```ov-d``` classes while light mode can be specified with ```ov-l``` classes. Applicable values suffixes ranges from lowest ```1``` to highest ```8```. 
    For example, ```ov-d1``` sets a dark background with opacity of 0.1 while ```ov-l1``` sets white background with opacity level of 0.1.

    ##### Border Colors 
    The border colors can also be applied with the ```bd-``` class followed by any of the supported color names. The border color effects are applied based on hover and opacity level. The ```bdh-```, ```bdo-``` ```bdho``` classes apply color based on color hover effect, color opacity level and color hover opacity level respectively. 
    
    + Border colors can also inherit border colors from parent element through the ```bd-i``` class or ```bd-ih``` hover class.
    
    + Naturally, border colors not specified will inherit colors from the text color. However, when hovered upon borders can inherit colors from the current text color through the ```bd-ch``` class.

    + To remove borders entirely from an element, the ```bd-f``` class can be applied

    ##### Outline Colors 
    The outine colors can be applied just like the borders. It uses the ```oc-``` class followed by any of the supported color names to apply colors. The ```oh-```, ```oco-``` and ```oho-``` classes apply color based on color hover effect, color opacity level and color hover opacity level respectively.
    
    + Outline colors can inherit outline colors from parent element through the ```oc-i``` class or ```oc-ih``` hover class.
    
    + Naturally, outline colors not specified will inherit colors from the text color. However, when hovered upon outlines can inherit colors from the current text color through the ```oc-ch``` class.

    + To remove outlines entirely from an element, the ```oc-f``` class can be applied

    ##### Transparent Colors 
    Transparent colors are specified with the ending ```t``` directive for specified color utility classes. 
    
    + ```ct``` color transparent
    + ```bt``` background color transparent
    + ```bd-t``` border color transparent
    + ```bdh-t``` border hover color transparent

     .

#### Outlines and offsets
Outline offsets are controlled with the ```oo-``` class which sets the offsets in pixels for the outline property of an element. The ```ooh-``` however, sets the offset for hover mode. The outline's offset value runs from one(1) 
to nine(9). For example, ```oo-1``` will set outline offset of 1 pixels on an element using the outline property while ```ooh-``` will apply offset only when element is hovered upon. Offsets can also be applied with the "em" unit. This is specified by ```oo-em-``` or ```ooh-em-``` for hover. In the case of "em" unit, values run from ```d1``` to ```d9``` and ```1``` to ```2``` with decimals specified with ```d```. Hence we have  ```oo-em-d1``` to mean an offset of 0.1em while a value of ```oo-em-1d1``` will mean offset of 1.1em. The highest value which is ```oo-em-2``` is the highest offset level that can be applied. 

#### Outlines and offsets
Outline offsets are controlled with the ```oo-``` class which sets the offsets in pixels for the outline property of an element. The ```ooh-``` however, sets the offset for hover mode. The outline's offset value runs from one(1) 
to nine(9). For example, ```oo-1``` will set outline offset of 1 pixels on an element using the outline property while ```ooh-``` will apply offset only when element is hovered upon. Offsets can also be applied with the "em" unit. This is specified by ```oo-em-``` or ```ooh-em-``` for hover. In the case of "em" unit, values run from ```d1``` to ```d9``` and ```1``` to ```2``` with decimals specified with ```d```. Hence we have  ```oo-em-d1``` to mean an offset of 0.1em while a value of ```oo-em-1d1``` will mean offset of 1.1em. The highest value which is ```oo-em-2``` is the highest offset level that can be applied. 

#### Borders
Borders property such as thickness and positional transparency can be applied with specific utility classes.

   ##### Border Thickness
   Border thickness is handled by the  ```bd-``` utility class followed by a value within the range of 1 to 12. For example, a value of ```bd-10``` will set the border thickness of an element to 10 pixels. For borders thickness, there is no available hover effect class specified but color opacity can be specified through the ```bdo-``` or ```bdho-``` classes. 

   ##### Border Transparency 
   Border tranparency is specified by setting the positional transparency after the thickness level has been specified. In order to achieve this, the following utility classes can be applied. 

   +  ```bd-xs``` sets the top and bottom borders to transparent
   +  ```bd-xl``` sets the top, bottom and right borders to transparent
   +  ```bd-xr``` sets the top, bottom and left borders to transparent
   +  ```bd-vs``` sets the right and left borders to transparent
   +  ```bd-vt``` sets the right, left and bottom borders to transparent
   +  ```bd-vb``` sets the right, left and top borders to transparent

#### Working with color opacity
Color opacity can be defined with specific opacity values that runs from one(1) to ten(10). One is the highest while ten is the lowest. The list below can be used as reference when working with color opacity. 

   + ```1``` sets opacity level to 0.9
   + ```2``` sets opacity level to 0.8
   + ```3``` sets opacity level to 0.7
   + ```4``` sets opacity level to 0.6
   + ```5``` sets opacity level to 0.5
   + ```6``` sets opacity level to 0.4
   + ```7``` sets opacity level to 0.3
   + ```8``` sets opacity level to 0.2
   + ```9``` sets opacity level to 0.1
   + ```10``` sets opacity level to 0

Once we are familiar with the color opacity utility classes such as ```co-```, ```cho-```, ```bdo-```, ```bdho-```, ```oco-``` and ```oho-``` classes, we can apply any of the color opacity values specified above.

#### Helper List 
The following lists provides easier description of the color classes 

   + ```c-``` sets text color
   + ```ch-``` sets text hover color
   + ```co-``` sets text color opacity
   + ```cho-``` sets text color hover opacity
   + ```bc-``` sets background color
   + ```bh-``` sets background hover color
   + ```bco-``` sets background color opacity
   + ```bho-``` sets background color hover opacity
   + ```bd-``` sets border color, thickness level or inheritance
   + ```bd-ch``` sets border color inheritance from font color
   + ```bd-xs``` sets the top and bottom borders to transparent
   + ```bd-xl``` sets the top, bottom and right borders to transparent
   + ```bd-xr``` sets the top, bottom and left borders to transparent
   + ```bd-vs``` sets the right and left borders to transparent
   + ```bd-vt``` sets the right, left and bottom borders to transparent
   + ```bd-vb``` sets the right, left and top borders to transparent
   + ```bd-f```  removes borders entirely
   + ```oc-``` sets border color, thickness level or inheritance
   + ```oc-ch``` sets border color inheritance from font color
   + ```oc-f``` removes outline entirely

#### Color List 
Colors are specified by color shades which ranges from a selected color to a dark shade ```-d``` or darker shade 
```-dd```. There are about 116 colors and shades. While the 116 colors will not be listed, the selected base colors are listed below: 

   + ```black```
   + ```white```
   + ```off-white```
   + ```blue```
   + ```red```
   + ```yellow```
   + ```green```
   + ```orange```
   + ```purple```
   + ```violet```
   + ```magenta```
   + ```teal```
   + ```lime```
   + ```indigo```
   + ```pink```
   + ```aqua```
   + ```bronze```
   + ```silver```
   + ```gold```
   + ```gold```
   + ```brown```
   + ```crimson```
   + ```grey```
   + ```grey```
   + ```ivory```
   + ```maroon```
   + ```olive```
   + ```sea-green```
   + ```sea-blue```
   + ```tan```
   + ```blue-violet```
   + ```dry-blue```
   + ```steel-blue```
   + ```dodger-blue```
   + ```deep-blue```
   + ```deeper-blue```
   + ```rebecca-purple```
   + ```slate-grey```
   + ```red-orange```

   > Each of the colors above may be stepped down to dark shade with the ```-d``` or darker shade ```-dd``` suffixes. For example, a dark shade of  ```teal``` is ```teal-d``` while a darker shade is the ```teal-dd``` class. This color can then be applied for either backgound, text, borders or outlines using the relative property idenfiers. For example: 

   + A color of ```teal``` will be ```c-teal```
   + A dark color ```teal-d``` will be ```c-teal-d```
   + A darker color ```teal-dd``` will be ```c-teal-dd```

   > By using the formats above we can also apply colors for backgrounds, borders, outlines and hover effects. This also makes it easier to control opacity level of each colors through relative color opacity levels