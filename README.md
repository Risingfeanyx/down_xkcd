# down_xkcd
a simple bash script to pull xkcd from the internet archive. pulls Volume 0 as well

```
(
clear
wget -nc https://archive.org/download/2009Xkcd/2009_xkcd.pdf&
wget -nc https://archive.org/download/xkcd.7z/xkcd.7z
7za x xkcd.7z
cd xkcd
convert *.png xkcd_$(date +%F).pdf
open xkcd_$(date +%F).pdf
)
```
