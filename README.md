# Research seminar website

## Created using:
* [Yeoman](http://yeoman.io/)
* [HTML5 Boilerplate](http://html5boilerplate.com)
* [960.gs](http://960.gs/)

## Steps for updating website
```sh
git pull origin master                         #just in case the site is edited somewhere else
#edit files
grunt                                          #build the website to the folder *dist*
git commit -am "updated for yyyy-mm-dd"        #save changes if everything goes well
git push origin master                         #push updated source code
grunt deploy                                   #deploy to *gh-pages* branch
git push origin gh-pages                       #push the website live!
git checkout master                            #dont forget to switch back
```