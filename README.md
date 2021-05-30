Tabular
==============
Sometimes, it's useful to line up text.  Naturally, it's nicer to have the
computer do this for you, since aligning things by hand quickly becomes
unpleasant.  While there are other plugins for aligning text, the ones I've
tried are either impossibly difficult to understand and use, or too simplistic
to handle complicated tasks.  This plugin aims to make the easy things easy
and the hard things possible, without providing an unnecessarily obtuse
interface.

See [Aligning Text with Tabular.vim](http://vimcasts.org/episodes/aligning-text-with-tabular-vim/)
for a screencast that shows how Tabular.vim works.

Demo
==============

![Alt text](https://i.imgur.com/TtZMpVg.gif?raw=true "this text shows when user hovers mouse") 

Usage Guide
==============

[vimcasts-org-aligning-text-with-tabular-vim.pdf](./vimcasts-org-aligning-text-with-tabular-vim.pdf)

Installation
==============

If you don't have a preferred installation method, I recommend installing
[pathogen.vim](https://github.com/tpope/vim-pathogen), and then simply
copy and paste:

    mkdir -p ~/.vim/bundle
    cd ~/.vim/bundle
    git clone git://github.com/godlygeek/tabular.git

Once help tags have been generated (either using Pathogen's `:Helptags`
command, or by pointing vim's `:helptags` command at the directory where you
installed Tabular), you can view the manual with `:help tabular`.

Detailed Documentation.
==============
See [doc/Tabular.txt](http://raw.github.com/sentientmachine/tabular/master/doc/Tabular.txt)


Bypassing installer, Jist for ripping out the source and grafting it onto our stack
==============

    copy and paste the file ./tabular/plugin/Tabular.vim into your ~/.vim/plugin/Tabular.vim
    copy and paste the file ./tabular/autoload/tabular.vim into your ~/.vim/plugin/tabular.vim
    copy and paste the file ./tabular/after/plugin/TabularMaps.vim into your ~/.vim/after/ftplugin/TabularMaps.vim
    
Usage Example
==============

    vim your_csv.csv
    :Tabularize /,
