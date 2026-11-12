# A little visual tablet weaving pattern reader

Hi all!

I've always used text notation to read my patterns while weaving, something along these lines:

```text
Pick | Up                  | Down
-----+---------------------+------
58   | 2 6-19 23           | 1 3-5 20-22 24
57   | 2 6-18 23           | 1 3-5 19-22 24
56   | 1-5 9-16 20-24      | 6-8 17-19
```

And I've also always struggled with reading these notations while weaving.

I'm constantly looking back and forth between my weaving and the sheet/screen, trying to keep track of:

- **Which pick I'm on.**
- **Which cards I've already turned**, and which still need turning.
- **Which column I'm supposed to be reading**, jumping back and forth between Up and Down.
- **Whether I've actually turned everything correctly**, because after all that counting and jumping around, I'm no longer entirely confident I haven't missed something.

I suspect I might have some mild form of dyscalculia, which probably doesn't help matters.

I've considered using the more commonly seen visual schematics, but those still involve quite a bit of scanning across rows and keeping track of where you are. So while they're certainly an improvement in some respects, they don't really eliminate the mental load I'm trying to get rid of.

So I figured I'd make something a little different!

The idea was to make reading a pattern as straightforward as possible, with as few mental 'jumps' as I could manage.

### The idea

Rather than having to interpret lists of card numbers, the tool converts each pick into a single, colour-coded strip representing all the cards in your pack, from left to right.

Adjacent cards turning in the same direction are grouped together, with the width of each group proportional to the number of cards it contains.

So instead of reading `1-5`, `6-8`, `9-16`, etc., you get a visual sequence telling you to turn **5 cards forward, 3 cards backward, 8 cards forward**, and so on.

Each group displays its number of cards and turning direction, with the actual card numbers underneath. And if a group is too narrow to comfortably display everything, you can simply tap it to see the exact cards involved.

The result is something you can hopefully read almost at a glance, working your way from left to right without having to do much counting or interpreting.


<img width="1334" height="822" alt="SCR-20261112-kddu" src="https://github.com/user-attachments/assets/9ccab7ba-e004-41b0-b66f-8d79752579be" />
<img width="1302" height="838" alt="SCR-20261112-kdij" src="https://github.com/user-attachments/assets/414a2b10-5e98-459b-a482-86f3fdc57725" />

### Some features

- **One pick at a time.** Only the current pick is displayed, with a rather large pick number to make it obvious where you are. No more accidentally reading the nearly identical pick above or below.
- **Proportional, colour-coded card groups.** Green for forward, orange for backward. Each group is sized according to how many cards it contains, so the visual layout also corresponds to the physical distribution of your cards.
- **Simple pick navigation.** Previous and Next buttons let you advance through the pattern, with the option to jump directly to a particular pick.
- **Focus mode.** Enlarges the current pick to fill the screen, getting rid of pretty much everything that isn't relevant while weaving. Particularly useful on a phone or tablet sitting beside your loom.
- **Unweaving mode.** Mistakes happen, and mentally reversing every instruction while undoing your work isn't exactly helpful. Enable this mode and all the turning directions are automatically reversed. Then simply work your way back through the picks using Previous.
- **Full pattern overview.** A collapsible overview displays all picks using the same visual notation. You can tap any row to jump directly to it, or print the entire thing if you prefer working from paper.
- **Dark mode.** Because sometimes you just don't want a bright white screen staring at you.
- **Automatic progress saving.** Your pattern, settings and current pick are saved locally in your browser, so you can close the page and pick up where you left off.

Nothing particularly revolutionary, but all aimed at reducing the amount of mental bookkeeping involved in following a pattern.

### How to use it

I've tried to keep this as straightforward as possible too.

**1. Get your pattern**

The tool accepts the `Pick | Up | Down` text notation exported from the excellent [Tablet Weaving Simulator](https://tabletweavingsim.com/).

Individual card numbers and ranges are supported, so there's no need to modify the notation beforehand.

**2. Paste and convert**

Open the **Pattern** menu at the top, paste your notation into the text field, enter your number of tablets, and hit **Convert pattern**.

That's it! The tool automatically groups adjacent cards by turning direction and generates the visual instructions.

There's already an example pattern loaded when you first open it, so you can have a look around without having to prepare anything.

**3. Start weaving!**

Use **Next** to advance through your picks as you weave, or **Previous** to go back.

Each pick shows the card groups in their physical left-to-right order. Just follow the instructions across the strip, insert your weft, and move on to the next pick.

If you're working from a phone, I'd recommend enabling **Focus mode**. This gives you a much larger view of the current pick, with navigation buttons at the bottom.

**4. If you make a mistake...**

Enable **Reverse turns · unweave**.

All the directions will flip, while keeping the original card groupings intact. Navigate backwards through the picks and undo the corresponding turns, without having to mentally translate each instruction into its opposite.

**5. Prefer paper?**

Open the pattern settings and hit **Print overview**. This generates a printer-friendly version of the complete visual pattern, which you can also save as a PDF.

You can even choose whether the overview lists the highest or lowest pick first.

**6. Want it on your phone?**

It works directly in your browser, but you can also add it to your home screen as an installable web app.

On iOS, open it in Safari and use **Share → Add to Home Screen**. After the app has cached its files, it can also be used offline.

No account, login, or pattern uploads required. Everything is handled locally in your browser.

---

### Give it a go!

**The tool:**

https://rxbxn.be/tablet-turn-reader/

---

And that's about it!

It's essentially a little attempt at making tablet weaving a bit more intuitive, especially for those of us who find constantly interpreting numerical instructions a bit exhausting.

I'm curious to hear whether anyone else struggles with reading patterns in the same way, or whether I've just invented an elaborate solution to a very particular *me* problem. :)

Any feedback or suggestions are very welcome!

**Full disclaimer:** This was made with AI. Do with that information what you will.
