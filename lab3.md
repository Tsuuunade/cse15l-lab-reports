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
