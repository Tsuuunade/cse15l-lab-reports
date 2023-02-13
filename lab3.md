# Lab 3

**Input 1**
```
$ find non-fiction/  -type f
```

**Output 1**
```
non-fiction/OUP/Abernathy/ch1.txt
non-fiction/OUP/Abernathy/ch14.txt
non-fiction/OUP/Abernathy/ch15.txt
non-fiction/OUP/Abernathy/ch2.txt
non-fiction/OUP/Abernathy/ch3.txt
non-fiction/OUP/Abernathy/ch6.txt
non-fiction/OUP/Abernathy/ch7.txt
non-fiction/OUP/Abernathy/ch8.txt
non-fiction/OUP/Abernathy/ch9.txt
non-fiction/OUP/Berk/ch1.txt
non-fiction/OUP/Berk/ch2.txt
non-fiction/OUP/Berk/CH4.txt
non-fiction/OUP/Berk/ch7.txt
non-fiction/OUP/Castro/chA.txt
non-fiction/OUP/Castro/chB.txt
non-fiction/OUP/Castro/chC.txt
non-fiction/OUP/Castro/chL.txt
non-fiction/OUP/Castro/chM.txt
non-fiction/OUP/Castro/chN.txt
non-fiction/OUP/Castro/chO.txt
non-fiction/OUP/Castro/chP.txt
non-fiction/OUP/Castro/chQ.txt
non-fiction/OUP/Castro/chR.txt
non-fiction/OUP/Castro/chV.txt
non-fiction/OUP/Castro/chW.txt
non-fiction/OUP/Castro/chY.txt
non-fiction/OUP/Castro/chZ.txt
non-fiction/OUP/Fletcher/ch1.txt
non-fiction/OUP/Fletcher/ch10.txt
non-fiction/OUP/Fletcher/ch2.txt
non-fiction/OUP/Fletcher/ch5.txt
non-fiction/OUP/Fletcher/ch6.txt
non-fiction/OUP/Fletcher/ch9.txt
non-fiction/OUP/Kauffman/ch1.txt
non-fiction/OUP/Kauffman/ch10.txt
non-fiction/OUP/Kauffman/ch3.txt
non-fiction/OUP/Kauffman/ch4.txt
non-fiction/OUP/Kauffman/ch5.txt
non-fiction/OUP/Kauffman/ch6.txt
non-fiction/OUP/Kauffman/ch7.txt
non-fiction/OUP/Kauffman/ch8.txt
non-fiction/OUP/Kauffman/ch9.txt
non-fiction/OUP/Rybczynski/ch1.txt
non-fiction/OUP/Rybczynski/ch2.txt
non-fiction/OUP/Rybczynski/ch3.txt
```

**Explanation 1**

This command searches for all files (f for files) within the given directory (non-fiction/ in this case) and all its subdirectories. It's useful if we want to see all files within this directory, but it's mroe useful when there aren't so many files.


**Input 2**
```
$ find non-fiction/OUP/Berk/ -type f
```

**Output 2**
```
non-fiction/OUP/Berk/ch1.txt
non-fiction/OUP/Berk/ch2.txt
non-fiction/OUP/Berk/CH4.txt
non-fiction/OUP/Berk/ch7.txt
```

**Explanation 2**

In this case we can see clearly see that there're four files in the given directory and what are the path for thoese files. Even there's a subdirectory in ```Berk```, we still have access to files inside it.


**Input 3**
```
$ find non-fiction/ -type d
```

**Output 3**
```
non-fiction/
non-fiction/OUP
non-fiction/OUP/Abernathy
non-fiction/OUP/Berk
non-fiction/OUP/Castro
non-fiction/OUP/Fletcher
non-fiction/OUP/Kauffman
non-fiction/OUP/Rybczynski
```

**Explanation 3**

This command searches for all directories (d for directories) within the given directory (non-fiction/ in this case) and all its subdirectories. We can see the directory we created so be more organized.

**Input 4**
```
$ find non-fiction/OUP/Berk/ -type d
```

**Output 4**
```
non-fiction/OUP/Berk/
```

**Explanation 4**

Since there's no subdirectories within ```Berk```, so the output only displays the current directory. It's useful to check the existance of subdirectories.


**Input 5**
```
$ find travel_guides/berlitz2/ -mtime -20
```

**Output 5***
```
travel_guides/berlitz2/
travel_guides/berlitz2/Algarve-History.txt
travel_guides/berlitz2/Algarve-Intro.txt
travel_guides/berlitz2/Algarve-WhatToDo.txt
travel_guides/berlitz2/Algarve-WhereToGo.txt
travel_guides/berlitz2/Amsterdam-History.txt
travel_guides/berlitz2/Amsterdam-Intro.txt
travel_guides/berlitz2/Amsterdam-WhatToDo.txt
travel_guides/berlitz2/Amsterdam-WhereToGo.txt
travel_guides/berlitz2/Athens-History.txt
travel_guides/berlitz2/Athens-Intro.txt
travel_guides/berlitz2/Athens-WhatToDo.txt
travel_guides/berlitz2/Athens-WhereToGo.txt
travel_guides/berlitz2/Bahamas-History.txt
travel_guides/berlitz2/Bahamas-Intro.txt
travel_guides/berlitz2/Bahamas-WhatToDo.txt
travel_guides/berlitz2/Bahamas-WhereToGo.txt
travel_guides/berlitz2/Bali-History.txt
travel_guides/berlitz2/Bali-WhatToDo.txt
travel_guides/berlitz2/Bali-WhereToGo.txt
travel_guides/berlitz2/Barcelona-History.txt
travel_guides/berlitz2/Barcelona-WhatToDo.txt
travel_guides/berlitz2/Barcelona-WhereToGo.txt
travel_guides/berlitz2/Beijing-History.txt
travel_guides/berlitz2/Beijing-WhatToDo.txt
travel_guides/berlitz2/Beijing-WhereToGo.txt
travel_guides/berlitz2/Berlin-History.txt
travel_guides/berlitz2/Berlin-WhatToDo.txt
travel_guides/berlitz2/Berlin-WhereToGo.txt
travel_guides/berlitz2/Bermuda-history.txt
travel_guides/berlitz2/Bermuda-WhatToDo.txt
travel_guides/berlitz2/Bermuda-WhereToGo.txt
travel_guides/berlitz2/Boston-WhereToGo.txt
travel_guides/berlitz2/Budapest-History.txt
travel_guides/berlitz2/Budapest-WhatToDo.txt
travel_guides/berlitz2/Budapest-WhereoGo.txt
travel_guides/berlitz2/California-History.txt
travel_guides/berlitz2/California-WhatToDo.txt
travel_guides/berlitz2/California-WhereToGo.txt
travel_guides/berlitz2/Canada-History.txt
travel_guides/berlitz2/Canada-WhereToGo.txt
travel_guides/berlitz2/CanaryIslands-History.txt
travel_guides/berlitz2/CanaryIslands-WhatToDo.txt
travel_guides/berlitz2/CanaryIslands-WhereToGo.txt
travel_guides/berlitz2/Cancun-History.txt
travel_guides/berlitz2/Cancun-WhatToDo.txt
travel_guides/berlitz2/Cancun-WhereToGo.txt
travel_guides/berlitz2/China-History.txt
travel_guides/berlitz2/China-WhatToDo.txt
travel_guides/berlitz2/China-WhereToGo.txt
travel_guides/berlitz2/Costa-History.txt
travel_guides/berlitz2/Costa-WhatToDo.txt
travel_guides/berlitz2/Costa-WhereToGo.txt
travel_guides/berlitz2/CostaBlanca-History.txt
travel_guides/berlitz2/CostaBlanca-WhatToDo.txt
travel_guides/berlitz2/Crete-History.txt
travel_guides/berlitz2/Crete-WhatToDo.txt
travel_guides/berlitz2/Crete-WhereToGo.txt
travel_guides/berlitz2/CstaBlanca-WhereToGo.txt
travel_guides/berlitz2/Cuba-History.txt
travel_guides/berlitz2/Cuba-WhatToDo.txt
travel_guides/berlitz2/Cuba-WhereToGo.txt
travel_guides/berlitz2/Nepal-History.txt
travel_guides/berlitz2/Nepal-WhatToDo.txt
travel_guides/berlitz2/Nepal-WhereToGo.txt
travel_guides/berlitz2/NewOrleans-History.txt
travel_guides/berlitz2/Paris-WhatToDo.txt
travel_guides/berlitz2/Paris-WhereToGo.txt
travel_guides/berlitz2/Poland-History.txt
travel_guides/berlitz2/Poland-WhatToDo.txt
travel_guides/berlitz2/Portugal-History.txt
travel_guides/berlitz2/Portugal-WhatToDo.txt
travel_guides/berlitz2/Portugal-WhereToGo.txt
travel_guides/berlitz2/PuertoRico-History.txt
travel_guides/berlitz2/PuertoRico-WhatToDo.txt
travel_guides/berlitz2/PuertoRico-WhereToGo.txt
travel_guides/berlitz2/Vallarta-History.txt
travel_guides/berlitz2/Vallarta-WhatToDo.txt
travel_guides/berlitz2/Vallarta-WhereToGo.txt
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
