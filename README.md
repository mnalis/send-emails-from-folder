# send-emails-from-folder
sends all *.eml files in folder via /usr/sbin/sendmail wrapper
optionally archiving (or removing) sent files.

Recepients are determined automatically from "To:" lines in .eml files.

you should run it from cron job via line like:
<pre>
# m h   dom mon dow user  command
*/15 *    *  *   *   user  /usr/local/bin/send-emails-from-folder sender@example.org /home/user/emails /home/user/archive
</pre>
