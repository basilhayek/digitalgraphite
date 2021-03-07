I've wanted to keep a journal--at least somewhat consistently--for a long time. 

There's a few things I want to log on a semi-regular basis: my coding, personal goals, reflections, quick notes about being the father to a 5.5 year old, etc.

I've tried different apps, sometimes a couple at a time, but none seemed so stick. Switching between apps seemed sub-optimal. Plus I didn't like being locked in to that platform.

So of course I thought: why not do it in Notion?
<!--excerpt-->

I set up a Gallery with very basic customization. Set the Card preview to be the page cover and added a formula to concatenate the Created date and the Name as the title. No tags for now, I'll add them later.

I chose the **Gallery** because I wanted it to be somewhat visual. But I realized that the Notion covers left a little to be desire. A set palette of solid colors and gradients. Some stock images. You could add other images but had to upload them from your machine or find them first.

So I decided to try something. I whipped up a simple web service using Flask that returns a 1500x300 cover. I started with solid backgrounds and then added a two-color gradient. 
![](https://cdn.digitalgraphite.dev/06_notion_covers/01_notion_covers_solid.png)
![](https://cdn.digitalgraphite.dev/06_notion_covers/02_notion_covers_gradient.png)

For a while this worked, but then I decided it would be nice to have some sort of illustration. After some quick Googling, I added emoji support.

![](https://cdn.digitalgraphite.dev/06_notion_covers/03_notion_covers_emoji.png)

I realize there's still a lot more that I could add, but it works for now.

To use this, choose to provide a Link as your Notion cover, and then enter a URL in one of the following formats:
* https\://www\.coversfornotion\.com/solid/\<color\>
* https\://www\.coversfornotion\.com/gradient/\<color1\>/\<color2\>
* https\://www\.coversfornotion\.com/emoji/\<emoji\>/\<color\>
* https\://www\.coversfornotion\.com/emoji/\<emoji\>/\<color1\>/\<color2\>


For the above:
* emoji: is an emoji name ([WebFx emoji cheat sheet](https://www.webfx.com/tools/emoji-cheat-sheet/))
* color: any hex code or standard color name ([W3C color names](https://drafts.csswg.org/css-color-4/#named-colors))

A bit more detailed instructions and examples are [here](https://www.notion.so/basilhayek/Covers-for-Notion-32e8918fbc3f46f6a8006f21a747cb96).

That's it. The code is here on [repl.it](https://repl.it/@basilhayek/notioncover) if you want to fork and play with it, and also on [Github](https://github.com/basilhayek/notioncover).
