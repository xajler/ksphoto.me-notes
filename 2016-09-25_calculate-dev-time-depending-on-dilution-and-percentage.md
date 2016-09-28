# Calculate dev time depending on dilution and percentage

Sometimes is all you need to do is read, but I'm not good with that, I just go straight to the matter. So, I've bought from Fotoimpex, Adox CMS 20 II bundle: developer Adotech III + 4 120 rolls of film. I even mailed to Adox to get some clarification on few things like agitation and Hypo Clear, and got reply from them, which is really great.

But this was not issue. Issue was, there is Adotech III developer of 100ml for developing those 4 films in the bundle, Very simple math should state 100/4 = 25ml. But this is not correct for proper dilution of 1+9, it is actually 50ml for 500ml of working solution.

Not sure what was going through my had, but actually I developed 3 rolls using 25ml of developer for 500ml of solution, which is 1+19 dilution. Even in their data sheet states that for 500ml of solution, there is need for 50ml of Adotech III. And also in data sheet it states that working solution can last for 4 weeks, so you don't need to do two rolls at once. But for some reason I did simple math and use 25ml for each 3 rolls, and I should have do 2 rolls in one same 500ml solution.

So my first 3 films were done on half strength, make it really flat, especially those that I rated at ISO 12, those of ISO 20, were tolerable, some of them like photo I called "Dies Irae III" and "Tunnel Vision" looks quite interesting with lack of contrast. But they were not developed "properly" but rather on half of its proper strength.

> Photos: Dies Irae III, Tunnel Vision

So I left with last 4th roll, and luckily I was more paying attention on this one, so I was stuck with cca. 30ml of Adotech III (needed was 50ml). And also found somewhere that this film should be rated at ISO 6, by decreasing development for 20%. Looks interesting to shoot at ISO 6, I never did in my life, so why not?

Honestly, I was stuck at that moment, since this is my first half year with film, and you can guess that I'm no expert. Nevertheless, since I'm software developer, I laid all my variables:

* 1+9 (50ml + 450ml) vs. 1+16 (29.4ml + 470.6ml) - ? increase
* ISO 20 vs ISO 6 (20% decrease, actual percent number found somewhere on the web, used as is)

OK, nothing that complicated, first I need to increase development than I need to decrease, easy stuff :)

But surely, this was a way above my comfort zone with usual development of film: look into data sheet, got time, temperature, and off you go.

But I really wanted to get something from that last roll of film. And here is how I did it....

## Dilution calculation

For normal (1+9) dilution developing time for 20 ISO @ 20°C is 8 min. Again with simple linear math, we can state that for (1+18) dilution will need double time: 16 min, and somewhere in between those two (1+13.5) we have half a time, 12 min, and going to the 4th of it, we got cca. (1+16) and 14min development.

This is might or might not be right, this is how I got about it, with pure linear fashion. But most things in film are not linear like reciprocity failure. Whole assumption for this calculation of dilution is that development is linear, meaning that if you have something at 8min and you want/have half of developer solution of normal development, you'll need to double the time (16min).

Linear dilution calculation for 120 film at ISO 20:

* 1 + 9 @ 8min (full strength)
* 1 + 13.5 @ 12min (between full and half strength)
* 1 + 16 @ 14min (4th between full and half strength, actually it is 1+15.75)
* 1 + 18 @ 16min (half strength with double time, should be full strength)

### UPDATE

Some explanation on how I got those numbers there:

* 1 + 9 @ 8min Starting point, look into Adox CMS 20 II data sheet for 120 roll and ISO 20.
* 1 + 13.5 is (18 - 9 = 9 / 2 (half) = 4.5 + 9 (initial) = 13.5. It is really middle between 1+9 and 1+18. Because 9 + 4.5 = 13.5.
* 12min is (16 - 8 = 8  / 2 (half) = 4 + 8 (initial) = 12min. Middle between 8 and 16, this should be obvious.
* 1 + 16 actually (1+15.75) it is 4.5 / 2 = 2.25. So 1 + 15.75 is between 1 + 13.5 and 1 +18, because 13.5 + 2.25 = 15.75, I've round it as 1 + 16, it is easier :)
* 14min is essentially between 12 and 16, and should be obvious that is 14.
* 1 + 18 @ 16min (half development solution with correct time: 9 + 9 = 18, and 8 + 8 = 16)

And that is essentially all to it, as smart would said 'divide and conquer'...

## Percentage calculation

OK, so we have linear dilution time for (1+16): 14min. How about doing percentage of 20% less development from ISO 20 to ISO 6. Here is how I did it, with help of some googling, didn't try so hard to understand it, but from calculation result easy to calculate like 50%, it seems correct.

Whole calculation in steps:

* 14 (min) * 60 = 840 (minutes converted to seconds)
* 840 * 0.20 = 168 (16min in seconds times 20%)
* 168 * 0.5 = 84 (Not sure what 0.5 means, only thing that interested me, is to work)
* 20% of 14min = 1min 24sec. 60 (1min) + 24sec = 84 sec.
* Putting it all together

So to put it all together so far we have:

* For dilution (1 + 16): 14 min development time
* 20% of 14min = 1min 24sec: decrease dilution time for 1min 24sec
* 14min - 1:24min = 12:36min

## Final Result

> Photos: Negatives and Contact sheet

Finally from all of this calculation, for some reason, I've used 14min, added more development to it. It is really personal preference, but this post it is really how to calculate to get "accurate" starting point development time, like those in data sheets and then apply more or less development depending on situation and preference.

> Photo: Iz tvoje sam kolijevke Rijeko...

## Caution

Please use this calculation notes with caution, I'm no expert with developing film, I did around 50 rolls of film in my life. This is just a guide how to do it (or how I did it), when you're really out of ordinary development and you're stuck with some variables like different dilution or percentage of development time.

Hope this helps somebody, I'm glad I've gone through it, and at least have workable negatives, and one more experience to use when needed and share with others on this blog.

If anyone have an comment on this and have better way for doing this, please do write in comment!