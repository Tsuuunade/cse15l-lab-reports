# Lab 5

I'd like to explore more command options on ```grep``` this time. I first use the command ```find written_2 > find-results.txt``` to create a file containing all results. I may refer to this file later on in my lab report.

**Input 1**
```
$ grep -v ".txt" find-results.txt
```

**Output 1**
```
written_2
written_2/non-fiction
written_2/non-fiction/OUP
written_2/non-fiction/OUP/Abernathy
written_2/non-fiction/OUP/Berk
written_2/non-fiction/OUP/Castro
written_2/non-fiction/OUP/Fletcher
written_2/non-fiction/OUP/Kauffman
written_2/non-fiction/OUP/Rybczynski
written_2/travel_guides
written_2/travel_guides/berlitz1
written_2/travel_guides/berlitz2
```

**Explanation 1**

This option inverts the match, displaying all lines that do not match the pattern. In this case, it searches for all lines in find-results.txt without the string ```.txt```. It's useful if we want to filtrate something.


**Input 2**
```
$ grep -v "a" ch1.txt
```

**Output 2**
```
A Dying Industry—or Not?
```

**Explanation 2**

We find the line in the given file (ch1.txt in this case) without ```a```. It's quite rare that a line doesn't contain letter a, so I decide to do something interesting and acrtually try it out.


**Input 3**
```
$ grep -w "Kauffman" find-results.txt
```

**Output 3**
```
written_2/non-fiction/OUP/Kauffman
written_2/non-fiction/OUP/Kauffman/ch1.txt
written_2/non-fiction/OUP/Kauffman/ch10.txt
written_2/non-fiction/OUP/Kauffman/ch3.txt
written_2/non-fiction/OUP/Kauffman/ch4.txt
written_2/non-fiction/OUP/Kauffman/ch5.txt
written_2/non-fiction/OUP/Kauffman/ch6.txt
written_2/non-fiction/OUP/Kauffman/ch7.txt
written_2/non-fiction/OUP/Kauffman/ch8.txt
written_2/non-fiction/OUP/Kauffman/ch9.txt
```

**Explanation 3**

This option searches for whole words only, matching only those lines that contain the pattern as a whole word and not as part of another word. So I search in find-result.txt for lines including ```Kauffman```.

**Input 4**
```
$ grep -w "Bond" ch1.txt
```

**Output 4**
```
In the late 1940s, Bond Stores, the largest men’s clothing chain at the time, created a sensation in New York City by offering a wide selection of suits with two pairs of pants instead of one, reintroducing a level of product choice not seen since before the war.1 When the line of hopeful buyers at its Times Square store stretched around the block, Bond had to impose a limit of two suits per customer. During World War II, the apparel and textile industries had been converted to supply field jackets, overcoats, and uniforms to the U.S. and Allied Forces. But in the years immediately following the war, returning soldiers, the end of rationing, and pent-up customer demand meant apparel was in short supply.
Fifty years later, it is hard to imagine a retailer—be it a high-end department store, mass merchandiser, or catalog service—limiting an individual customer’s clothing purchase. Retailers collect detailed point-of-sales information that reflects the real-time demand for goods by consumers. Through new computer systems, they share this information with suppliers who, in turn, can ship orders within days to automated distribution centers. The contemporary equivalent of Bond Stores now has a much better chance of avoiding stock-outs of popular items and the inventory gluts that lead to costly markdowns. By the same token, the overall risk associated with fickle consumers, numerous selling seasons, and segmented markets—along with fierce overseas competition—has currently made this a tough arena for American retailers and manufacturers.
The most surprising aspect of this story is that today’s U.S. apparel and textile industries—left for dead by business commentators and economic analysts in the 1980s—have begun to transform themselves, reaping new competitive advantages. Although Bond Stores’ customers were thrilled by a suit with two pairs of pants, contemporary customers want and expect a huge range of choices, and the consumer desire for limitless variety has kept the American apparel industry alive. In 1995, for instance, American consumers purchased 28.7 outerwear garments (all coats, jackets, shirts, dresses, blouses, sweaters, trousers, slacks, and shorts) per capita; in China the estimated number of such garments was only 2 per capita.2
Supply channels are not new, of course; for centuries, fabric-makers have sold their wares to those who cut and sew garments. But, until recently, most channels in the textile and apparel industries have been characterized by arm’s-length relationships among relatively autonomous firms. It is only since the mid-1980s that a number of market and technological changes have encouraged companies to enhance the links 
among different stages of production and distribution. Indeed, retailers like Wal-Mart Stores, Kmart Corporation, and Dillard’s Inc. have been the driving forces behind changes in manufacturing and logistics 
systems in a way that was unheard of in Bond Stores’ time. For instance, entrepreneur Sam Walton built a retail juggernaut that began with thirty-nine Wal-Mart stores in 1971 and grew to almost three thousand by 1996. He did so by insisting that suppliers implement information technologies for exchanging sales data, adopt standards for product labeling, and use modern methods of material handling that assured customers a variety of products at low prices.
When Bond Stores had customers lining up around the block to buy suits, “casual wear,” as we know it today, did not exist. Even in the 1960s, men wore suits, ties, and hats to the ballpark, and women were clothed in dresses and millinery. As recently as 1969, the dress code at Harvard required undergraduate men to wear a collar, necktie, and jacket in the dining halls; women had to wear a dress or a skirt and blouse. It wasn’t until the 1970s that these vestiges of formality gave way to blue jeans and T-shirts—the casual wear uniform. The 1980s ushered in yuppie brands, and in the 1990s history repeated itself as baby boomers’ children adopted the bedraggled grunge look. Many business firms have “casual days” for office attire. Now six out of ten U.S. employers now have casual days in their workplaces, all but a few establishing this practice during the 1990s. About seven out of ten organizations with dress-down days permit employees to wear polo shirts, jeans, and sneakers.4
The information-integrated channel, with its emphasis on time and product perishability, is the basis for our cautiously optimistic—and unconventional—outlook. Even more important, the forces examined in this book provide a glimpse into processes reshaping a considerable portion of the economy. Consumers no longer line up for a special suit at a store like Bond Stores; they also expect an ever more “fashionable” 
array of cereal products, computers, and automobiles. As the next chapter shows, the changes now under way have their roots in new technologies, just as technical advances in transportation and communication 
shifted the industrial landscape at the end of the last century.
```

**Explanation 4**

These are the lines in a chi1.txt with the word ```Bond```. It's useful when you want to search for a specific word in a long passage.


**Input 5**
```
$ grep -r "sensation" Abernathy/
```

**Output 5***
```
Abernathy/ch1.txt:In the late 1940s, Bond Stores, the largest men’s clothing chain at the time, created a sensation in New York City by offering a wide selection of suits with two pairs of pants instead of one, reintroducing a level of product choice not seen since before the war.1 When the line of hopeful buyers at its Times Square store stretched around the block, Bond had to impose a limit of two suits per customer. During World War II, the apparel and textile industries had been converted to supply field jackets, overcoats, and uniforms to the U.S. and Allied Forces. But in the years immediately following the war, returning soldiers, the end of rationing, and pent-up customer demand meant apparel was in short supply.
```

**Explanation 5**

This option searches for the pattern recursively in all files and subdirectories within the specified directory. Since there's only one sentence in all files and subdirectories for the given directory ```Abernathy/```, there's only one line of output.


**Input 6**
```
$ grep -r "berlitz" travel_guides/
```

**Output 6***
```
Nothing!!!
```

**Explanation 6**

There's nothing in the files in the directory and its potential subdirectories. Only the names of the two subdirectories include ```berlitz```. So result is empty.


**Input 7**
```
$ grep -c ".txt" find-results.txt 
```

**Output 7**
```
224
```

**Explanation 7**

This option displays only the count of matching lines rather than the lines themselves. So if you're not that interested in the content of the lines, you can use this option. It's quiet useful here because I can know the amount of txt files easily.


**Input 8**
```
$ grep -c "100" HandRLosAngeles.txt
```

**Output 8**
```
2
```

**Explanation 8**

We can know that there are two lines match our expectation. This is a useful tool when you want to get a brief information about how much (big percentage or small) does a certain word exist in the file.


**Sources used**

Overall, I use [ChatGPT](https://chat.openai.com/chat). I type in ```can you give me some interesting command line options of command grep``` and it provides me with many options to use the command ```grep```, so I chosse 4 of them and put them into my lab report.
