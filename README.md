# silk components
### components for the Silk Web Toolkit

Components can be used to display common text, layout and data-sources inside your silk site. 
(Please note customisable data-sources are not currently supported.)
Build whatever components you need, complement the limited core complements bundled with Silk.

## how to build a component
### manually

* have a look at the handful of samples under org/silkyweb
* find or create a package directory to place your component in
  * placing components in packages helps guarantee uniqueness
* name your component something sensible
  * 'component-missing' shows how static text can be displayed. Note: this text will be displayed if your component can not be found
  * 'site-modified-timestamp' shows how components can be rendered based on a data-source given to them E.G. ':date/timestamp'
* create a directory with the same name as the version of Silk you are using
  * just use the major.minor.patch ie 0.1.0
* create the required .dna config directory
* add a dna.conf definition to .dna, see the examples under org/silkyweb
  * check your package value is the same as the directory hierarchy you have placed your component in
  * silk-version is the version of Silk the component has been built and tested against
  * it is useful to add a quick description of the purpose of the component
* add the component see the examples under /org/silkyweb
  * ensure the filename is the same as the component's name
  * ensure it has an id along the lines of silk-component:component-filename
* test your component by including it in a silk site and 'spinning'

### or with silk

* 'silk clone-component some-component'
* modify the .dna/dna.conf file to suit
* rename and modify the component file to suit 
* in your component's parent directory 'silk install-component'


## how to contribute

### you

* fork this repository
* add your component
* submit a pull request

### us

* review your pull request
* add to silk component repository so your component is available with 'silk update'
