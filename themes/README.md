# quickbox_themes
All additional themes for the QuickBox Dashboard are housed here... nice and tidy like! Want to make your own? Fork and submit!

https://www.dropbox.com/s/300201cvzlilz3z/QuickBox%20-%20Smoked%20preview.gif

##Feel free to discuss... :stuck_out_tongue_winking_eye:

### Want to install the QuickBox Smoked Theme?

##Updated Theme Install Method

Thanks [@Reynald](https://plaza.quickbox.io/u/reynald) for confirming this method to be working!

You can add a **.smoked.lock** which the updater (if it dicovers the theme lock) will port in the needed theme assets. You can add this lock by doing
```
printf "" > /srv/rutorrent/home/db/.smoked.lock
```

If you want the default theme back then do:
```
rm -f /srv/rutorrent/home/db/.smoked.lock
```
Then add the 'defaulted' lock file and run the update.
```
printf "" > /srv/rutorrent/home/db/.defaulted.lock
```

Perform `box upgrade` to set the new/previous theme.


##The [@Reynald](https://plaza.quickbox.io/u/reynald) method - simple one liner!

Select **smoked**:
```
rm -f /srv/rutorrent/home/db/.defaulted.lock && printf "" > /srv/rutorrent/home/db/.smoked.lock && box upgrade
```

Select **defaulted**:
```
rm -f /srv/rutorrent/home/db/.smoked.lock && printf "" > /srv/rutorrent/home/db/.defaulted.lock && box upgrade
```

>These have been built in for an addition to the dashboard to swap themes... (that's coming soon)
