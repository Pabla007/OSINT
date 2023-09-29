Download the torrent File:
```
magnet:?xt=urn:btih:7ffbcd8cee06aba2ce6561688cf68ce2addca0a3&dn=BreachCompilation&tr=udp%3A%2F%2Ftracker.openbittorrent.com%3A80&tr=udp%3A%2F%2Ftracker.leechers-paradise.org%3A6969&tr=udp%3A%2F%2Ftracker.coppersurfer.tk%3A6969&tr=udp%3A%2F%2Fglotorrents.pw%3A6969&tr=udp%3A%2F%2Ftracker.opentrackr.org%3A1337
```

We don't have dehashed or any subscription this will help as at some point of time this data was gone public. It's always good to have something that nothing.

Breach Parse 
```
https://github.com/hmaverickadams/breach-parse
```


This has has to be done locally let's see how to do that
If you search to much than it will trigger sometime these Shadow ban on you as a result that will stops showing results for you.

```
theHarvester -d tcm-sec.com -b all
we can all set the limit from 500 which is default to 1000
theHarvester -d tcm-sec.com -b all -l 1000 
```

```
theHarvester -d tesla.com -b google -l 500 
./breach-parse.sh @tesla.com tesla.txt 
h8mail -t shark@tesla.com -bc "/opt/breach-parse/BreachCompilation/" -sk
```
When trying to use Google it throws some kind of error
![[Pasted image 20230926123354.png]]

![[Pasted image 20230926123441.png]]

So if got the email address and what to find the password related to it. That's where the breached parse will come in Handy

There's a great tool called H8mail  it has a lot of sites that shows breached password but u need to have API access for that which i don't have as of now.

https://github.com/khast3x/h8mail
![[Pasted image 20230926124027.png]]

```
h8mail -t shark@tesla.com
```
![[Pasted image 20230926124140.png]]

But we know that this email is compromised and still getting not compromised as we don't have access to the above site aka API access. So will depend on the breach parse for now.

cat tesla-master.txt | grep shark
./breach-parse.sh shark tesla.txt

