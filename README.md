## VIM Clutch by Aleksandr Levchuk ##

*COMING SOON TO KICKSTARTER.COM!

VIM Clutch is a hardware pedal for improved text editing speed for users of the magnificent VIM text editor (<a href="http://www.vim.org/about.php">1</a>, <a href="http://www.viemu.com/a-why-vi-vim.html">2</a>). When the pedal is pressed down, the pedal types "i" causing VIM to go into Insert Mode. When released, it types &lt;Esc&gt; and you are back in Normal Mode.

I just made one and it works great. Here is how I did it.

1. Purchased 2 USB foot switches (pedals) from China:
I used Ankaka.com and payed 20 USD (includes 2 pedals and shipping to California). <br />
Later I found out the OEM: PC sensor http://www.pcsensor.com/index.php?_a=viewProd&productId=2 $5.50 per pedal

2. The peddal is programmable via a Windows GUI. Once programmed you can plug it into any Mac or Linux and it will work.

3. Unfortunately, only the Pedal Down event is programmable. But we need to be able to press &lt;Esc&gt; as the pedal is release. I emailed PC sensor, reaching out to collaborate but I just got the pedals from the post office today and really wanted it to work. So I stated hacking at it and came up with a solution in a about 1 hour.

  1. I programmed one pedal to send the letter "i" and the other to send the &lt;Esc&gt;

  2. Took both pedals apart


     <img src="https://github.com/alevchuk/vim-clutch/raw/master/pic1.jpg" />
     <br />
     <br />
     <br />
     <br />


  3. With electrical tape, attached 2 toothpicks to the plastic blade that goes between the Infrared sensors when the pedal is in the down possition.


     <img src="https://github.com/alevchuk/vim-clutch/raw/master/pic2.jpg" />
     <br />
     <br />
     <br />
     <br />


  4. Placed both sensors boards into one pedal enclosure so that, as the pedal is pressed, first the toothpicks will cross the &lt;Esc&gt; sensor, and after that the plastic blade will enter the "i" sensor. As the pedal is release the toothpicks will cross the &lt;Esc&gt; sensor again.


     <img src="https://github.com/alevchuk/vim-clutch/raw/master/pic3.jpg" />
     <br />


## Acknowledgments ##

I would like to say Thank You to:

   * Sean Mahoney for suggesting the name Vim Clutch. 

   * Anton Polishko for suggesting pressing &lt;Esc&gt; every time right before pressing "i" in order to avoid typing undesired "i"s.

   * Tyler Backman for letting my use a Windows computer.

   * The company PC Sensor for building such a clean and incredibly inexpensive device.


## Finally the first VIM Clutch ##

  <img src="https://github.com/alevchuk/vim-clutch/raw/master/pic4.jpg" />


## Has anyone thought of this before? ##

Perhaps, but I was not able to find any mention of using a pedal for Vi or VIM. I searched for this occasionally for a span of more than 2 years. Nothing like this comes up on Google. I shared my idea with a lot of my friends and no one mentioned that this was already thought of by someone else.

As a result I consider myself the inventor of the VIM Clutch.


## Extras ##

PC Sensor also has a triple version of the pedal. I will order two of those as well. I will program:

   * The left pedal to "I" - insert at the beginning of the line
   * The middle pedal to "i" - regular insert mode
   * The right pedal to "A" - insert at the end of the line


## License ##

<a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/"
><img alt="Creative Commons License"
style="border-width:0" src="http://i.creativecommons.org/l/by-sa/3.0/88x31.png"i
 /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" 
href="http://purl.org/dc/dcmitype/Text" property="dct:title" 
rel="dct:type">The VIM Clutch work</span> by <a 
xmlns:cc="http://creativecommons.org/ns#" 
href="https://github.com/alevchuk/vim-clutch" property="cc:attributionName" 
rel="cc:attributionURL">Aleksandr Levchuk</a> is licensed under a <a 
rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/">Creative 
Commons Attribution-ShareAlike 3.0 Unported License</a>.
