# instalação simples do Openbox no Debian Buster

:<>: instalar e configurar o Openbox no Debian 10 "Buster" :<>: <br />
-- Lembrando, se você estiver em um desktop<br />
leve em consideração ter instalado o <br />
Debian sem nenhuma interface gráfica <br />
ou gerenciador de janelas. <br />

$ sudo aptitude install xorg openbox xdm<br />
-- reinicia a maquina<br />
-- logue normalmente<br />

-- Instalando Dock<br />
$ sudo apt-get install cairo-dock<br />

-- Adiciona cairo-dock ao ‘autostart’<br />
$ nano ~/.config/openbox/autostart<br />

-- Add o comando ao arquivo<br />
$ nano ~/.config/openbox/autostart<br />
cairo-dock &<br />

-- Wallpaper<br />
$ sudo apt-get install feh<br />

-- Add este comando no arquivo nano ~/.config/openbox/autostart<br />
$ feh — bg-scale /path/to/your/background/image.jpg<br />

-- Bonus este é o comando para configurar 2 monitores no leptop<br />
-- não testei no desktop*<br />
xrandr --output VGA-1 --mode 1440x900 --rate 59.89 --left-of LVDS-1 --output LVDS-1 --mode 1366x768 --rate 60.10<br />

-- Meu arquivo ~/.config/openbox/autostart ta assim<br />
xrandr --output VGA-1 --mode 1440x900 --rate 59.89 --left-of LVDS-1 --output LVDS-1 --mode 1366x768 --rate 60.10 &<br />
feh --bg-scale /home/izaias/Imagens/wallpapers/05VrI7H.jpg & cairo-dock &<br />

-- Considerações finais<br />
Este tutorial foi baseado em um artigo sobre o arch <br />
Linux e o meu setup é um leptop positivo com 4g de memoria <br />
hd mecânico de 500g processador Celeron(R) Dual-Core CPU T3300 2.00GHz <br />
placa mãe POSITIVO M14<br />
 [Creditos](https://medium.com/canivete-sui%C3%A7o-hacker/instala-e-configurar-o-openbox-37c054c759f2)<br />
 [Instalação mimima Debian](https://medium.com/canivete-sui%C3%A7o-hacker/guia-para-uma-instala%C3%A7%C3%A3o-m%C3%ADnima-do-debian-linux-debian-core-abee1218d6b)<br />
 # Ajuda para estudos e laboratorio
 
![openbox](https://user-images.githubusercontent.com/20734038/143509108-dff83ac0-aa78-4219-98a5-b76a91b1cd98.png)

# Obrigado!
 
