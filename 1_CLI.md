# CLI (Command Line Interface)



Windows (mac, microsoft) , shoma yechizi darid bename GUI (graphical user interface)


GUI--> YEk rabeti hast beyne user va computer va be shekle graphical hast --> Sheklo shamayel dare



chera vaghty GUI hast ma cli estefade konim?
1- Choon aksare server ha linux based hastan va cli based hastan
2- Kh az abzar (tools) faghat dar halate cli sakhte shodan




ba click mizani rooye Desktop , listesho mibine, chizi bekhay roosh click mikoni open mishe, chizi bekhy delete mikone, new folder -->< folder jadi misazi, file e jadid misazi


Command Line interface -->  CLI 

yani yek safe meshki jolomon bashe va ba oon kar konim...




![cli_terminal](/tutorial_figs/terminal.png)


aksare developer ha az CLI estefade mikonan na GUI , vaghty migim server gerefte --> yek windowsi --> yek keshvari , yek sherkati , yek tabaghe ei , computer majazi dar ekhtiare shoma gharar mide.



shoma bayad CLI balad bashid k betonid behesh vasl shid.


Mac --> Command + Space --> search terminal


windows --> CMD , Powershell


```bsh
Last login: Wed Aug  5 20:10:10 on ttys000
(base) apm@APMs-MacBook-Pro ~ % 

```


pas bebinim koja hastim? az pwd estefade mikonim

```bsh
(base) apm@APMs-MacBook-Pro ~ % pwd
/Users/apm
```


bekhay jaei beri az cd estefade mikoni


```bsh
(base) apm@APMs-MacBook-Pro ~ % cd desktop
(base) apm@APMs-MacBook-Pro desktop % 
```

mikhay ,motmaen shi?

```bsh
/Users/apm/desktop
```




yek command dastori hast bename 

baraye didaneh az ls estefade mikoni
```bsh
(base) apm@APMs-MacBook-Pro desktop % ls
179542454.png
2-ML.pdf
3-ML AND DL.pdf
AD2 Final Plan.docx
AD2 Final Plan.pdf
AI_Neural_Nets_Intro.ipynb
APM-Bluenest
Ali-Pilehvar-Meibody-CV.pdf
Answer to AD2 Supabase Columns.docx
Answer to AD2 Supabase Columns.pdf
BlueNest
CLI.md
Django Tutorials.docx
Edisu_Swis
Initial Research on MoS2.docx
Knowledge
L1_ADV.py
L2.py


```




mikhay yek fodler besazi

```bsh
(base) apm@APMs-MacBook-Pro desktop % mkdir new_folder
```

bejaye new fodler harchizi bekahhi

varedeszh bessahm --> cd


pwd --> mige kojaei , cd --> mire , mkdir --> fodler misaze, ls --> listo neshonh mide

```bsh
(base) apm@APMs-MacBook-Pro desktop % pwd
/Users/apm/desktop
(base) apm@APMs-MacBook-Pro desktop % cd new_folder
(base) apm@APMs-MacBook-Pro new_folder % pwd
/Users/apm/desktop/new_folder
```


file chijori besazam? touch hast


```bsh
(base) apm@APMs-MacBook-Pro new_folder % touch l1.py
(base) apm@APMs-MacBook-Pro new_folder % ls
l1.py
```


vrede folder1 shodam 3 ta file sakhtam
```bsh
(base) apm@APMs-MacBook-Pro desktop % cd folder1
(base) apm@APMs-MacBook-Pro folder1 % pwd
/Users/apm/desktop/folder1
(base) apm@APMs-MacBook-Pro folder1 % ls
(base) apm@APMs-MacBook-Pro folder1 % touch l1.py
(base) apm@APMs-MacBook-Pro folder1 % touch req.txt
(base) apm@APMs-MacBook-Pro folder1 % touch new_table.csv
(base) apm@APMs-MacBook-Pro folder1 % ls
l1.py		new_table.csv	req.txt

```
baraye hazfe yek file az rm estfade mikonam

```bsh
(base) apm@APMs-MacBook-Pro folder1 % rm l1.py
(base) apm@APMs-MacBook-Pro folder1 % ls
new_table.csv	req.txt

(base) apm@APMs-MacBook-Pro folder1 % rm req.txt
(base) apm@APMs-MacBook-Pro folder1 % ls
new_table.csv
```

baraye inke back bznm azon folder bayad cd .. bezanam
```bsh
(base) apm@APMs-MacBook-Pro folder1 % cd ..
(base) apm@APMs-MacBook-Pro desktop % pwd
/Users/apm/desktop
```


hazfe folder az rm estefade nmikoni az rm -rf estefade mikoni

```bsh
(base) apm@APMs-MacBook-Pro desktop % rm -rf folder1
```



vim --> NA TANHA file misaze balke ejaze mdie, too file chizi benevisi



touch l1.py

vim l1.py --> I minevisi harchi mikhay mitoni benvisi
badesh mizani ESC -->  :wq  enter -->na taha filet skhte mishe balek chizaye tosham hast


cat 
 

```bsh
(base) apm@APMs-MacBook-Pro folder3 % vim l3.py
(base) apm@APMs-MacBook-Pro folder3 % ls
l1.py	l2.py	l3.py
(base) apm@APMs-MacBook-Pro folder3 % cat l1.py
(base) apm@APMs-MacBook-Pro folder3 % cat l2.py
(base) apm@APMs-MacBook-Pro folder3 % cat l3.py
print('salam')

```



## Summary 

shoma varede terminal (mac) , powershell , cmd (windows) mishid . yek safe meshki hast behesh migan bsh (Bash) -->inja yek dargahi (gate) ke mostaghim ba core (hasteye) laptabeton harf bznid bedone niaz b GUI (rabete graphici) 

server ha injorian va hamchenin, bazi az abzaar ha injorian


pwd --> kojam --> mige Users/apm

cd name --> mire oon folderi k mikhahi <br>
cd .. --> barmigarde az jaei k hasti

mkdir name --> yek folder misaze
cd name --> varede oon fodler mishi

touch name.format ---> touch l1.py --> yek file misaze<br>
vim name.format --> vim l1.py --> ham yek file msiaze ham toosh chizi minevsii

ls --> harja bezanid , mohtaviate oon folder ro neshon mide<br>
cat file --> oon file e mohtaviate dakhelesho neshon mide <br>


rm file --> rm l1.py --> yek file ro haZf mikoni <br>
rm -rf folder --> rm -rf folder1 --> yek folder ro hazf mikon i





yek folder sakhtam va toosh yek file e python sakhtam va ba vim rftm toosh 4,5 kaht code zadam

```bsh
(base) apm@APMs-MacBook-Pro desktop % mkdir project1
(base) apm@APMs-MacBook-Pro desktop % pwd
/Users/apm/desktop
(base) apm@APMs-MacBook-Pro desktop % cd project1
(base) apm@APMs-MacBook-Pro project1 % touch l1.py
(base) apm@APMs-MacBook-Pro project1 % vim l1.py
(base) apm@APMs-MacBook-Pro project1 % ls
l1.py
(base) apm@APMs-MacBook-Pro project1 % cat l1.py
print('salam')

a=10
b=30
c = a + b
print(c)

```


baraye ejra kardan l1.py hatman niazi nist k in file .py ro berizam too editor ya IDE , mitonam az terminal runesh konm.

```bsh
(base) apm@APMs-MacBook-Pro project1 % python3 l1.py
```

yahni ba python3 , file l1.py ro run kon.


```bsh
(base) apm@APMs-MacBook-Pro project1 % python3 l1.py
salam
40
```

man mikhaham mohti besazam --> boro too file e projected va benev isi

```bsh
(base) apm@APMs-MacBook-Pro project1 % python3 -m venv fanavari

```

bejay efanavari migoni esme mohtii k mikhahi besazi ro benevisi

```bsh
(base) apm@APMs-MacBook-Pro project1 % ls
fanavari	l1.py
```

faal kardane mohti kafie benvisi

```bsh
(base) apm@APMs-MacBook-Pro project1 % source fanavari/bin/activate
(fanavari) (base) apm@APMs-MacBook-Pro project1 % 


```

az keyabkhone haye fanavari esteafde mikonam




too anaconda felan mohti , spyddr baz krde bashi


```bsh
(fanavari) (base) apm@APMs-MacBook-Pro project1 % deactivate
(base) apm@APMs-MacBook-Pro project1 % 

```


mikhahaam yek file besazam bename git_tutorial.ms toye desktopam

aval bbibm kojam ba pwd


```bsh
(base) apm@APMs-MacBook-Pro project1 % pwd
/Users/apm/desktop/project1
```


beram too desktop --> cd ..


```bsh
(base) apm@APMs-MacBook-Pro project1 % cd ..
(base) apm@APMs-MacBook-Pro desktop % pwd
/Users/apm/desktop
```

tooye deksotp ba touch misazam badsh baz mikonm o toosh minevisak

```bsh
(base) apm@APMs-MacBook-Pro desktop % touch git_tutorial.md
(base) apm@APMs-MacBook-Pro desktop % 
```


------
# Overview

| Command | Example | che mikonad? |
|---------|---------|--------------|
| `pwd` | `pwd` | neshan midahad kojaeid |
| `cd` | `cd desktop` | mire be folderi k mikhahid |
| `cd ..` | `cd ..` | bar migarde ye folder aghab|
| `ls` | `ls` | list mikone tamame folder haye jaei ke toosh hastid|
| `mkdir` | `mkdir project1` | new folder misaze|
| `touch` | `touch l1.py` | yek file e khali misaze |
| `vim` | `vim l1.py` | baz mikone ya misaze yek file va mitoni benevisi (`i` → benevis → `ESC` → `:wq` enter) |
| `cat` | `cat l1.py` | namayesh mide dakhele yek file ro  |
| `rm` | `rm l1.py` |yek file ro delete mikone |
| `rm -rf` | `rm -rf folder1` | yek folder ba tamame file haye toosho delete mikone |
| `python3` | `python3 l1.py` | run mikone yek python file ro  |
| `python3 -m venv` | `python3 -m venv fanavari` | yek mohit misaze |
| `source .../activate` | `source fanavari/bin/activate` | oon mohit ro activate mikone (faal mikone)|
| `deactivate` | `deactivate` | oon mohit ro deactivate miikne |










