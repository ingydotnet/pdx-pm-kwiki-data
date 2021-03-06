[[JoshHeumann]]

    alias brc='vim ~/.bashrc'
    alias sbrc='source ~/.bashrc'
    alias vrc='vim ~/.vimrc'

    alias psa='ps auwx | grep'
    alias psaw='ps auwwx | grep'

    alias pd='perldoc'
    alias pf='perldoc -f'

    alias svu='svn up'
    alias svs='svn status'
    alias svsu='svn status -u | grep -v swp'

    alias lsf='ls -p | grep -v /'
    alias lsd='ls -p | grep /'

---

[[EricWilhelm]]

    # pretty colors (may need "export PS1...")
    PS1='\n\[\033[45m\]\u@\h: \[\033[49m\]\[\033[31m\]\w\n\[\033[0m\]\[\033[45m\]#\[\033[0m\]\t \[\033[45m\]$\[\033[0m\] '
    # and red for root
    PS1='\n\[\033[41m\]\u@\h: \[\033[49m\]\[\033[31m\]\w\n\[\033[0m\]\[\033[41m\]#\[\033[0m\]\t \[\033[41m\]#\[\033[0m\] '

---

[[TomHeady]]

    # exclude *.svn\* files from all grep searches
    export GREP_OPTIONS="--exclude=\\*.svn\\*"

    # if there is a detached screen session, reattach
    # otherwise, create one
    alias screen='screen -d -R'

    # auto launch screen, unless we are already in a screen session
    # or we are in a dumb terminal.
    # also, put which screen window at the beginning of the
    # prompt: [0] or [1] ...
    case $TERM in
    screen*)
        PROMPT_COMMAND='echo -n [$WINDOW]\ '
        ;;
    dumb*)
        ;;
    *)
        screen
        ;;
    esac

---

[[chromatic]]
The most useful tip is:

    source ~/.aliases

That file contains the alias:

    alias realias='chmod u+w ~/.aliases; $EDITOR ~/.aliases; source ~/.aliases; chmod -w ~/.aliases'

From the command line, type realias to open your favorite editor on your aliases file, add a new alias, and reload your aliases all from the same terminal.  Don't waste any more time closing terminals and opening them again to get your latest aliases.

Now put everything that annoys you in your alias file.  Some good ones are:

    alias testcover='cover -delete; ./Build testcover; cover'
    alias newsvn='cd ~/dev/repos; svnadmin create --fs-type fsfs'
    alias um="uptime && free -m"
    alias makepugs='PARROT_PATH="/home/chromatic/dev/parrot" PUGS_EMBED="perl5 parrot" perl Makefile.PL'
    alias spp='svk pull; svk push'
    alias stunnel='ssh snafu -L2500:snafu:25'

---

[[AdamMonsen]]

    # only do the following during an interactive prompt
    if [ "$PS1" ]
    then
      alias egrep='egrep --color=auto'
      alias f='find . | grep'
      alias grep='grep --color=auto'
      alias indent='indent -bli0 -nut'
      alias ls='ls -F --col'
      alias p='ps auxwww | grep'
      # this is DEFINITELY my most often-used command
      alias s='cd ..'
      alias r='rpm -qa | grep'
      alias packup='/bin/tar -czvf'
      alias unpack='/bin/tar -xzvpf'
      alias contents='/bin/tar -tzf'
      # make a temp dir, then immediately cd into it
      alias mktd='tdir=`mktemp -d` && cd $tdir'

      # list contents right after changing directories
      cd() {
        if [ "$1" ]
        then builtin cd "$1" && ls
        else builtin cd && ls
        fi
      }

      # make a directory, then immediately cd into it
      mkcd() {
        if [ "$1" ]
        then mkdir -p "$1" && cd "$1"
        fi
      }

      # correct minor errors in 'cd' commands
      shopt -s cdspell
      # good for double-checking history substitutions
      shopt -s histverify

      # If this is an xterm set the title to user@host:dir
      case "$TERM" in
      xterm*|rxvt*)
          PROMPT_COMMAND='echo -ne "\033]0;${USER}@${HOSTNAME}: ${PWD/$HOME/~}\007"'
          ;;
      *)
          ;;
      esac

      # ~ the Emotiprompt(TM) ~
      # idea came from: http://linuxgazette.net/122/lg_tips.html#tips.1
      smiley() {
         err=$?
         if [ $err == 0 ]
         then echo ':)'
         else echo ":( $err"
         fi
      }
      PS1="\$(smiley) [\u@\h \W]\\$ "
    fi
