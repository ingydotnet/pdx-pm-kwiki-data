## Upgrading a Kwiki Site

After installing the new CGI::Kwiki module, just cd into the old Kwiki directory and reinstall with:

    kwiki-install --upgrade

This will upgrade everything except the config file and the changed pages. Other upgrade options are:

    --reinstall  - Upgrade everything including config file.
    --config     - Upgrade config file. You will lose local settings!
    --scripts    - Upgrade cgi scripts.
    --pages      - Upgrade default kwiki pages unless changed by a user.
    --template   - Upgrade templates.
    --javascript - Upgrade javascript.
    --style      - Upgrade css stylesheets.
