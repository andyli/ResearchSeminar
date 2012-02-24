# Research seminar website

## Created using:
* [HTML5 Boilerplate](http://html5boilerplate.com)
* [960.gs](http://960.gs/)

## Steps for updating website
	git pull origin master #just in case the site is edited somewhere else
	#edit files
	cd build && ant && cd .. #build the website to the folder *publish*
	git commit -am "updated for ddmmyyyy" #save changes if everything goes well
	git push origin master #push updated source code
	git checkout gh-pages
	ls -1 | grep -v 'publish' | xargs -I {} rm -rf {} #remove everything except *publish*
	cp -a publish/* publish/[^.]* . #copy everything in *publish* to root
	rm -rf publish #remove *publish*
	git add .
	git commit -am "sync with master"
	git push origin gh-pages #push the website live!
	git checkout master #dont forget to switch back