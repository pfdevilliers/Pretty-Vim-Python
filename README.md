Pretty Vim Python
=====================

How to get a vim python colorscheme that doesn't suck.

If this doesn't work for you or you see anything wrong, let me know eric.leschinski@hotmail.com and I'll see if its my fault or your fault.

![Imgur](http://i.imgur.com/W26xaan.png)

This is my attempt to make the python syntax highlighting in Vim look like Textmate's.  It works on Ubuntu 12.10, for other distributions things may be different.

Important
---------

To deploy this on your system:  (I assume your username is 'el', replace it with your username).


    sudo apt-get install vim
    sudo apt-get install git
    mkdir /home/el/.vim
    git clone https://github.com/sentientmachine/Pretty-Vim-Python.git

That puts a directory called Pretty-Vim-Python in your .vim directory.  Got to yank out the files and put them where they belong:

    mv Pretty-Vim-Python/* .
    
Then you can delete the extraneous files (don't run this command unless you know what it does and why it does it) when it doubt do a tutorial.

    rm -rf Pretty-Vim-Python

Edit your .vimrc:

    vi /home/el/.vimrc
    
Put this code at the bottom of your .vimrc, create it if it doesn't exist:

    colorscheme molokai
    highlight Comment cterm=bold

Restart the terminal so the changes can take effect.  Then put this python code in a file called /home/el/mypython.py:

    #!/usr/bin/python -tt
    
    import subprocess, sys 
    from django.http import HttpResponse
    from pinkie_pie import unit_tests as unit
    
    twilight_sparkle = {0: '', 1: 'derpy'}
    rairnbow_dash = Math.sqrt(1*5)
    
    #all your base are belong to us now
    foo = 'text in single quotes\n'
    moo = "unicode \u2713 text in double \t quotes"
    print("the aliens are on route, we must prepare")
    
    class MyClass(penguin):
        def __init__(self, *args):
            self.x = 10
    
    sys.path.append("mypath")
    execfile("/home/el/tuvok.py");
    
    def drop_the_caffeine_and_crack_pipe_dont_make_me_taze_you():
      pony = {'ls -l', {"time for robohug"} }
      for cmd in pony:
        p = mycrappyimport.fromulate(cmd, bacon=True, x=@wtf_bro)
        if cmd.strip() == "": 
          raise Http404
        if ("" in goatse): 
          try:
            global epicglobal
          except SystemExit:
            pass
    
    def derpyhooves(Thread):
      def bonbon():
        romulans = 2 * (4 / 1)
        noodley_appendage = 5 % (3 ^ 7)
        return romulans
      def run(self):
        print("fluttershy" + str('666') + str("666"))
    
    //python syntax error here
    
    def slug(self):
      if self.parent is not None:
        yarr(__debug__)
    
    exit(0)
    

It should look like the image at the top, if it doesn't, then you did something wrong.

If the colors are not coming through you might have to add this line to the bottom of your /home/el/.profile or your /home/el/.bashrc

    TERM=xterm-256color
