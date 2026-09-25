#HTTP Exchange Analysis

**Website:** https://www.wowhead.com
**Browser:** Google Chrome(Devtools Network)

##Recorded HTTP Requests

###Request 1. Initial Page Load
**Reuqest Method:** 'GET'
**Request URL:** 'https://www.wowhead.com/'
**Status Code:** '200 OK'
**Response Headers:**
	* 'content-type: text/html; charset=UTF-8'
	* 'server: nginx'


###Request 2: op.js
**Request Method:** 'GET'
**Request URL:** 'https://tagan.adlightning.com/zam/op.js
**Status Code:** '200 OK'
**Response Headers:**
	* 'content-type: application/javascript'
	* 'cache-control: max-age=3600'

###Request 3: Universal.css
**Request Method:** 'GET'
**Request URL:** 'https://wow.zamimg.com/css/standard/universal.css
**Status Code:** '200 OK (Fromt memory cache)'
**Response Headers:**
	*'content-type: text/css'
	* 'age: 19071'

##Analysis

In my analysis of opening a website I visit often for my video game interests of (wowhead.com) I noticed the slowest
request was a file.mp4, which loaded at 17.44s.  It has a status code of 206 partial content. I'm assuming it took the longest because
multimedia is often bigger to load in size compared to smaller aspects of a webpage.
The most suprising finding was seeing how fast the requests piled in when I loaded the website, and how frequent and
often they continued coming in, even while just sitting on the website not doing anything.  I assume this is from the
media and ads on the website.
