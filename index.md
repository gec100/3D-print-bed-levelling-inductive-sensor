Had this sensor for long time working great on my custom made prusa clone and now I'm building a new corexy printer around SKR 1.4 Turbo board on 24V.

I'm not a electronics engineer but I can find my way around.

The sensor needs 6-36V to work properly, but probe connectors on the board can accept only 3-5V. On 12V boards this sensor needed to be connected to the 12V pin (spare Fan connector) with voltage divider described here http://reprap.com/wiki/Z_probe

In this 24V setup, resistors had to be changed. With https://www.allaboutcircuits.com/tools/voltage-divider-calculator/
I calculated that my resistors need to be roughly 4:1 (R1:R2) in size to get the output voltage below 5V needed for the Z-stop probe pins. That would be cca 4kΩ for R1 and 1kΩ for R2 or 8kΩ for R1 and 2kΩ for R2 . You get the point. I had at my hands 5k1 for R1 and 1k for R2 giving me cca 3.9V that is well inside 3-5V range.

here is my very rough schematics:

![Image](https://user-images.githubusercontent.com/8178773/89330570-be9fcd80-d690-11ea-98d7-8f2fd71f060a.png)


[//]: # ## Welcome to GitHub Pages
[//]: # 
[//]: # You can use the [editor on GitHub](https://github.com/gec100/3D-print-bed-levelling-inductive-sensor/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.
[//]: # 
[//]: # Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.
[//]: # 
[//]: # ### Markdown

<!--Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for -->

<!--```markdown -->
<!--Syntax highlighted code block -->

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/gec100/3D-print-bed-levelling-inductive-sensor/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
-->
