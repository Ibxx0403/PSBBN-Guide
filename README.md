Denne guide er til at tilføje flere spil til PS2 drevet. 
Jeg anbefaler at man går hele guiden igennem samt videor, inden man går i gang med nogle af trinene. 







Da man skal bruge Linux mint eller andre debian distributioner kan man enten installere Linux på sin computer og dual boote, eller installere en virtual machine. 

Hvis man ønsker at bruge en virtual machine kan man bruge redskabet VirtualBox, få at kunne køre linux i windows. 

https://www.virtualbox.org/wiki/Downloads

Jeg har linket en guide som viser hvordan man kan få VirtualBox op at køre. 

https://www.youtube.com/watch?v=nvdnQX9UkMY


Det styresystem man skal køre (ISO fil) er Linux mint 

Download begynder med det samme, når man åbner linket. 

http://ftp.klid.dk/ftp/linuxmint/stable/22.1/linuxmint-22.1-cinnamon-64bit.iso



Efter at man har sat linux mint op, skal man første gang, tilføje sit PS2 drev med spil, og sit USB  / eksterne drev hvor man ønsker at opbevare de spil som skal overføres til PS2 konsollen. 

Alternativt kan man gøre brug af tomme filer som er navngivent korrekt, dette vil gøre at man kan have flere spil på sit drev, men vis ps2 drevet bliver formateret, vil denne metode ikke længere virke og man vil blive nødt til at have de fulde spil filer. 

Jeg har vedhæftet de tomme filer, som kan bruges i stedet for de større filer i følgende link. (Direkt download, kan også findes på denne github)

https://github.com/Ibxx0403/PSBBN-Guide/raw/refs/heads/main/blank_games.zip



Først skal man lave en mappe i USB drevet der hedder games


Nu skal man overføre følgende mapper fra PS2 drev (OPL) til games mappen. 
![Alt text](Images/game_transfer_usb.png?raw=true "Title")
CD, DVD, POPS disse mapper indeholder alle de spil som er på PS2 drevet (OPL)



Årsagen til at de skal kopieres til USB er så spillene ikke bliver slettet når man ønsker at overføre nye spil, dette vil tage noget tid, hvis man ikke bruger de tomme filer. 


Nu skal selve programmet til at overføre spillene installeres. Dette kan gøres ved at følge trinnene fra videoen neden under 

https://youtu.be/LLmJPF-XVxs?si=0PQvcrMvff62D8MI&t=916

Se videoen fra 15:16 til 21:13

Efter at havet installeret programmet, kan man slette mappen games i PSBBN mappen. 

Herefter indsættes USB drevet i computeren, man vil nu kunne kopiere lokationen af games mappen.
Nu åbnes PSBBN mappen i terminalen, dette kan gøres med et højre klik. 

Derefter bruger man følgende kommando.

ln -s /path/to/new/games/folder games

hvor "/path/to/new/games/folder" slettes og erstattes med den kopieret lokation. Denne kommando linker ens usb mappe til PSBBN programmet. Et eksempel vises underneden hvor "/media/ibxx0402/PS2 HDD" er lokationen.

![Alt text](Images/folder_link.png?raw=true "Title")


Nu kan man tilføje SSD / HDD til computeren som de nye spil skal tilføjes til, siden der er tale om 2.5 drev behøver man ikke en adapter som skal have strøm forbindelse.

Derefter skip til 27:15 som viser processen for resten af installationen eller klik på følgende link

https://youtu.be/LLmJPF-XVxs?si=O4kHXu8R7b9ioHHt&t=1634


Dog vil der være et ekstra step ved 27:54, vil der blive spurgt om OPL eller Neutrino, her vælges OPL ved at trykke 1. 

![Alt text](Images/install_choice.png?raw=true "Title")

