---
layout: post
title:  "How Long Would It Take Bacteria to Eat the Earth?"
tags: [ science, estimates ]
featured_image_thumbnail:
featured_image: assets/images/posts/2020/cells_mozhvilo.jpg
featured: true
hidden: true

---

When I first heard that bacteria in the body outnumber human cells ten-to-one, [eight years ago](https://www.ted.com/talks/bonnie_bassler_how_bacteria_talk/transcript?language=en), I thought, “Now that is truly terrifying, to be mostly bacterial, a container for microbial soup.” The thought is morbid, but I can explain its appeal.

The notion that bacterial cells outnumber human ones is intriguing because I, like others, envision bacteria as microscopic, impotent creatures that only exert their influence when causing some terrible disease. The idea that people are “mostly bacterial” removes the impotent adjective from these creatures — bacteria are interesting because they are me. In the titular words of Ed Yong, [“I Contain Multitudes”](https://www.amazon.com/Contain-Multitudes-Microbes-Within-Grander/dp/0062368605/ref=sr_1_1?crid=1VYJETIMK83PH&dchild=1&keywords=i+contain+multitudes&qid=1596515930&sprefix=i+contain+%2Caps%2C185&sr=8-1).

Unfortunately, it turns out that the ten-to-one thing is not true. Bacteria and human cells [probably inhabit our bodies at a one-to-one ratio](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4991899/). But I still think of bacteria as mighty beings, packed into a small frame.

***

Last year, a class at the California Institute of Technology further solidified, for me, the dynamism of the microbial world. The course, called _Physical Biology of the Cell_, was taught by an enigmatic professor named Rob Phillips. As a graduate student in the Phillips lab, I considered it my solemn duty to enroll.

Expecting a semester filled with esoteric math equations, I was a bit surprised when the first two weeks of the course were devoted entirely to arithmetic; what the syllabus called **_order-of-magnitude_** thinking.

Order-of-magnitude thinking is a way to estimate mathematical values using nothing but your brain, some paper, and a pen. Basically, if you were stuck on a desert island, with nothing but a stick, and rescue was assured only if you could answer a series of questions, you could very nearly answer questions like _how many red blood cells are in the human body?_ and _how many viruses are in one drop of ocean water?_

With order-of-magnitude thinking, we can’t answer these questions exactly, but we can get pretty close.

When performing these estimations, any answer within an order of magnitude from the truth is considered “good enough”. Calculations are performed in factors of ten, solutions are rounded, and guesses are an integral part of the game. It is basically a loose and fast form of algebra.

But why did a course on physical biology — where scientists often use ultra-sensitive instruments to obtain precise values in their experiments — start with such reckless thinking?

The course began this way, I would later reflect, because so much of biology demands an approximate solution. Every time a scientist mixes up growth media to culture a batch of cells, or dilutes a chemical, or does anything else, they must first determine how much stuff they are working with. How much DNA can be extracted from 5 milliliters of _E. coli_? How much glucose to grow a liter of yeast? These are questions that demand order-of-magnitude thinking.

But, taken outside of the lab, basic estimates and algebraic calculations are even more powerful. Just by sitting down and taking the time to think, we can quantify the world around us. Many people have no sense as to how small a bacterium is compared to a person, or how small a person is compared to, say, a planet. With order-of-magnitude thinking, we place the world in context.
Outside of class, with time on my hands (thanks, coronavirus), I decided to ask myself silly questions, rooted in biology, and to answer them (approximately) with order-of-magnitude thinking. Some of the questions that I asked were strange, like _how long would it take bacteria, dividing every 30 minutes, to consume the earth?_ while others are just intriguing, like _how many bacteria, together, would weigh one gram?_

These are the questions that I will answer in this article. Along the way, just remember that the solution is not all that matters here; the journey is just as important. I hope you will find joy in thinking through and solving a problem, with nothing but your brain, paper, and a pen.

***

Before tackling a question as ambitious as bacteria consuming the earth, we need to start small and get a grasp of the basics of the biological world. To do that, let’s start where we began, and thoroughly debunk the notion that bacteria outnumber human cells ten-to-one. A [research article from 2016](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4991899/) states that “the number of bacteria in the body is actually of the same order as the number of human cells, and their total mass is about 0.2 kg.”

So the article says that the number of human and bacterial cells in the body are roughly the same, but we can verify this claim for ourselves — if a person harbors 0.2 kg of bacterial goop, how many cells are tingling around inside?

To arrive at an answer, we first need to calculate the mass of a single bacterium, a task made difficult, in part, because bacteria come in all sorts of shapes and sizes. Fortunately, we are thinking quickly, not precisely. We will use a typical bacterium, _Escherichia coli_, as our “mathematical model”.

E. coli live in our guts and can be viewed under some microscopes with high-resolution lenses. These cells are typically [2 microns in length, and 1 micron in width](https://www.ncbi.nlm.nih.gov/books/NBK224751/#:~:text=Escherichia%20coli%20is%20a%20typical,with%20radius%20about%200.5%20micrometers.). They look a bit like extended, cylindrical blobs, and their [volume is roughly 1 µm³](http://book.bionumbers.org/how-big-is-an-e-coli-cell-and-what-is-its-mass/#:~:text=One%20of%20the%20simplest%20routes,pico%3D10%2D12).). That’s an approximation, but it’s good enough for our calculations.

A volume of 1 µm³ is tiny; it is about 500 million times smaller than the volume of a grain of sand (assuming the grain of sand has a diameter of 1 mm, and a volume of 0.52 mm³).
Where did these values come from?

When performing order-of-magnitude calculations, there are ample resources at our disposal to “check” our estimates. The best resource for obtaining biological values is [BioNumbers](https://bionumbers.hms.harvard.edu/search.aspx), an online database that includes quantities obtained from thousands of peer-reviewed studies. To find the true size of a protein, for example, search for “protein size” in the search bar. The results that appear will list the relevant value, the units, and the research article that obtained that value. Each entry in BioNumbers also has a unique ID (for example, BNID: 113349), which I will sometimes use in this article to direct you to a specific number.

{% include image-caption.html imageurl="/assets/images/posts/2020/ecoli_dividing.jpg#wide" title="SEM of dividing E. coli" caption="A scanning electron micrograph (SEM) of a dividing E. coli cell. The scale bar is shown at the bottom of the image." %}


While a bacterial volume of 1 µm³ is small, it is difficult to really understand _just how small_ without placing that number in context, and making comparisons.

To do that, let’s consider things that are smaller than a bacterium. Viruses are a good example; a typical virus has a diameter of 100 nanometers. If we approximate a virus as a sphere, then roughly 2,000 of them could fit inside of a single bacterium, and roughly 200,000 viruses could fit inside of a human cell (which have a volume about 100-times greater than that of a bacterium). It would take 1,000 viruses, placed side by side, to span the width of a human hair.

In a final set of comparisons, let’s consider the size of a protein, that fundamental, molecular machine that enables life to carry out its functions. A typical protein in a cell is 5 nanometers in diameter (BNID: 100481) and has a volume of 65 nm³, which means that more than 15 million of them could fit into a single bacterium. When compared to viruses and proteins, bacterial cells are massive!

But let’s return to our initial question; namely, how many bacterial cells are inside of us, given that there is a total mass of about 0.2kg of bacterial cells inside of a 70 kilogram person?

To solve this problem, we first need to figure out the mass of a single bacterium, a problem made challenging, again, because bacteria are so small and difficult to measure. Fortunately, we don’t need to weigh a bacterium — we can throw precision to the wind and make an educated guess.

If we assume, again, that a bacterium is 1 µm³ in volume, then we can easily approximate its mass if we make some assumptions. This is a vital part of “order-of-magnitude” thinking. A “good” assumption to make when calculating the mass of almost any organism is that it is made mostly of water.

Like most cells, bacteria are about [two-thirds water](http://book.bionumbers.org/how-big-is-an-e-coli-cell-and-what-is-its-mass/). Therefore, if a bacterium has a volume of 1 µm³, and approximately the density of water (1000 kg/m³), then it must have a mass of roughly 1 picogram. There are 10¹² picograms in one gram, which means that a trillion bacteria would weigh just one gram.

With these fundamental numbers in hand, we are ready to answer some complex questions.

First, let’s return to our initial question, regarding the number of bacterial cells in the human body. If those bacteria weigh 0.2 kilograms, we can simply divide by 1 picogram to show that there are approximately 2 x 10¹⁴ bacterial cells in the body.

This is a bit more than the estimated value of 3.8 x 10¹³ from the [research article](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4991899/), but our estimate is within an order of magnitude, which is the goal when performing these calculations.

Equipped with a solid understanding of bacterial mass and volume, we are now ready to tackle questions on a larger scale.

***

While size and mass are important values to estimate, they are not particularly interesting. What is far more interesting is that these fundamental numbers can be built upon to answer progressively more difficult questions. The next questions that I want to focus on in this article relate to the metabolism of a cell. Again, we will start with a simple question, and then grow in complexity.

Let’s answer the question: _how many sugars are needed to build a cell?_

This question, and the associated estimates, are taken from an excellent 2009 paper in the [_Proceedings of the National Academy of Sciences_](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2799844/pdf/zpq21465.pdf).

To reach an answer, we first need to make assumptions, based on previous knowledge. For this question, I will assume that _E. coli_ cells double roughly every 30 minutes — a factoid that I picked up from my time in research labs — and I will also assume, again, that _E. coli_ are about 70% water (BNID 100044). These seem like fair assumptions, and it is just fine if we are slightly off in our estimates. The important thing is to think through a problem, and come out with a deeper understanding at the other end.

If a cell weighs one picogram, and is roughly 70% water, then it must consist of 30% of cellular…_stuff_; proteins and DNA and RNA and sugars and many other chemicals. If we assume that most of those compounds have a mass greater than water, than another fair assumption is that a bacteria’ dry mass is about 0.5 picograms. This estimate is backed up by the data, too (BNID 103892, 103904, 102230, 102242).

Let’s make one final assumption, to inch a bit closer to the answer. Let’s assume that, of the 0.5 picograms of dry mass in a bacterium, that a further half of that is carbon. This seems like a good estimate, as carbon is the primary elemental building of life, and is found in every single cellular component. Based on this estimate, a bacterium must have about 0.25 picograms of carbon, which equates to about 10¹⁰ carbon atoms per cell (BNID 103010).

Since each molecule of glucose has six carbon atoms, we can assume that it takes about 2 × 10⁹ sugars to make a new cell!

Thus equipped with our guess, we are ready to answer what is, in my opinion, an immensely intriguing question:

_How long would it take one bacterium to eat one sugar cube?_

***

For this thought experiment, assume that our little, bacterial cell is happily munching on the sugar cube (the same kind that you mix into coffee in the morning) and, every 30 minutes, the bacterium creates another cell. Instead of sticking around, though, that “daughter” cell washes away, while the parent continues eating, on and on, producing clones forever.

The question is, how long would it take that one cell, at “maximum metabolism”, to consume the sugar cube?

Well, every 30 minutes, our imaginary cell is creating a clone, and it requires 2 × 10⁹ sugars to do that. So if we figure out how many sugar molecules are in a sugar cube, and divide by 2 × 10⁹, we can figure out how many minutes it would take our imaginary cell to eat the cube.

A typical sugar cube [weighs 4 grams](https://en.wikipedia.org/wiki/Sugar_cubes#:~:text=Sugar%2C%20shaped%20in%20cubes%20usually,through%20a%20special%20production%20process.) (I looked it up!), a molecule of glucose has a molecular weight of ≈180 grams per mole, and there are 6.02 × 10²³ molecules in one mole (this is called [Avogadro’s number](https://en.wikipedia.org/wiki/Avogadro_constant)). If we do the algebra, we’ll find that there are about 1.34 × 10²² glucose molecules in a single sugar cube. That is about ten times more than there are [stars in the universe](https://scienceline.ucsb.edu/getkey.php?key=3775#:~:text=There%20are%20about%201%2C000%2C000%2C000%2C000%2C000%2C000%2C000%20stars,That%20is%20a%20lot!!), or grains of sand on all the beaches on earth (apparently). It is an incredible number, nestled into a single sugar cube.

If we divide our estimate of 1.34 × 10²² glucose molecules in a single sugar cube by the number of sugars needed to “feed a cell” every 30 minutes, we arrive at ≈ 6.7 × 10¹², the fraction of glucose molecules in the sugar cube compared to the number of glucose molecules needed to build a single bacterium. If we multiply this value by 30 minutes, the time it takes to build a cell, we find that ≈ 2 × 10¹⁴ minutes will elapse before one bacterium, at maximum metabolism, is able to consume a single sugar cube. That’s equivalent to 382,420,091 years . Dinosaurs first roamed the earth about 240,000,000 years ago.

With all of these calculations done, let’s remind ourselves of the “key” values obtained so far:

1. A typical bacterium has a volume of 1 µm³ and weighs 1 picogram.
2. We assume that a cell divides roughly every 30 minutes.
3. It takes about 10¹⁰ carbon atoms to build a cell.

Equipped with our quantitative arsenal, we are now ready to tackle the final question:

_How long would it take a dividing colony of bacteria to consume the planet?_

***

This is a nuanced question, and requires that we slowly build up our understanding of bacterial metabolism and growth. The key to this question is in the phrase dividing colony, which means that we begin with one bacterium and allow that cell to divide for days, or weeks, with infinite nutritional resources. If we continue to feed the growing colony, how long until the earth is exhausted of carbon-based resources?

Well, let’s start by estimating how quickly bacterial cells divide. Using Python and Matplotlib, I’ve made a line plot that shows the exponential growth of a bacterial colony ([using numerical integration with the forward Euler method](http://www.rpgroup.caltech.edu/be262/code/forward_euler.html)), assuming a division time of 33.3 minutes.

{% include image-caption.html imageurl="/assets/images/posts/2020/growth_480_min.png#wide" title="E. coli growth for 480 minutes" caption="Exponential growth of bacterial cells, dividing every 33.3 minutes, for 8 hours." %}


After just 8 hours, a single bacterial cell will give rise to more than 1.5 million cells. If we let the colony grow for several days (with infinite nutritional resources), their numbers quickly surpass the most absurd of values. After a week, our theoretical colony would surpass 10¹¹⁹ cells, a number so vast as to be incomprehensible. This is nearly one hundred orders of magnitude more than the [estimated number of stars in the universe](https://www.space.com/26078-how-many-stars-are-there.html#:~:text=Multiplying%20that%20by%20the%20Milky,quadrillion%20in%20the%20European%20system).) (10²⁴).

For comparison, the mass of the known universe is a paltry 10⁵⁶ grams. If each _E. coli_ weighs one picogram, then 10⁶⁸ E. coli would weigh as much as the known universe…a feat that would (theoretically) take a few days.

{% include image-caption.html imageurl="/assets/images/posts/2020/growth_10080_min.png#wide" title="E. coli growth for 10,080 minutes" caption="Exponential growth of bacterial cells, dividing every 33.3 minutes, for a week. The magnitude of cells soon exceeds all reasonable understanding from our rudimentary thinking." %}


Thank goodness there are not infinite resources, or the planet — and universe — would soon be overrun with bacteria!

But understanding how quickly a population of bacteria will grow does not answer our initial question; to do that, we must first figure out how much carbon is on earth in the first place. A previous study called “The biomass distribution on Earth”, published in PNAS, estimated that “the sum of the biomass across all taxa on Earth is ≈550 Gt C, of which ≈80% (≈450 Gt C) are plants”.

550 Gt is a lot of carbon, but I suspect our theoretical bacterial colony will quickly overrun this supply.

Recall that, to build a single cell, a dividing bacterium requires ≈ 10¹⁰ carbon atoms (BNID 103010). One gigatonne is equal to one billion metric tons (10⁹ tons). If we convert 550 gigatonnes to the actual number of carbon atoms, using the molecular weight of carbon and Avogadro’s number, we can determine that the entire biomass of planet earth consists of approximately 2.75 × 10⁴⁰ atoms of carbon.

Using these estimates, I computed the number of carbon atoms that our growing bacterial colony would consume after a paltry 2500 minutes (nearly 42 hours). After less than two days, they would consume more than 2.75 × 10⁴⁰ atoms of carbon .

In other words, it would take a bacterial colony, without nutritional limitations, less than two days to eat the planet.

{% include image-caption.html imageurl="/assets/images/posts/2020/carbon_consumed_2500_min.png#wide" title="Carbon consumed by dividing E. coli over 2500 minutes" caption="The number of carbon atoms consumed by an exponentially growing bacterial colony, dividing every 33.3 minutes, after 2500 minutes." %}


This is a stunning result that highlights the true power of “exponential” growth. Of course, it is based on estimates. And yes, we made some assumptions (including that the bacterial colony can move about freely and access all of the carbon locked away in biomass).

But this result is powerful because it showcases just how finite earth’s resources really are. That a colony of micron-wide cells could overrun earth’s resources in two days, even theoretically, is a breathtaking thought.

***

Inperforming these calculations, I wanted to showcase the power and utility of “order-of-magnitude” thinking. This skill should not be confined to the lecture halls of prestigious universities — everybody should be able to make estimates, using basic algebra, to advance their thinking at home and in the workplace.

Many of the figures used in this post — such as the size, volume, and mass of a cell, as well as the number of carbon atoms required to build a bacterium — are taken directly from the inspiring work of Rob Phillips, Ron Milo, and others.

Order-of-magnitude thinking provides the first “line of attack” when approaching a problem. Estimates give us a sense of the timing and scale of things; they help put subjects in context. I find that this way of thinking is particularly relevant to a field like biology, where it is otherwise difficult to understand, or appreciate, the size and power of the organisms living beneath our noses.

Now go forth and make estimates!

***

**References:**

[Cell Biology by the Numbers](http://book.bionumbers.org/) — a free e-book on order-of-magnitude thinking and a great resource for quantitative biology.

[BioNumbers](https://bionumbers.hms.harvard.edu/search.aspx), a database of biological numbers.

[_The biomass distribution on Earth_](https://www.pnas.org/content/115/25/6506), by Bar-On, Y.M., Phillips, R. and Milo, R. in PNAS (2018).

[Using Python for numerical integrations, and the Forward Euler method](http://www.rpgroup.caltech.edu/be262/code/forward_euler.html).

***

**Images**

Featured image from Elena Mozhvilo on [Unsplash](https://unsplash.com/photos/HRjdJddvPu8).

Bacterial SEM image from the CDC’s [Public Health Image Library](https://phil.cdc.gov/).

All Python plots made by Niko McCarty, with Matplotlib.