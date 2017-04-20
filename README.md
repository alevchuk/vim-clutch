## VIM Clutch by Aleksandr Levchuk ##

VIM Clutch is a hardware pedal for improved text editing speed for users of the [magnificent](http://www.viemu.com/a-why-vi-vim.html) VIM [text editor](http://www.vim.org/about.php). When the pedal is pressed down, the pedal types <kbd>Esc</kbd>+<kbd>i</kbd> causing VIM to exit your current mode and go into Insert Mode. When released, it types <kbd>Esc</kbd> and you are back in Normal Mode.

I just made one and it works great. Here is how I did it.

1. Purchased 2 USB foot switches (pedals) from China:

    I used Ankaka.com and payed 20 USD (includes 2 pedals and shipping to California).
    Later I found out the OEM: PCsensor for [$5.50 per pedal](http://www.pcsensor.com/index.php?_a=viewProd&productId=2)
    They also sell a [cheaper version](http://www.suntekstore.com/goods-10010504-pc_usb_foot_switch_keyboard_pedal.html) from Hong Kong.

2. The pedal is programmable via a Windows GUI or on Mac/Linux through the [footswitch CLI](https://github.com/rgerganov/footswitch). Once programmed you can plug it into any Mac or Linux computer and it will work.

3. Unfortunately, only the Pedal Down event is programmable. But we need to be able to press <kbd>Esc</kbd> when the pedal is released. I emailed PC sensor, reaching out to collaborate but I just got the pedals from the post office today and really wanted it to work. So I stated hacking at it and came up with a solution in a about 1 hour:

    1. I programmed one pedal to send the letter <kbd>i</kbd> and the other to send the <kbd>Esc</kbd>.

    2. I took both pedals apart.

        ![Disassembled pedal](https://github.com/alevchuk/vim-clutch/raw/master/pic1.jpg "Pedal disassembly")

    3. With electrical tape, I attached 2 toothpicks to the plastic blade that goes between the infrared sensors when the pedal is in the down position.

        ![The sensor blocker](https://github.com/alevchuk/vim-clutch/raw/master/pic2.jpg "Taping the sensor blocker")

    4. I placed both sensors boards into one pedal enclosure so that, as the pedal is pressed, first the toothpick will cross the <kbd>Esc</kbd> sensor, and after that the plastic blade will enter the <kbd>i</kbd> sensor. As the pedal is release the toothpicks will cross the <kbd>Esc</kbd> sensor again.

        ![Sensor configuration](https://github.com/alevchuk/vim-clutch/raw/master/pic2.jpg "Arranging the sensors")

## Acknowledgments ##

I would like to say Thank You to:

   * Sean Mahoney for suggesting the name Vim Clutch. 

   * Anton Polishko for suggesting pressing <kbd>Esc</kbd> every time right before pressing <kbd>i</kbd> in order to avoid typing undesired <kbd>i</kbd>s.

   * Tyler Backman for letting me use a Windows computer.

   * The company PC Sensor for building such a clean and incredibly inexpensive device.

## Finally the first VIM Clutch ##

  ![Arranging the sensors](https://github.com/alevchuk/vim-clutch/raw/master/pic4.jpg "The final product")

## Has anyone thought of this before? ##

Perhaps, but I was not able to find any mention of using a pedal for Vi or VIM. I searched for this occasionally for a span of more than 2 years. Nothing like this comes up on Google. I shared my idea with a lot of my friends and no one mentioned that this was already thought of by someone else.

As a result I consider myself the inventor of the VIM Clutch.

## Extras ##

PC Sensor also has a triple version of the pedal. I will order two of those as well. I will program:

   * The left pedal to <kbd>I</kbd> - insert at the beginning of the line
   * The middle pedal to <kbd>i</kbd> - regular insert mode
   * The right pedal to <kbd>A</kbd> - insert at the end of the line


## License ##

![Creative Commons License](http://i.creativecommons.org/l/by-sa/3.0/88x31.png "Creative Commons License")

<span xmlns:dct="http://purl.org/dc/terms/" 
href="http://purl.org/dc/dcmitype/Text" property="dct:title" 
rel="dct:type">The VIM Clutch work</span> by <a 
xmlns:cc="http://creativecommons.org/ns#" 
href="https://github.com/alevchuk/vim-clutch" property="cc:attributionName" 
rel="cc:attributionURL">Aleksandr Levchuk</a> is licensed under a <a 
rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/">Creative 
Commons Attribution-ShareAlike 3.0 Unported License</a>.
