Aquaria
=======

Aquaria OpenGL game

engine
	https://github.com/fgenesis/Aquaria.git	branch "experimental"


data from the legal games need to convert
see here https://aur.archlinux.org/packages/aquaria-data-hib/ 

and use this script from there
******************************************
  # Remove binaries & libraries, and other redundant files
  rm {aquaria,xdg-open,lib*}
  rm README-linux.txt
  rm -r gfx/nag


while read line; do echo -n '.'; done < <(  # show progress as dots
    find */ -name '*.png' | xargs ./pngrim  
); echo
******************************************

also need for conversion pngrim from git://github.com/fgenesis/pngrim.git



And most importantly need - (GL - GLES) runtime translator

from https://github.com/lunixbochs/glshim.git

	
	
