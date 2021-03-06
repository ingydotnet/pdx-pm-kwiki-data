The only two Emacs keybindings I know are Ctrl-A and Ctrl-E for jumping to the start and end of a line respectively.  I hate to lose these in screen sessions, so I map my screen control key to Ctrl-\, as it's difficult to hit accidentally.  In my .screenrc:

    escape \034\034

---

    [chromatic]

---

[[TomHeady]]

my .screenrc file:

    shell -$SHELL
    startup_message off
    defscrollback 1024

    hardstatus on
    hardstatus alwayslastline
    # show a status screen at the bottom of screen that shows the windows
    # open, the hostname of the box you are on, and the date/time
    hardstatus string "%{.bW}%-w%{.rW}%n %t%{-}%+w %=%{..G} %H %{..Y} %m/%d %C:%a "

    escape ^Za          # set escape key to CTRL-z

    autodetach on       #aut detach instead of terminating
    vbell on            #use a visual bell instead of audible

    sorendition rw 

---

[[AdamMonsen]]

    # .screenrc
    # $Id: ScreenRCFile,v 1.2 2008/01/12 17:01:57 apache Exp apache $

    defscrollback 5000

    # let scrollbars work in xterm, gnome-terminal
    # (from http://www4.informatik.uni-erlangen.de/~jnweiger/screen-faq.html)
    termcapinfo xterm ti@:te@

    # add some cool stuff from the GNU screen-users mailing list
    # see http://lists.gnu.org/archive/html/screen-users/2004-08/msg00005.html

    # set the last line of the terminal to have a useful, pretty status line kinda
    # like the GNOME panel
    caption always "%{wk}%?%-Lw%?%{bw}%n*%f %t%?(%u)%?%{wk}%?%+Lw %= %{mk}@%H %{yk}%D %{ck}%M%{wk} %{ck}%d %{gk}%c"

    # Enter copy mode (INSERT) PgUp/PgDn to move
    bindkey -k kI copy

    # Paste copy buffer (ESC-INSERT)
    bindkey "^[^[[2~" paste .

    # Use ALT-; and ALT-' to switch to previous and next window, respectively
    bindkey "^[;" prev
    bindkey "^['" next

    # detach on hangup
    autodetach on

    # don't display the copyright page
    startup_message off

    # emulate .logout message
    pow_detach_msg "Screen session of $LOGNAME $:cr:$:nl:ended."
