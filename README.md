# Lets Start! With Creating a File
After opening Glyphs, a window with different glyph sets will appear for you to choose which alphabet you want to make, or you can open this window later through _File > New from Glyph Sets..._

![screenshot01](images/01.png)

Select Thai and say _YES_ to _Prepare glyphs_
![screenshot02](images/02.png)
(For first time user) Before diving into editing, there are some modules you need to install for the future plugins to work. You can access them through _Window > Plugin Manager_ 

![screenshot03](images/03.png)

Then this window will appear. Go to _Modules_ located next to the search box. Then install all 4 modules, also for the future use ;-)
![screenshot04](images/04.png)

# Metric & Alignment Zones for Thai
After finishing a character, it's time to define body height and alignment zones — please see more details in [Glyphs 3 Handbook](https://cdn2.glyphsapp.com/media/pages/learn/f84e457b88-1639830290/glyphs-3.0.4-handbook.pdf). This is useful as the rest of the consonants will have heights to depend on and the vowels and tones will be easier to position. You can do this through _Font Info_. Then go to _Masters_ tab, scroll down to _Metrics_ and click the _+_ symbol on the right. (All the default specifications with the tag _Thai_ are not essential, so in this tutorial I will delete them out.)
![screenshot05](images/05.png)

A new _undefined_ input will appear. Simply click on it, then choose _Body Height_ for the _Metrics type_ and add a _Custom Name_. In this example, I put Thai.
![screenshot06](images/06.png)
![screenshot07](images/07.png)

The first input is the body height and the second input is the amount of overshoot.
![screenshot08](images/08.png)

Now you can start drawing the first vowel! It is recommended to start with saraIi as its height is usually in between the rest, so it is easier to keep as reference. You can also add 2 guidelines to easily refer to the baseline and height of saraIi.
![saraIiguidelines](images/saraIiguidelines.png)

# About Thai Tones and Vowels
Because of how Thai tones and vowels can be placed, there usually need to be more than one glyphs for each tone and vowel. 

### Top Tones and Vowels
In the case of _top tones and vowels_, there are usually
- default glyphs or normal glyphs with unicodes for the 1st floor tones and all vowels (as grammatically tones can be on top of vowels but not the other way around);
- glyphs with their names followed by ".small" for the 2nd floor tones or tones that are placed on top of vowels;
- glyphs with their names followed by ".narrow" for all tones and vowels used with ascender letters: poPla, foFa, foFan or in some case narrow letters such as roRua, woWean, khoKhai, choChang etc.

![mark_all05](images/mark_all05.png)
<sub>An example of maiTho, maiTho.small and maiTho.narrow</sub>

![mark_all06](images/mark_all06.png)
<sub>An example of maiTho, maiTho.small and maiTho.narrow in use</sub>

<!-- 
![screenshot10](images/tone-10.png)
<sub>An example of default maiTho</sub>

![screenshot11](images/tone-11.png)
<sub>An example of maiTho.small</sub>

![screenshot12](images/tone-12.png)
<sub>An example of maiTho.narrow</sub> -->

> [!NOTE]
> Not all tones may have all kinds of glyphs. This can be adjusted depending on the needs within a typeface. If non of the above glyphs fits, you can also create ".mid" width tones.

### Bottom Vowels
In the case of _bottom vowels_, there are usually
- default glyphs or normal glyphs with unicodes for all vowels;
- glyphs with their names followed by ".small" for ".short" descender letters: doChada and ToPatak.

![mark_all07](images/mark_all07.png)
<sub>An example of saraU and saraU.small</sub>

![mark_all08](images/mark_all08.png)
<sub>An example of doChada.short and saraU.small in use</sub>

<!-- ![screenshot13](images/tone-13.png)
<sub>An example of saraU and saraU.small</sub>

![screenshot14](images/tone-14.png)
<sub>An example of saraU.small</sub> -->

# About Tone-Marks
All the tones and vowels are connected to consonants with anchors called "marks." These marks act like hooks that you can place on each glyph for them to hook to another glyph. 

![mark_all01](images/mark_all01.png)

There are 2 marks placed on consonants namely _top_ and _bottom_, and they , like their names, connect to top tones or vowels and bottom vowels consecutively. You can place tone-marks on the top and bottom right corners of each consonant. 

Though it is good to note that for rounded corners of some letters, tone-marks need to be shifted inward a little bit, as in the top tone-mark in this example. 
<!-- ![screenshot15](images/mark-15.png)
<sub>top tone-mark on the top right corner of the image and bottom tone-mark on the bottom right corner of the image</sub> -->

For the top tones and vowels, there are also 2 marks and are called *top* and *_top*. It is recommended to add marks on the top and bottom of each tone and vowel, eventhough some tones are not grammatically be topped with anything. This is just to prevent user errors.
<!-- ![screenshot16](images/mark-16.png)
<sub>top tone-mark on the top right corner of the image and _top tone-mark on the bottom right corner of the image</sub> -->

![mark_all02](images/mark_all02.png)

For bottom vowels, there is only 1 tone-mark to connect to the consonant above as there is nothing beneath these vowels. This tone-mark is called *_bottom*.
<!-- ![screenshot17](images/mark-17.png)
<sub>_bottom tone-mark on the top right corner of the image</sub> -->

### How to Add Tone-Marks
After double clicking onto a glyph, you will be in that glyph page. You can type _cmd + u_ and the marks will appear in the center of the glyph. Therefore, it is recommended to create a guideline at x=200 and set the character width to 400, so that when checking them later, all the marks will be at the same place.
![mark_all03](images/mark_all03.png)

### How to Preview Tone-Marks
What if you want to preview a word or a sentence with correct mark positions? There is a free plugin called *Show Mark Preview* that allows you to display tones and vowels in place in the Edit View using Text tool (T). 

The plugin can be installed through _Window > Plugin Manager_. Then click the taps *All* and *Plugins*. Type in "Show Mark Preview" in the search box and install it.
![screenshot18](images/mark-18.png)

The Mark Preview can be turned on through _View > check Show Mark Preview_
![screenshot19](images/19.png)

### The Special Case of saraAm
SaraAm when combined with maiTho or maiTri is normally not easy to align, so the solution would be to make new alternate glyphs. This can be done in Grid View by selecting the saraAm glyph then _cmd + d_ or _Glyph > Duplicate Glyph_. SaraAm glyph will be duplicated, and you can adjust the new glyph with maiTho or maiTri.
