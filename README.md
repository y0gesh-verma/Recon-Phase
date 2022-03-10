# Recon Phase
Reconnaissance is the first step of a Penetration Testing service engagement regardless if you are verifying known information or seeking new intelligence on a target.</br>	

The term Reconnaissance by definition comes from the military warfare strategy of exploring beyond the area occupied by friendly forces to gain information about the enemy for uture analysis or attack. Reconnaissance of computer systems is similar in nature, meaning typically a Penetration Tester or hacker will attempt to learn as much as possible about a target's environment and system traits prior to launching an attack. This is also known as establishing a Footprint of a target.



• Website information


			>	Employee details ( User Name / Email )
			>	Location details
			>	Addresses / Phone numbers
		
		
• Sitemap </br>		
A sitemap is a file where you provide information about the pages, videos, and other files on your site, and the relationships between them. Search engines like Google read this file to crawl your site more efficiently.</br>	
One by one visit the sitemap urls and see is there any sencetive information axsist or not. By using sitemap we know how many url's we visited or how many url's is remaining for visit. All website's not contains sitemap but Most of the website's contains sitemap. sitemap is placed For Search engin's .
	
	Types of sitemap:
	
	
			>	user sitemap		-	sitemap.html	-	user index
			>	Search engin sitemap	-	sitemap.xml	-	Search engin index
		
		
User sitemap is available on the footer of the website, make for users. (example:- https://example.com  )</br>	
Search ingen sitemap is made for search engines. This is the search engine index. (example:- https://www.example.com/sitemap.xml</br>
	
If sitemap is not available on the website then we will generate the sitemap. By Using this website (https://www.xml-sitemaps.com/) we can create sitemap.html and sitemap.xml file for any website. 		
	
sitemap.xml vulnerability hackerone:-  https://hackerone.com/reports/318603
	
• robots.txt </br>	
In robots.txt file here is some links which is not for users, as well as not visible for users and which is not allowd to index by search engine.	


			>	robots.txt		-		Disallow for any user agent and google / search engine 
	
	
• By this url https://www.convertcsv.com/url-extractor.htm extract all anker tag of the perticular page. we get all anker tag links by this.
	(download the output in csv or excel bot format.)	
	
	
			>	https://www.convertcsv.com/url-extractor.htm 
	
	
• screamingfrog</br>	
SEO Spider, do indexing like search engines, this goes to website and how many contents or pages are there and generate index then provide us output.  the functonality of this tool is goes one link to second link and second link to third link this is called spider. user friendly output. internal links and external links all link is shown in output
	
	
			>	seo spider	-	https://www.screamingfrog.co.uk/seo-spider/
			
			
• Mirror the website </br>	
Mirror the website For analysing web pages source code.
	
	
			>	Locally mirroring the website		-		Read Source Code
			
				 wget
				# wget -m https://www.armourinfosec.com
				
• HTTrack</br>	
HTTrack availabe on both windows or kali linux (GUI or CLI both) (alternative option for Mirroring)				
	
	
			>	# httrack https://www.armourinfosec.com
			
			
• this file tell about technology use.	


			>  	readme.html or readme.txt
			
			
• what technology are used for website some information may be	(also see this files and folder ).


			>	crossdomain.xml
			>	clientaccesspolicy.xml	
			>	license.txt
			>	.well-known/
			
			
• Waybackmachine</br>	
Previous content identify. May be we get some sensitive information  and end points like user name and all those thing. 
archive is a collection of usefull information or historical documents or records providing information about a place, institution, or group of people. 
For this we use two resources:
	
	
			>	Waybackmachine		-		https://archive.org 
			>	archive.today		-		https://archive.ph/
			
			
https://archive.org  take a snapshot of website. save website look and feel frontend html, css, javascript and store. and old resource also available. websites, books, software and so on. to see old version of website go to https://archive.org  waybackmachine enter the url https://armourinfosec.com Click on Brows History.
	
we can archive website content by using https://archive.ph/	
go to https://archive.ph/ here (My url is alive and I want to archive its content) enter the url of the website which we want to archive https://www.armourinfosec.com the click to save.
	
to see old version of website go to https://archive.ph/  here (I want to search the archive for saved snapshots) enter the url of the website https://armourinfosec.com then click to search.

• waybackurls</br>	
It is use for find out end points, end point it means url. waybackurls give us numbers of url. All those number of Resources that have now been removed, The page that used to be before  that is now deleted.we can see that pages by using waybackmachine but here we want the urls of the deleted pages. for web pages content we use waybackmachine and for page urls we will use Waybackurls. </br>	
	
For waybackurls we must have install golang.

			>		# apt install golang
			
create a directory in which we will clone the git reposetory.
			
			>		# mkdir -p /root/go/bin
			>		# cd /root/go/bin
			
Now clone the git reposetory by using go command.

			>		# go get github.com/tomnomnom/waybackurls

Now we have  waybackurls binary file. we will put this binary file to /usr/local/bin/ for run this binary from anywhere. 

			>		# cp -v /root/go/bin/waybackurls /usr/local/bin/ 
			>		# waybackurls --help
			
The waybackurls command is working. Now we give a url to waybackurls command.

			>		#waybackurls https://www.armourinfosec.com
			
Now we have numbers of previous waybackurls. May be this url's or numbers of resource or link also exist today, which is removed from the website.
By using waybackurls we get the end points or link or url of the target.</br>	


• On what technology is the website built?

			>	readme.html
			>	readme.txt
			>	licence.txt
			>	feed (RSS feed)
			
we get some information in these files which through we can ensure that on what technology is the website built.</br>	

Other than this, there are some other online resources that we use.</br>	


			like:
			
			> 	https://builtwith.com/
			>	https://www.wappalyzer.com/


builtwith and wappalyzer analyze source code of the frontend language of the website, and tell us that on what technology is the website built or what methology is use.</br>	
builtwith and wappalyzer addon also available.</br>	
Verifying information from more than one place is the right approach.</br>	

• siteinfo</br>	
Website Traffic, Statistics, and Analytics related information
		
			>	https://www.alexa.com/siteinfo

we get site traffic, global rank related information and so on.







