[![nsxiv](https://codeberg.org/nsxiv/pages/raw/branch/master/img/logo.png)](https://codeberg.org/nsxiv/nsxiv)

NSXIV with video & document library scripts
-------------------------------------------

With the scripts `liblist` and `animelist` you can make nsxiv your movie/e-reader launcher.

Usage
-----

- Change the variable **library_dir** in `liblist` and **anime_dir** in `animelist` to your anime or library paths.
- Download a cover for the specific movie/anime as `cover.jpg` and place inside the respective directories.
- Keep a cover of the book/document in its respective directory with the same name the book/document.
- Copy the scripts at `scripts` folder to your path.
- Copy the `etc/examples/key-handler` file to the respective config path of nsxiv.
- Bind a keybinding to execute each script seperately.

animelist
---------

- Pressing the keybinding or executing the script `animelist` will open nsxiv in thumbnail mode.
- Goto to thumbnail you want and press Space + p (p = play).
- This will open mpv on the directory the `cover.jpg` is from and kills nsxiv.

liblist
-------

- Pressing the keybinding or executing the script `liblist` will open dmeu in the directory given to **library_dir**.
- Choose what catagory you want or All to show all the books/documents.
- Nsxiv opens in thumbnail mode with all the book/document covers.
- Goto to thumbnail you want and press Space + l.
- Nsxiv will see if there is a PDF or EPUB file with the same name as the image and opens it in zathura and kills nsxiv.

Requirements
------------

- X11
- dmenu
- zathura
- mpv
- notify-send
