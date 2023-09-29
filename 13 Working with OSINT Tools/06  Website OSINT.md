Will use Wappalyer  but will not go into the detail as we have already install it during our PEH course.

If u recall we have used many different sites for website osint and use WHOis feature in that and we have a similar tool inbuilt as well
![[Pasted image 20230926142047.png]]

But before installing all the tools that are listed below we have to do little tweaks in our bash.rc file 
```
nano ~/.bashrc 

export GOPATH=$HOME/go 
export GOROOT=/usr/lib/go 
export PATH=$PATH:$GOROOT/bin:$GOPATH/bin

source ~/.bashrc
```



![[Pasted image 20230926144749.png]]
Subfinder - [https://github.com/projectdiscovery/subfinder](https://github.com/projectdiscovery/subfinder)

```
go install -v github.com/projectdiscovery/subfinder/v2/cmd/subfinder@latest
```



![[Pasted image 20230926144838.png]]
Assetfinder - [https://github.com/tomnomnom/assetfinder](https://github.com/tomnomnom/assetfinder)

```
go install -v github.com/tomnomnom/assetfinder
```


![[Pasted image 20230926145127.png]]

httprobe - [https://github.com/tomnomnom/httprobe](https://github.com/tomnomnom/httprobe)
```
go install github.com/tomnomnom/httprobe@latest
```



Amass - [https://github.com/OWASP/Amass](https://github.com/OWASP/Amass)

```
go install -v github.com/owasp-amass/amass/v4/...@master
```


Will simply strip off the extra data before passing it to the gowitness
![[Pasted image 20230926145404.png]]

GoWitness - [https://github.com/sensepost/gowitness/wiki/Installation](https://github.com/sensepost/gowitness/wiki/Installation)
Recommend to install goWitness from pimpykali 
![[Pasted image 20230926145638.png]]

![[Pasted image 20230926145926.png]]

