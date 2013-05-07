munin-tenki-jp
==============
Add entry to /etc/crontab, and specify URL to check the area you are interested in.

> `45  * * * * nobody  /path/to/atomtemp cron http://tenki.jp/component/static_api/rss/amedas/point-XXX.xml`

Symlink munin plugin file.

`symlink -s /path/to/atomtemp /path/to/munin/plugins/dir/`

Setup munin environment `wgetcmd` and `outfile` for customize.
