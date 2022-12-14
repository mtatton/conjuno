```
----------------------------------------------

           CONSOLE JUPYTER NOTEBOOK

----------------------------------------------
            _______ _______ ______ 
           |   _   |   _   |   _  \
           |.  1___|.  |   |.  |   |
           |.  |___|.  |   |.  |   |
           |:  1   |:  1   |:  |   |
           |::.. . |::.. . |::.|   | 
           `-------`-------`--- ---`
                      SOLE
      _______ ___ ___   ______  _______
     |   _   |   Y   | |   _  \|   _   |
     |___|   |.  |   | |.  |   |.  |   |
     |.  |   |.  |   | |.  |   |.  |   |
     |:  1   |:  1   | |:  |   |:  1   |
     |::.. . |::.. . | |::.|   |::.. . |
     `-------`-------` `--- ---`-------'
           PYTER             TEBOOK
   
----------------------------------------------

              CONJUNO 0.1.0

----------------------------------------------

  install : pip3 install -U conjuno
  prereq  : python3.9
  run     : conjuno

----------------------------------------------
  
  Keyboard:

  enter, ctrl+e - run current cell
  t - run as external program (e.g. curses)
  u, page up - scroll fullscreen page up
  n, page down - scroll fulscreen page down 
  h, left - scroll fullscreen left more
  l, right - scroll fullscreen right more
  h, left - scroll fullscreen left
  l, right - scroll fullscreen right
  i - switch to input
  o - switch to output
  f - switch current pad full-screen
  r - reset layout
  gg - go to first cell
  shift+g (G) - go to last cell
  k, up - previous cell
  j, down - next cell
  a - insert cell above current cell
  a - insert cell below current cell
  x - cut cell
  c - copy the cell
  ctrl+v - paste cell above
  ctrl+v - paste cell below
  s, ctrl+s - save notebook
  e - edit input cell [1]
  ctrl+p - run all cells one by one
  q - quit
  
----------------------------------------------

  [1] uses tmp.txt in current directory

----------------------------------------------

  Tips:

  * You can save file and exit vim faster 
    using ZZ keyboard shortcut

  * On Windows You can download unofficial
    ncurses from:

  https://www.lfd.uci.edu/~gohlke/pythonlibs

----------------------------------------------

  Command line parameters:


 -d, --debug
   turns on kernel debug messages

 -k kernel_type, --kernel kernel_type
   runs conjuno with specified kernel
   when no kernel is specified python3
   kernel is used

 -n, --no-kernel
   runs conjuno with no kernel

 -v, --version
   displays the current program version

 -r, --run
   runs notebook and saves result 
   into <fname>_run.ipynb
   

----------------------------------------------

  Changelog:

  0.1.0 - Minor Bugfixing. The cell output is
    now correctly stored to executing cells
    not current cell as expected.

  0.0.9 - Rewritten the keyboard control. Now
    it's completly asynchronous. Added several
    keys. First try to include the time counter.

  0.0.8 - Minor Bugfixing. Added -r parameter
    to run the notebook and save the output
    to a {fname}_run.ipynb notebook file.
    Markdown Cells are displayed fullscreen
    by default.

  0.0.7 - Minor Bugfixing

  0.0.6 - Minor Bugfixing

  0.0.5 - Minor Bugfixing

  0.0.4 - Curses pad to show more of the 
    input and output content possibility 
    to show the cell input or output full 
    screen. And possibility to scroll the 
    content around. Console resizing 
    handler.

  0.0.3 - Added traceaback printing from 
    python3 kernel, added yet another 
    level of DEBUG. If it's set to 2 in
    the log.py then the trace is printed
    to file in case of exception. Added
    support for ctrl-c program exit.
    Prepare for terminal resizing events.
    The complication is from processing
    unix signals in async events. Yet
    for the traceback of python3 kernel
    when it detects an exception is the
    render_ans method in the console
    Class. It it used to display uniform
    traceback and exception. The colors
    are not yet to be added. But it is
    planned in the future version.

  0.0.2 - Asynchronous execution of the
    cell and the possibility to quit 
    the program while the kernel is 
    executing the cell. There was a try
    to add time counter to measure the
    execution time but this will be 
    probably added in the future 
    eventually. 
  
  0.0.1 - Intial version. The very basis
    for this was nbterm. Or rather it's
    for nbtermix. Then I decided to change
    the principle of the work with the 
    notebook on terminal. Instead of 
    trying to simulate the web version it
    was decided to switch to full-screen
    mode for each the cell. That means
    only the first line of input is
    displayed. And when user wants to edit
    the cell the external editor is used.
    So far this approach leaves almost
    the whole screen to the output. I would
    like to prepare the possibility to 
    switch between full screen input, output
    and divided screen for input and output.
    But the only one cell per screen seems
    quite working by now. Another decision
    than eliminating other drawing libraries
    than curses was to use getopt for the
    options as it's the very standard in
    the *nix world. There was a quite
    reduction in the number of the working
    parameters and others are to be added
    eventually.

----------------------------------------------

  Note: This is de facto modified nbterm.
        The difference is it uses only
        ncurses.

----------------------------------------------

  This is highly EXPERIMENTAL software.
  I take no responsibility nor even implied 
  responsibility for any damage, harm or any 
  consequences caused by use of this 
  software. The software found here is
  provided as it is without any liability, 
  guarantees or support.

  The software here is provided ONLY 
  for research purposes.

----------------------------------------------
```


IMAGES:

![CONJUNO 001](https://raw.githubusercontent.com/mtatton/conjuno/master/img/20220808_conjuno_001.png)
![CONJUNO 001](https://raw.githubusercontent.com/mtatton/conjuno/master/img/20220808_conjuno_002.png)
![CONJUNO 001](https://raw.githubusercontent.com/mtatton/conjuno/master/img/20220808_conjuno_003.png)

