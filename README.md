# maxupdate-libraries

Several applications, including Max!Buddy and MaxBackup rely on files that used to be provided on manufactures website (`http://www.max.eq-3.de/maxupdate/lib/`).
Sadly, these file are no longer available. I've tried to search the webarchive, caches and local copies and I've managed to get the important files. I've saved them to this repository. I've also modified some of them so that they don't contain URLs to the original website, but to this repository.

`maxupdate/lib/MaxEssentialsBackend-1.4.1.jar` (source: MAXBuddy-r9.16.2-win-portable)
`maxupdate/lib/MaxLocalBackend-1.4.1.jar` (source: MAXBuddy-r9.16.2-win-portable)
`links-916.xml` (the original is kept in file `links-916_original.xml`, source: MAXBuddy-r9.16.2-win-portable)
`maxupdate/digest.txt` (the original is kept in file `digest_original.txt`, [source](https://web.archive.org/web/20130103235227/http://www.max-portal.elv.de:80/maxupdate/digest.txt))

Depending on your usecase, you might have to host them locally, because some implementations don't support HTTPS and Github is HTTPS only.
If you host locally, you can for example write the following lines to `hosts` file to redirect the domains to your localhost.

```
127.0.0.1 www.max.eq-3.de
127.0.0.1 www.max-portal.elv.de
```

Some versions use other files, for example `links-914.xml`, `maxupdate/lib/MaxEssentialsBackend-1.3.7.jar`, `maxupdate/lib/MaxLocalBackend-1.3.7.jar`.
I've not been able to source those, but I've found that if you just rename their newer counterparts, than it works.
