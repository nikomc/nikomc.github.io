---
layout: post
title:  "Automated Biology Is Now an Affordable Reality"
tags: [ science, synthetic biology, tech ]
featured_image_thumbnail:
featured_image: assets/images/posts/2020/chibio_setup.jpg
featured: true
hidden: true

---

When the sun dips below the Pacific ocean, the white domes of Mount Wilson Observatory can still be seen to the east. Perched on the San Gabriel crest, the Observatory receives the final kisses of sunlight at the end of every day.

There is not a window near my bench, but I can sense the shift from day to night by the lulls in conversation, the departing bodies, and the long shadows that drape across the laboratory.
With pipette in hand, the wall clock reads “8”. Still, I set up my experiment, moving tip to liquid, liquid to cells, tip to trash. Repeat _ad infinitum_.

Experiments are a drudgery, and I easily lose track of time. My mind inevitably wanders, I make a mistake and am forced to discard the experiment. So I begin again, _ad infinitum_.
At times like this — after the sun has fallen, but I remain rooted to my chair — I think about my travails, and consider whether they could be solved with a benevolent robot.

***

“I do my experiments from home, actually,” said [Dr. Harrison Steel](http://sysos.eng.ox.ac.uk/wiki/index.php/User:Harry), one of the creators of a new device called Chi.Bio, through my computer screen.

Steel’s room in Oxford is spotless, so much so that Room Rater might be inclined to give it a ten out of ten. His answers are neat and polished, without a single ‘umm’ or ‘ahh’ injected.

When Steel was a PhD student, many of his experiments felt banal. He, too, has felt the pain of solitude in the laboratory — the lone scientist, hunched over an experiment, after all others have departed.

“For days, I would have to measure and dilute cells, which is very tedious if you’re doing it by hand,” said Steel. “Now, after I set everything up, I can sit at home and watch each of my graphs and add chemicals or turn on lights and take measurements.”

In other words, Steel has figured out a way to avoid the evening drudgery that plagues so many biologists.

While most PhD students, at some point, go through a period of experimental tedium and dejection, few emerge from that experience with an automated solution. But now Steel has solved it, four years after hatching an idea. The new device was [published in _PLoS Biology_](https://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.3000794), an open-access journal, last week.

[Chi.Bio](https://chi.bio/) began as a cure for monotony — a simple device to grow cells — but soon expanded in functionality. Whenever Steel had to perform a new type of experiment, he figured out a way to automate it with some DIY know-how. The result is an intricate piece of equipment made from about 300 dollars worth of printed circuit boards (PCBs) and off-the-shelf parts, that can grow cells, dilute them, probe them, control them, and measure them — all remotely.

***

{% include image-caption.html imageurl="/assets/images/posts/2020/chibio_turbidostat.png#wide" title="A schematic of the Chi.Bio device, which integrates a microcontroller, peristaltic pumps, and a bioreactor that incorporates lasers, LED, and other components for measuring cells and proteins." %}

Chi.Bio only has three components: a control computer, peristaltic pumps for liquid handling, and bioreactors. But those components are loaded with functionality.

“The device has a really cheap chip spectrometer, which was only released a couple of years ago,” said Steel. “Also, a whole array of different LEDs in a single LED chip is built into the device, so you can output and carefully control the complete visual spectrum of light, which is very important for measuring fluorescent proteins, or for growing certain photosynthetic cells. Over time, I added heat plates, stirring, temperature sensors, and all this pumping hardware.”

The device that emerged after years of tinkering, with lots of “soldered parts”, was uniquely enabled by Steel’s background. “I had some hardware experience,” he said, “because before I came to Oxford, I worked in quantum computing research and did some electrical engineering.”

Towards the end of our discussion, I asked Steel why, in his opinion, the Chi.Bio is useful to scientists when so many similar devices already exist. I was thinking mainly about the [eVOLVER system](https://www.nature.com/articles/nbt.4151), published a couple of years ago in _Nature Biotechnology_, but there are also “biohackers” that build DIY hardware, in kitchens and garages, for similar purposes.

Steel’s response was assured.

“eVOLVER is designed to be a very parallelized platform, and so you get the ability to grow many things at once and mix between them. This makes it ideal for things like high-dimensional evolutionary studies, and the platform has certainly been groundbreaking in that area,” said Steel.

“However, you don’t have the same level of control as our device; you can’t measure all these fluorescent proteins and you can’t do optogenetics, and you’re limited to the number of pumps and inputs that are going to each reactor. We tried to make a very adaptable system, which can be used in many different applications. We tried to make it very cheap. And we tried to make it scalable as well.” And it’s still open-access.

Steel thinks that his platform is perfect for biotech startups, especially — researchers that cannot afford 100,000 dollars worth of equipment but want to automate their experiments. It could also prove a boon to the DIY-Bio enthusiasts that are flocking to maker spaces and community labs, searching for ways to [democratize insulin](https://openinsulin.org/), create [“real vegan cheese”](https://realvegancheese.org/), or produce [glow-in-the-dark plants](https://www.technologyreview.com/2016/07/15/158184/why-kickstarters-glowing-plant-left-backers-in-the-dark/#:~:text=In%20any%20discussion%20of%20biohacking,code%2C%20living%20things%20mere%20hardware.).

For a few hundred dollars, you could build a Chi.Bio yourself with the online [instruction manual](https://chi.bio/hardware/). Or you can skip the soldering and buy one from [LabMaker](https://www.labmaker.org/collections/biotechnology/products/chi-bio) for just under a thousand dollars.

Until I find the time and money to automate my own experiments, I will be here, in the laboratory, with the long shadows of Mount Wilson. There are always more experiments to run. So I pick up my pipette, move tip to liquid, liquid to cells, tip to trash. Repeat _ad infinitum_.

{% include robot_svg_animation.html %}

***
The other authors on the PLoS Biology paper are Robert Habgood, Ciarán Kelly and Antonis Papachristodoulou.

**Reference:** Steel H, Habgood R, Kelly C and Papachristodoulou A. “In situ characterisation and manipulation of biological systems with Chi.Bio” _PLoS Biology_ (2020). DOI: https://doi.org/10.1371/journal.pbio.3000794

***

**Image:**

Animation made by Niko McCarty with SVG and CSS.

All other images courtesy of the [Chi.Bio](https://chi.bio/) team.
