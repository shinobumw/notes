# rsync

## Backup

`/etc/cron.daily/backup`
```bash
#!/bin/bash

rsync -a --delete --quiet /folder/to/backup /location/of/backup

if [ $? != "0" ] ; then
    echo "rsync backup failed."
else
    tar czf /var/backup/home-`date +%Y%m%d`.tar.gz /folder/to/backup /location/of/backup
fi
```

## Reference

- [rsync - ArchWiki](https://wiki.archlinux.org/index.php/rsync)
- [Trying to create a cron to Rsync then tar the folder](https://unix.stackexchange.com/questions/37912/trying-to-create-a-cron-to-rsync-then-tar-the-folder)