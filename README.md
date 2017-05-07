# Base de donn�es des times de Toyunda Mugen

Ceci est la base de donn�es des times de Toyunda Mugen. 

## Format d'un time

Un karaok� Toyunda Mugen est compos� de 3 �l�ments rang�s dans les dossiers

* ini
* lyrics
* videos

### Dossier "ini"

C'est le fichier qui contient les informations permettant d'afficher le time dans la liste et que le daemon Toyunda Mugen le g�re ensuite. Il est d�riv� du format des .ini de Toyunda d4epitanime


Exemple :
```origin=Bakaclub
aviname=Beck Mongorian Chop Squad - OP - Hit in the USA.avi
file=dummy.ass```

* **origin** : Facultatif, stipule l'origine d'un karaoke. 
* **aviname** : Nom du fichier vid�o, tel quel dans le dossier des Vid�os. Toyunda Mugen lit tout ce que peut lire mpv.
* **file** : Nom du fichier de sous-titres tel que trouvable dans le dossier lyrics
	* Formats accept�s :
		* ass
		* srt
		* vtt
		* txt (format Toyunda)
	* Cas sp�cial : dummy.ass qui n'existe pas et est utilis� quand le fichier vid�o contient d�j� des sous-titres, soit incrust�s (hardsub) soit embarqu�s (ass dans la piste sous-titres d'un mkv). Dans ce cas, Toyunda Mugen ira extraire le sous-titre � la vol�e avant la lecture du karaok� pour le modifier avant lecture.

### Dossier "lyrics"

Contient le fichier de sous-titres tel que sp�cifi� dans le .ini

### Dossier "videos"

Contient le fichier de vid�o tel que sp�cifi� dans le .ini

Les vid�os ne sont pas fournies dans ce d�p�t, par souci de place (et �a ferait un d�p�t de 170 Go au bas mot). Des tas d'openings peuvent se retrouver sur Youtube.


