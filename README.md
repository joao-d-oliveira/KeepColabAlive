# TypingBird - KeepColabAlive
**Descrition**: AppleScript to keep colab alive during training

![Typing Bird](https://github.com/joao-d-oliveira/TypingBird-KeepColabAlive/raw/main/img/typingbird.gif "Typing Bird")

Pretty much what the description says, it's a very simple script so that you can leave your colab working for 
the 12hrs you're "entitled" without needing to go physically and punch some keys.

I struggled with some heavy models for work which take +9hrs to complete a single epoch, ... 
so I created this very simple work around which at every *x minutes* types in a key.

# How to Use

First of all, this is for Mac OS users... so if you're in linux 
or Windows, I'm sure you can find other options.

The script has the following algorithm:
* Make Chrome's 1st window active
* Click on the tab containing Google's Colab 
* Click on an empty code text-box from google colab (will be reused... so better have it empty than with your code)
* Press a random key
* Wait between 8-10 minutes and then re-run

In order to make it work for your scenario / Environment, you will most certainly need to adjust the places
where to click... unless by some chance the places where you have you tab or Colab empty text_box match mine. 

In case you need to figure it out the X, Y where to click, you can use a simple trick, which is to click on 
"[Apple] + [shift] + 4" (this is my shorcut key to take a screenshot, in case you have different, use different).

When taking a screenshot, the cursor will tell you the X, Y coordinates, as the picture exemplifies it below. 

![example screenshot](https://github.com/joao-d-oliveira/TypingBird-KeepColabAlive/raw/main/img/Example_screenshot.jpeg "Example Screenshot")

Simply take the script and edit the following parts:
* `click at {213, 50}` in order to edit where to click corresponding to the tab
* `click at {954, 557}` in order to edit where to click corresponding to the text box in Google Colab.

**attention:** choose the coordinates inside the textbox where you can type. The whole black box from the 
code, doesn't enable you to type. check that the typing cursor is active.

![example text box](https://github.com/joao-d-oliveira/TypingBird-KeepColabAlive/raw/main/img/ExampleTextBoxColab.jpeg "Example TextBox Google colab")

## Possible problems

This is working for me as of March-2022... Google is known to 
change this to make it harder for these workarounds... so who knows until 
when this is working.
Another thing is that after a while, Google might have a random "are you a human box"
Which will make this script unworkable ... 

## Help from whoever wants to help...

If you want to complete the script with an identification 
of the "Are you a human", in order to make the script more complete...
that will be highly appreciated.

That's it! Good Luck!