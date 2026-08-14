# CLI (Command Line Interface)

![cli_wall](https://programming.dev/pictrs/image/1d9edc2d-c279-4133-9d07-5dad16fc7692.jpeg?format=webp)


Windows (mac, microsoft) , shoma yechizi darid bename GUI (graphical user interface)


GUI--> YEk rabeti hast beyne user va computer va be shekle graphical hast --> Sheklo shamayel dare



chera vaghty GUI hast ma CLI estefade konim?
1- Choon aksare server ha linux based hastan va cli based hastan
2- Kh az abzar (tools) faghat dar halate cli sakhte shodan



GUI yani -->  ba click mizani rooye Desktop , listesho mibine, chizi bekhay roosh click mikoni open mishe, chizi bekhy delete mikone, new folder -->< folder jadi misazi, file e jadid misazi


Command Line interface -->  CLI 

yani yek safe meshki jolomon bashe va ba oon kar konim...


![cli_terminal](/tutorial_figs/terminal.png)


aksare developer ha az CLI estefade mikonan, na GUI , vaghty migim server gerefte --> yek windowsi --> yek keshvari , yek sherkati , yek tabaghe ei , computer majazi dar ekhtiare shoma gharar mide.


shoma bayad CLI balad bashid k betonid behesh vasl shid.



Baraye neveshtane CLI shoma yek mohit mikhahid : 

Mac --> Command + Space --> search terminal

windows --> CMD , Powershell


Yadeton bashe powershell kh ghavitar va bishtar shabihe terminal hast ta CMD , 


Agar bekahhid tamame in dastoorate terminal ro bezanid dakhele windows mitoni az khode barnameye *git bsh* estefade konid. 






vaghty baz mikonid chenin chizi mibinid : 

```bsh
Last login: Wed Aug  5 20:10:10 on ttys000
(base) apm@APMs-MacBook-Pro ~ % 

```

pas bebinim koja hastim? az dastoori bename **pwd** estefade mikonim

```bsh
(base) apm@APMs-MacBook-Pro ~ % pwd
/Users/apm
```


Tooye CMD ma pwd nadarim va bayad az dastore zir bezani

```bsh
cd
```

ama powershell pwd dare va mitoni estefade koni.




In yani ma jaei hastim bename Users/apm va harchizi benevisim inja ejra mishe. pas agar bekhahim jaei berim masalan agar bekhahim berim desktop, dg mesle GUI injori nist rooye desktop click konim faghat bayad code bezanim masalan 

bekhay jaei beri az dastoore **cd** estefade mikoni


```bsh
(base) apm@APMs-MacBook-Pro ~ % cd desktop
(base) apm@APMs-MacBook-Pro desktop % 
```

In command too powershell va CMD yeksan hast .


mikhay ,motmaen shi bebini kojaei?

```bsh
(base) apm@APMs-MacBook-Pro desktop %  pwd
/Users/apm/desktop
```

yek command dastori hast bename  **ls**

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


in dastoore ls ro ham terminal dare ham powershell ama baraye cmd bayad az **dir** estefade konid.





mikhay yek fodler besazi kafie az dastoore **mkdir** estefade koni

```bsh
(base) apm@APMs-MacBook-Pro desktop % mkdir new_folder
```

bejaye new fodler harchizi bekhahi varedesh beshi az **cd** estefade mikoni


pas ta inja :
- pwd : mige kojaei
- cd : mire dakhelesh
- mkdir : folder misaze
- ls / dir : liste file haro neshon mide



```bsh
(base) apm@APMs-MacBook-Pro desktop % pwd
/Users/apm/desktop
(base) apm@APMs-MacBook-Pro desktop % cd new_folder
(base) apm@APMs-MacBook-Pro new_folder % pwd
/Users/apm/desktop/new_folder
```

File mikhahi besazi? yek dastoor hast bename **touch**


```bsh
(base) apm@APMs-MacBook-Pro new_folder % touch l1.py
(base) apm@APMs-MacBook-Pro new_folder % ls
l1.py
```


CMD va terminal touch ro nadaan va mitonid injori estefade konid

baraye sakhte file tooye powershell

```bsh
New-Tterm a.py
```

baraye dakhele CMD 

```bsh
type nul > a.py
```


behjaye a.py mitonid har file e k mikhahid benevisid.






varede folder1 shodam 3 ta file sakhtam


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
baraye hazfe yek file az dastoore **rm** estfade mikonam

```bsh
(base) apm@APMs-MacBook-Pro folder1 % rm l1.py
(base) apm@APMs-MacBook-Pro folder1 % ls
new_table.csv	req.txt

(base) apm@APMs-MacBook-Pro folder1 % rm req.txt
(base) apm@APMs-MacBook-Pro folder1 % ls
new_table.csv
```


rm ham baraye teminal hast ham baraye powershell ama baraye CMD bayad az commande zir estefade konid

```bsh
del a.py
```




baraye inke back bznm azoon folder bayad **cd ..** bezanam


```bsh
(base) apm@APMs-MacBook-Pro folder1 % cd ..
(base) apm@APMs-MacBook-Pro desktop % pwd
/Users/apm/desktop
```


hazfe folder az **rm** estefade nmikoni az **rm -rf** estefade mikoni

```bsh
(base) apm@APMs-MacBook-Pro desktop % rm -rf folder1
```

tooye powershell bejaye rm -rf bayad az command zir estefade konid

```bsh
Remove-Item folder -Recurse -Force
```

dakehle CMD bayd bazanid

```bsh
rmdir /s /q folder
```

bejaye folder , esme fodler ro beznid









yek dastoor darim bename **vim**

dakhele terminal besorate by default nasb hast vim ama tooye powershell va cmd baayd nasb konid



vim --> NA TANHA file misaze balke ejaze mdie, too file chizi benevisi



touch l1.py --> in faghat file e khali misaze

vim l1.py --> I minevisi harchi mikhay mitoni benvisi
badesh mizani ESC -->  :wq  enter -->na taha filet skhte mishe balek chizaye tosham hast


cat  --> ba in mitoni dakhele file ro bebini chi hast
 

```bsh
(base) apm@APMs-MacBook-Pro folder3 % vim l3.py
(base) apm@APMs-MacBook-Pro folder3 % ls
l1.py	l2.py	l3.py
(base) apm@APMs-MacBook-Pro folder3 % cat l1.py
(base) apm@APMs-MacBook-Pro folder3 % cat l2.py
(base) apm@APMs-MacBook-Pro folder3 % cat l3.py
print('salam')

```



-----------------
## Summary 

shoma varede terminal (mac) , powershell , cmd (windows) mishid . yek safe meshki hast behesh migan bsh (Bash) -->inja yek dargahi (gate) ke mostaghim ba core (hasteye) laptabeton harf bznid bedone niaz b GUI (rabete graphici) 

server ha injorian va hamchenin, bazi az abzaar ha injorian


pwd --> kojam --> mige Users/apm

cd name --> mire oon folderi k mikhahi <br>
cd .. --> barmigarde az jaei k hasti

mkdir name --> yek folder misaze<br>
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


| Mac / Linux | PowerShell | CMD | Example | che mikonad? |
|-------------|------------|-----|---------|--------------|
| `pwd` | `pwd` / `Get-Location` | `cd` | `pwd` | neshan midahad kojaeid |
| `cd` | `cd` | `cd` | `cd desktop` | mire be folderi k mikhahid |
| `cd ..` | `cd ..` | `cd ..` | `cd ..` | bar migarde ye folder aghab |
| `ls` | `ls` / `Get-ChildItem` | `dir` | `ls` | list mikone tamame file va folder haye jaei ke toosh hastid |
| `mkdir` | `mkdir` / `New-Item -ItemType Directory` | `mkdir` / `md` | `mkdir project1` | new folder misaze |
| `touch` | `New-Item` | `type nul >` | Mac: `touch l1.py` <br> PowerShell: `New-Item l1.py -ItemType File` <br> CMD: `type nul > l1.py` | yek file khali misaze |
| `vim` | `vim`* | `vim`* | `vim l1.py` | file ro baz mikone va mitoni edit koni |
| `cat` | `cat` / `Get-Content` | `type` | Mac: `cat l1.py` <br> PowerShell: `Get-Content l1.py` <br> CMD: `type l1.py` | mohtaviate dakhele file ro neshan mide |
| `rm` | `rm` / `Remove-Item` | `del` | Mac: `rm l1.py` <br> PowerShell: `Remove-Item l1.py` <br> CMD: `del l1.py` | yek file ro delete mikone |
| `rm -rf` | `Remove-Item -Recurse -Force` | `rmdir /s /q` | Mac: `rm -rf folder1` <br> PowerShell: `Remove-Item folder1 -Recurse -Force` <br> CMD: `rmdir /s /q folder1` | yek folder ba tamame file haye dakhelesh ro delete mikone |
| `python3` | `python` / `py` | `python` / `py` | Mac: `python3 l1.py` <br> Windows: `python l1.py` | yek Python file ro run mikone |
| `python3 -m venv` | `python -m venv` | `python -m venv` | Mac: `python3 -m venv fanavari` <br> Windows: `python -m venv fanavari` | yek virtual environment misaze |
| `source .../activate` | `.\fanavari\Scripts\Activate.ps1` | `fanavari\Scripts\activate.bat` | Mac: `source fanavari/bin/activate` <br> PowerShell: `.\fanavari\Scripts\Activate.ps1` <br> CMD: `fanavari\Scripts\activate.bat` | virtual environment ro activate mikone |
| `deactivate` | `deactivate` | `deactivate` | `deactivate` | virtual environment ro deactivate mikone |

> `vim` be soorate default dar Windows mojood nist. Agar Vim nasb shode bashad, ham dar PowerShell va ham CMD mitavanid az `vim` estefade konid.










