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

This command searches for all files modified within the last 20 (we can change this number) days within the directory (travel_guides/berlitz2/ in this case) and all its subdirectories. We can use this command to find our most recent updated files for instance.


**Input 6**
```
$ find travel_guides/berlitz2/ -mtime -5
```

**Output 6***
```
Nothing!!!
```

**Explanation 6**
From the output, we can know that there's no files in the gien directory and files in its subdirectories that are modified within 5 days. This is a good way to check the time we modify those files.


**Input 7**
```
$ find berlitz1/ -name "*.txt" -print
```

**Output 7**
```
berlitz1/HandRHawaii.txt
berlitz1/HandRHongKong.txt
berlitz1/HandRIbiza.txt
berlitz1/HandRIsrael.txt
berlitz1/HandRIstanbul.txt
berlitz1/HandRJamaica.txt
berlitz1/HandRJerusalem.txt
berlitz1/HandRLakeDistrict.txt
berlitz1/HandRLasVegas.txt
berlitz1/HandRLisbon.txt
berlitz1/HandRLosAngeles.txt
berlitz1/HandRMadeira.txt
berlitz1/HandRMadrid.txt
berlitz1/HandRMallorca.txt
berlitz1/HistoryDublin.txt
berlitz1/HistoryEdinburgh.txt
berlitz1/HistoryEgypt.txt
berlitz1/HistoryFrance.txt
berlitz1/HistoryFWI.txt
berlitz1/HistoryGreek.txt
berlitz1/HistoryHawaii.txt
berlitz1/HistoryHongKong.txt
berlitz1/HistoryIbiza.txt
berlitz1/HistoryIndia.txt
berlitz1/HistoryIsrael.txt
berlitz1/HistoryIstanbul.txt
berlitz1/HistoryItaly.txt
berlitz1/HistoryJamaica.txt
berlitz1/HistoryJapan.txt
berlitz1/HistoryJerusalem.txt
berlitz1/HistoryLakeDistrict.txt
berlitz1/HistoryLasVegas.txt
berlitz1/HistoryMadeira.txt
berlitz1/HistoryMadrid.txt
berlitz1/HistoryMalaysia.txt
berlitz1/HistoryMallorca.txt
berlitz1/IntroDublin.txt
berlitz1/IntroEdinburgh.txt
berlitz1/IntroEgypt.txt
berlitz1/IntroFrance.txt
berlitz1/IntroFWI.txt
berlitz1/IntroGreek.txt
berlitz1/IntroHongKong.txt
berlitz1/IntroIbiza.txt
berlitz1/IntroIndia.txt
berlitz1/IntroIsrael.txt
berlitz1/IntroIstanbul.txt
berlitz1/IntroItaly.txt
berlitz1/IntroJamaica.txt
berlitz1/IntroJapan.txt
berlitz1/IntroJerusalem.txt
berlitz1/IntroLakeDistrict.txt
berlitz1/IntroLasVegas.txt
berlitz1/IntroLosAngeles.txt
berlitz1/IntroMadeira.txt
berlitz1/IntroMadrid.txt
berlitz1/IntroMalaysia.txt
berlitz1/IntroMallorca.txt
berlitz1/JungleMalaysia.txt
berlitz1/WhatToDublin.txt
berlitz1/WhatToEdinburgh.txt
berlitz1/WhatToEgypt.txt
berlitz1/WhatToFrance.txt
berlitz1/WhatToFWI.txt
berlitz1/WhatToGreek.txt
berlitz1/WhatToHawaii.txt
berlitz1/WhatToHongKong.txt
berlitz1/WhatToIbiza.txt
berlitz1/WhatToIndia.txt
berlitz1/WhatToIsrael.txt
berlitz1/WhatToIstanbul.txt
berlitz1/WhatToItaly.txt
berlitz1/WhatToJamaica.txt
berlitz1/WhatToJapan.txt
berlitz1/WhatToLakeDistrict.txt
berlitz1/WhatToLasVegas.txt
berlitz1/WhatToLosAngeles.txt
berlitz1/WhatToMadeira.txt
berlitz1/WhatToMalaysia.txt
berlitz1/WhatToMallorca.txt
berlitz1/WhereToDublin.txt
berlitz1/WhereToEdinburgh.txt
berlitz1/WhereToEgypt.txt
berlitz1/WhereToFrance.txt
berlitz1/WhereToFWI.txt
berlitz1/WhereToGreek.txt
berlitz1/WhereToHawaii.txt
berlitz1/WhereToHongKong.txt
berlitz1/WhereToIbiza.txt
berlitz1/WhereToIndia.txt
berlitz1/WhereToIsrael.txt
berlitz1/WhereToIstanbul.txt
berlitz1/WhereToItaly.txt
berlitz1/WhereToJapan.txt
berlitz1/WhereToJerusalem.txt
berlitz1/WhereToLakeDistrict.txt
berlitz1/WhereToLosAngeles.txt
berlitz1/WhereToMadeira.txt
berlitz1/WhereToMadrid.txt
berlitz1/WhereToMalaysia.txt
berlitz1/WhereToMallorca.txt
```

**Explanation 7**

This command searchs for all files with the ```.txt``` extension within the given directory (berlitz1 in this case) and its subdirectories, and print the names of the files found. It's useful since we can have access to all filenames.


**Input 8**
```
$ find non-fiction/OUP/Rybczynski/ -name "*.txt" -print
```

**Output 8**
```
non-fiction/OUP/Rybczynski/ch1.txt
non-fiction/OUP/Rybczynski/ch2.txt
non-fiction/OUP/Rybczynski/ch3.txt
```

**Explanation 8**

For a small directory, we can clearly see the filenames in the terminal. We don't have to look for them in the open editor.


**Sources used**

Overall, I only use [ChatGPT](https://chat.openai.com/chat). I type in ```find command-line options or alternate ways to use the command``` and it provides me with many options to use the command ```find```, so I chosse 4 of them and put them into my lab report.
