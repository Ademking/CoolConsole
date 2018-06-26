<div align="center">
<a href="https://www.emojione.com/emoji/1f410">
<h1>CoolConsole.js 😎</h1>
<img alt="CoolConsole" src="https://i.imgur.com/BccwhSM.gif" />
</a>
<p>😎 CoolConsole Library : The Coolest Browser Console ever </p>
</div>

# What is CoolConsole?

This Library lets you write Beautiful "console.Log()" in your Google Chrome Console without the hassle of having to add CSS styles or SVG icons.


## Table of Contents

* [Dependencies](#dependencies)
* [Getting Started](#getting-started)
* [Usage](#usage)
    * [Basic Usage](basic-usage)
    * [Advanced Usage](advanced-usage)
* [List Of Styles](#list-of-styles)
* [List Of Icons](#list-of-icons)
* [Note](#note)
* [License](#license)
* [Contributing](#contributing)


## Dependencies
There are no other libraries that CoolConsole is dependent of 😉

## Getting Started
There are several ways to start using CoolConsole. You can:
* Download the CoolConsole library from  [Here]("#")
* Include CoolConsole from a CDN. If you don't want to download and host CoolConsole yourself, you can include it from a CDN (Content Delivery Network).

The CoolConsole library is a single JavaScript file, and you reference it with the HTML 

```javascript
<html>
    <head>
        <script src="CoolConsole.js"></script>
    </head>
    <body> 
        ... 
    </body>
</html>
```
## Usage

You Have Plenty of Options 😎👌

> ### Basic Usage

### cc() :

Default CoolConsole (with multi texts and styles)

**cc ( TEXT , [ STYLES ... ] ) ;**

There are 2 types of params : **STYLES (Optinal)** and **TEXT**
    
    TEXT {style}    : Text you want to write

    [ STYLES ]  {*} : (Optional) you can check list of STYLES [here](#list-of-styles)
    
    
* Example :

```javascript
    cc("Hello World", bold, large, red, underline);
    // this line will generate console.log message with bold, large, red , underline style
    // see result below
```
![](https://i.imgur.com/HlYxDMD.png)

you can also write multiple texts with multiple styles :

**cc(  FistText ,  [ STYLES... ], SecondText , [ STYLES... ] , Nth-Text, [ STYLES ...] );**

* Example :

```javascript
    cc("CoolConsole", bold, bg_red, white , large ," is the Coolest", red, medium);
    // this line will generate console.log message with :
    // bold, red background, white text , large size "CoolConsole
    // red, medium size "is the Coolest"
    // see result below
```

![](https://i.imgur.com/vjzVnZa.png)

------


### cc_primary() - cc_success() - cc_info() - cc_warning() - cc_danger() - cc_error()

Like CSS Frameworks like **Bootstrap**, **Foundation**, etc... 
Theses functions lets you generate colorful Console.log messages for your needs :

**cc_primary ( TEXT , [ TITLE ] , [ CUSTOM TITLE ] );**

**cc_success ( TEXT , [ TITLE ] , [ CUSTOM TITLE ] );**

**cc_info    ( TEXT , [ TITLE ] , [ CUSTOM TITLE ] );**

**cc_warning ( TEXT , [ TITLE ] , [ CUSTOM TITLE ] );**

**cc_danger  ( TEXT , [ TITLE ] , [ CUSTOM TITLE ] );**

**cc_error   ( TEXT , [ TITLE ] , [ CUSTOM TITLE ] );**

    TEXT {string} : the text you want to write

    [TITLE] {boolean}: (Optional) if you want to add Default Title (Picture Below)
    
    [CUSTOM TITLE] {string} : (Optinal) if you want to add your custom Title (TITLE must be true)

* Examples :

```javascript
    cc_primary("Hello Folks !");
    // this line will generate console.log message with Primary Style (Without Title)
    cc_info("2 + 2 is 4 Minus 1 Dat's 3 Quick Maths" , true);
    // this line will generate console.log message with Info Style (With Default Title)
    cc_danger("Boooooooooom !" , true, "Explotion");
    // this line will generate console.log message with Danger Style (With Custom Title)
```

![](https://i.imgur.com/9xjNxA7.png)

-----





### cc_color() : CoolConsole with Custom Font Color

If you're typing too fast and you have no-time for styling , this is just made for you

**cc_color(TEXT , COLOR);**

    TEXT {string} : the text you want to write
    
    COLOR {string} : the color of text

Note: color must be a valid color like (**"red"** , **"green"** , **"blue"** ...) Or you can use RGB colors **"#ffffff"**

* Example :

```javascript
    cc_color("This is a Red Text !", "red");
    // Console.log with red font color
    cc_color("This is a #ff00ff Text !", "#ff00ff");
    // Console.log with #ff00ff font-color
```
![](https://i.imgur.com/Pc5VokM.png)


------------


### cc_bold() - cc_italic() - cc_midline() - cc_underline() cc_xsmall() - cc_small() - cc_medium() - cc_large() - cc_xlarge()

   If you're typing too fast and you have no-time for styling , this is just made for you

**cc_bold(TEXT);**

**cc_italic(TEXT);**

**cc_midline(TEXT);**

**cc_underline(TEXT);**

**cc_small(TEXT);**

**cc_medium(TEXT);**

**cc_large(TEXT);**

**cc_xlarge(TEXT);**

    TEXT {string} : the text you want to write

* Example :

```javascript
    cc_bold("This is BOLD");
    cc_italic("This is Italic");
    cc_midline("This is MidLine");
    cc_underline("This is Underline");
    cc_xsmall("This is XSmall");
    cc_small("This is Small");
    cc_medium("This is Medium");
    cc_large("This is Large");
    cc_xlarge("This is XLarge");
    
``` 

![](https://i.imgur.com/YTx7O3W.png)

-----


### cc_rainbow() 

#### Rainbow Text 🌈

This function lets you write console.log message with rainbow colors 🌈 ( *Just for fun !* )

**cc_rainbow(TEXT)**

    TEXT {string} : the text you want to write

* Example :

```javascript
    cc_rainbow("RAINBOWWWWWWWWW");
``` 

![](https://i.imgur.com/lXircRZ.png)

-----


### cc_zebre() -

#### Black & White Text 🦓

This function lets you write console.log message with Black & White colors 🦓 ( *Just for fun !* )

**cc_zebre(TEXT)**

    TEXT {string} : the text you want to write

* Example :

```javascript
    cc_zebre("This Text is Black & White!");
```

![](https://i.imgur.com/ACeBcJv.png)

-----

### c_all() 
#### Apply Style to All Text (Does not support Multi Text)

This function is like cc() but style applies to all string!
    
    Q: Why does this exists ?
    A: Sometimes i want to apply multiple styles to one single string without making extra effort
    Q: Then, you can do it with cc() with one single text and multi styles... Right ?
    A: Yes , you can do both...

**cc_all( TEXT , [STYLES ...] ) ;**
    
    TEXT {style}    : Text you want to write

    [ STYLES ]  {*} : (Optional) you can check list of STYLES [here](#list-of-styles)

* Example :

    ```javascript
        cc_all("Hello World", bold, large, red, underline);
        // this line will generate console.log message with bold, large, red , underline style
    ```

![](https://i.imgur.com/puumnUB.png)

-----

### cc_line() 
#### Line Break

This function draws a line in Console.log

**cc_line( [COLOR ])**
    
    [ COLOR ] {string} : (Optional) Color of Line

Example :
    
```javascript
    cc_line();
    /* Draws a Line in Console (Color: "black" by default) */
    cc_line("red");
    /* Draws a "red" Line in Console  */        
```

![](https://i.imgur.com/bqO6dtk.png)

-----


### cc_logo() 
#### Console Log with Custom Icons 😎 (My Favourite One)

You want Icons in your Console Log ? 😎

You can make console.log messages with Custom Icons ---> Icons List [Here](#list-of-icons)

**cc_icon( ICON , TEXT , [ TITLE ]);**

        ICON {*} : Name of Icon you want to add (See Icons List)

        TEXT {string} : Text you want to write
        
        [Title] {string} : (Optional) Title of your Message

* Example :

```javascript
    cc_icon(icon_diamond, "Wowww");
    /* Console.log with Diamond Icon and with no Title */
    cc_icon(icon_facebook, "https://facebook.com/Ademkouki.Officiel", "Facebook");
    /* Console.log with Facebook Icon and "Facebook" title */
    cc_icon(icon_heart, "Don't forget to like & Share CoolConsole")
    /* Console.log with Heart Icon */
    
```
![](https://i.imgur.com/08m58lj.png)

-----

> ### Advanced Usage

### cc_custom() :
#### CoolConsole with Custom CSS style

if you want to make your own style, 2 steps :
    
1. in your CSS, create a new class. For example, ".custom-console" and add your custom style

Example :

```html
        <style>
        .custom-console {

                font-size: 20px;
                font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
                text-shadow: 1px 2px red ;
                font-weight: normal;
                /* Any Style You Want ...*/
        }
        </style>
```

2. After that, in your Javascript do:

```javascript
            cc_custom("Your Text Here" , "custom-console");
            // cc_custom( TEXT ,  Class Name in CSS ( without Dot '.' )  );
```
3. That's All!

![](https://i.imgur.com/anNrXmc.png)

🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧
    
========[ Warning! ]=========
    
🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧

Don't add  ---> **.** (Dot)  in the classname

if your class (in CSS) ---> ".myclass" 
    
type -----> cc_custom("Your Text", **"myclass"** );

**You get it ? Right ??** 😅

-----

## List Of Styles

* Font Styles :

|  Font Style  |   Description      |      Example          |
| ------------ | -----------------  | --------------------- |
| normal       | Normal Style       | cc("text", normal)    |
| bold         | Bold Style         | cc("text, bold)       |
| italic       | italic Style       | cc("text", italic)    |
| underline    | Underline Style    | cc("text", underline) |
| midline      | Midline Style      | cc("text", midline)   |
| xsmall       | Extra Small Style  | cc("text", xsmall)    |
| small        | Small Style        | cc("text", small)     |
| medium       | Medium Style       | cc("text", medium)    |
| large        | Large Style        | cc("text", large)     |
| xlarge       | Extra Large Style  | cc("text", xlarge)    | 

-----

* Colors :

|  Color       |   Description      |      Example          |
| ------------ | ------------------ | --------------------- |
| red          | Red Font Color     | cc("text", red)       |
| orange       | Orange Font Color  | cc("text", orange)    |
| yellow       | Yellow Font Color  | cc("text", yellow)    |
| green        | Green Font Color   | cc("text", green)     |
| blue         | Blue Font Color    | cc("text", blue)      |
| indigo       | Indigo Font Color  | cc("text", indigo)    |
| violet       | Violet Font Color  | cc("text", violet)    |
| brown        | Brown Font Color   | cc("text", brown)     |
| black        | Black Font Color   | cc("text", black)     |
| grey         | Grey Font Color    | cc("text", grey)      |
| white        | White Font Color   | cc("text", white)     |
| cyan         | Cyan Font Color    | cc("text", cyan)      |
| pink         | Pink Font Color    | cc("text", pink)      |
| navy         | Navy Font Color    | cc("text", navy)      |
| magenta      | Magenta Font Color | cc("text", magenta)   |
| gold         | Gold Font Color    | cc("text", gold)      |

-----

* Custom Colors :

| Custom Color |   Description      |      Example          |
| ------------ | ------------------ | --------------------- |
| "#ffffff"    | #ffffff Font Color | cc("text", "#ffffff") |

Example :

```javascript
cc("Text Here" , "#3b00ff" );
```

-----

* Background Colors :

| Background Color |   Description            |          Example         |
| ---------------  | ------------------------ | ------------------------ |
| bg_red           | Red Background Color     | cc("text", bg_red)       |
| bg_orange        | Orange Background Color  | cc("text", bg_orange)    |
| bg_yellow        | Yellow Background Color  | cc("text", bg_yellow)    |
| bg_green         | Green Background Color   | cc("text", bg_green)     |
| bg_blue          | Blue Background Color    | cc("text", bg_blue)      |
| bg_indigo        | Indigo Background Color  | cc("text", bg_indigo)    |
| bg_violet        | Violet Background Color  | cc("text", bg_violet)    |
| bg_brown         | Brown Background Color   | cc("text", bg_brown)     |
| bg_black         | Black Background Color   | cc("text", bg_black)     |
| bg_grey          | Grey Background Color    | cc("text", bg_grey)      |
| bg_white         | White Background Color   | cc("text", bg_white)     |
| bg_cyan          | Cyan Background Color    | cc("text", bg_cyan)      |
| bg_pink          | Pink Background Color    | cc("text", bg_pink)      |
| bg_navy          | Navy Background Color    | cc("text", bg_navy)      |
| bg_magenta       | Magenta Background Color | cc("text", bg_magenta)   |
| bg_gold          | Gold Background Color    | cc("text", bg_gold)      |

-----

## List Of Icons

> (40) and More ... (Coming Soon)

![](https://i.imgur.com/VpWflnd.png)

|  Color               |   Description            |            Example                           |
| -------------------- | ------------------------ | -------------------------------------------- |
|  icon_flower 		   | flower Icon    		  | cc_icon( icon_flower  , "Text Here")         |
|  icon_ok 			   | OK Icon			      | cc_icon( icon_ok 	  , "Text Here")         |
|  icon_heart 		   | Heart Icon 		      | cc_icon( icon_heart   , "Text Here")         |
|  icon_user_f 		   | Female User Icon         | cc_icon( icon_user_f  , "Text Here")         |
|  icon_user_m 		   | icon_user_m 		      | cc_icon( icon_user_m  , "Text Here")         |
|  icon_message 	   | icon_message 	          | cc_icon( icon_message , "Text Here")         |
|  icon_facebook 	   | icon_facebook 	          | cc_icon( icon_facebook , "Text Here")        |
|  icon_youtube 	   | icon_youtube 	          | cc_icon( icon_youtube , "Text Here")         |
|  icon_github 		   | icon_github 		      | cc_icon( icon_github , "Text Here")          |
|  icon_add 		   | icon_add           	  | cc_icon( icon_add , "Text Here")             |
|  icon_remove 		   | icon_remove 		      | cc_icon( icon_remove , "Text Here")          |
|  icon_time 		   | icon_time 		          | cc_icon( icon_time , "Text Here")            |
|  icon_music 		   | icon_music 		      | cc_icon( icon_music , "Text Here")           |
|  icon_setting 	   | icon_setting 	          | cc_icon( icon_setting , "Text Here")         |
|  icon_cursor 		   | icon_cursor 		      | cc_icon( icon_cursor , "Text Here")          |
|  icon_star 		   | icon_star 		          | cc_icon( icon_star , "Text Here")            |
|  icon_greenflag 	   | icon_greenflag 	      | cc_icon( icon_greenflag , "Text Here")       |
|  icon_redflag 	   | icon_redflag 	          | cc_icon( icon_redflag , "Text Here")         |
|  icon_yellowflag 	   | icon_yellowflag          | cc_icon( icon_yellowflag , "Text Here")      |
|  icon_blueflag 	   | icon_blueflag 	          | cc_icon( icon_blueflag , "Text Here")        |
|  icon_key 		   | icon_key 		          | cc_icon( icon_key , "Text Here")             |
|  icon_love 		   | icon_love 		          | cc_icon( icon_love , "Text Here")            |
|  icon_map 		   | icon_map 		          | cc_icon( icon_map , "Text Here")             |
|  icon_thumb_up 	   | icon_thumb_up 	          | cc_icon( icon_thumb_up , "Text Here")        |
|  icon_thumb_down 	   | icon_thumb_down 	      | cc_icon( icon_thumb_down , "Text Here")      |
|  icon_zoomin 		   | icon_zoomin 		      | cc_icon( icon_zoomin , "Text Here")          |
|  icon_zoomout 	   | icon_zoomout 	          | cc_icon( icon_zoomout , "Text Here")         |
|  icon_wifi 		   | icon_wifi 		          | cc_icon( icon_wifi , "Text Here")            |
|  icon_world 		   | icon_world 		      | cc_icon( icon_world , "Text Here")           |
|  icon_send 		   | icon_send 		          | cc_icon( icon_send , "Text Here")            |
|  icon_hand 		   | icon_hand 		          | cc_icon( icon_hand , "Text Here")            |
|  icon_picture 	   | icon_picture 	          | cc_icon( icon_picture , "Text Here")         |
|  icon_phone 		   | icon_phone 		      | cc_icon( icon_phone , "Text Here")           |
|  icon_folder 		   | icon_folder 		      | cc_icon( icon_folder , "Text Here")          | 
|  icon_audio 		   | icon_audio 		      | cc_icon( icon_audio , "Text Here")           |
|  icon_diamond 	   | icon_diamond             | cc_icon( icon_diamond , "Text Here")         |
|  icon_money 		   | icon_money 		      | cc_icon( icon_money , "Text Here")           |
|  icon_idea 		   | icon_idea 		          | cc_icon( icon_idea , "Text Here")            |
|  icon_computer 	   | icon_computer 	          | cc_icon( icon_computer , "Text Here")        |



# Note

This library was made in 2 days ( + 1 day for documentation )

Sorry For my Bad English ... It's my third language , feel free to correct my mistakes...

If you want to ask me , just send me an email [ademkingnew@gmail.com][1].  😅 


# License

This project is licensed under the MIT open-source license.

# Contributing

If you have any feedback on this wrapper drop us an email to [ademkingnew@gmail.com][1].

The project is hosted on GitHub at [https://github.com/Ademking/CoolConsole][2].
If you would like to contribute a bug fix or improvement please fork the project 
and submit a pull request.

[1]: mailto:ademkingnew@gmail.com
[2]: https://github.com/Ademking/CoolConsole



