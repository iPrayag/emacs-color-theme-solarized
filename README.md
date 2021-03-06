Original at [Solarized Colorscheme for Emacs](https://github.com/sellout/emacs-color-theme-solarized/blob/master/README.md)

Screenshots
-----------

![solarized dark](https://github.com/altercation/solarized/raw/master/img/solarized-vim.png)

Installation & Usage
--------------------

### emacs 24

0. If `emacs24` [not installed](http://wikemacs.org/wiki/Installing_Emacs_on_GNU/Linux#Emacs_24)
   ```
      $ sudo apt-add-repository ppa:cassou/emacs
      $ sudo apt-get install emacs24
   ```

1. install `color-theme-solarized`

   ```
      $ git clone https://github.com/sellout/emacs-color-theme-solarized.git;
      $ sudo mv emacs-color-theme-solarized ~/.emacs.d/emacs-color-theme-solarized
   ```
   
   [OR](http://david.rothlis.net/emacs/customize_colors.html)

    `$ cd ~/.emacs.d;`

    `$ git submodule add https://github.com/sellout/emacs-color-theme-solarized.git;`

   OR 
   
   install from [marmalade](http://marmalade-repo.org/) using :

    `package-install color-theme-solarized`
   
2. Add `(load-theme 'solarized-[light|dark] t)` to your emacs init file.

   The final `.emacs.d/init.el` looks as : 

    `(add-to-list 'custom-theme-load-path "~/.emacs.d/emacs-color-theme-solarized")`
    
    `(load-theme 'solarized-dark t)`

3. Reload the init file, or restart emacs24.

### [color-theme] \(pre-Emacs 24\)

1. Download and install [color-theme].
2. Add the `emacs-color-theme-solarized` directory to your Emacs `load-path`.
3. Add `(require 'color-theme-solarized)` to your Emacs init file (usually `~/.emacs`).
3. Reload the init file, or restart Emacs.
4. Use the usual [color-theme] mechanism to select one of the Solarized themes, or `M-x color-theme-solarized-[light|dark]`.

Advanced Configuration
----------------------

Solarized will work out of the box with just the instructions specified above
but does include several variables that can be customized.

    variable name            default   optional
    --------------------------------------------
    solarized-termcolors =   16    |   256
    solarized-degrade    =   nil   |   t
    solarized-bold       =   t     |   nil
    solarized-underline  =   t     |   nil
    solarized-italic     =   t     |   nil
    solarized-contrast   =   normal|   high, low
    solarized-visibility =   normal|   high, low
    solarized-broken-srgb=   nil   |   t (see details for Mac behavior)
    --------------------------------------------

