Here is a summary report of the network activity captured in the "wireshark\_capture.pcapng" file.

### **General Information**

The packet capture was taken on a 64-bit Windows 11 machine with an Intel(R) Core(TM) i5-8350U CPU. The capture tool used was Dumpcap (Wireshark) version 4.4.5.

### **Network Activity**

The capture shows network traffic related to web browsing and background services. The primary web servers and services contacted include:

* **Google-related services**: www.google.com, play.google.com, beacons.gcp.gvt2.com, clients4.google.com, www.google-analytics.com, and safebrowsing.google.com. This suggests a user was browsing the web and other Google services were running in the background.  
* **Networking and Education**: www.netacad.com and web.simmons.edu were accessed. Specifically, a request was made to  
   http://web.simmons.edu/\~grovesd/comm244/notes/week2/links 1. The content of this page discusses dissecting URLs and different types of links (absolute and relative URLs). This indicates the user was likely viewing a webpage related to a networking or web development class.  
* **Content Delivery Networks (CDNs)**: The capture also shows connections to several CDNs, including cdnjs.cloudflare.com, d1h6v4iwmfkzng.cloudfront.net, eum-appdynamics.com, use.fontawesome.com, and fonts.gstatic.com. These are typically used to load web assets such as CSS, JavaScript, and fonts, which is consistent with web browsing activity.  
* **Certificate Services**: The capture contains requests to certificate-related domains such as identrust.com and lencr.org. This is normal activity for establishing secure HTTPS connections. A certificate for  
   **DigiCert Global Root G2** was exchanged 22222, along with another one for a certificate from  
* **R3** 333333333.  
* **Other Web Servers**: A connection was made to neverssl.com, which returned an HTML page 4. This is a common test site for checking if a network has a captive portal that redirects all web traffic to a login page.

### **Observed Protocols**

The capture primarily contains unparsed binary data, but based on the domains and content types, the following protocols and services were likely used:

* **DNS (Domain Name System)**: DNS queries were made for most of the domains mentioned above, including play.google.com, cdn.appdynamics.com, freshsilverbrightplan.neverssl.com, and x1.i.lencr.org 555555555555555555555555555555555555.  
* **HTTP/HTTPS**: Connections were established to various web servers. A few of the unparsed packets appear to be HTTP requests and responses 666666666.  
* **TLS (Transport Layer Security)**: The presence of certificate traffic to domains like identrust.com and lencr.org suggests that many of the connections were secured using TLS 777777777.

### **Specific File Requests**

The capture contains evidence of requests for several file types:

* **HTML**: http://web.simmons.edu/\~grovesd/comm244/notes/week2/links was requested, and the response was an HTML document 8.  
* **CSS**: A CSS file, notes.css, was requested from the same Simmons server9.  
* **JavaScript**: A JavaScript file, prism.js, was requested from the Simmons server 10.  
* **Images**: Several image files, including url-parts.jpg and rb-site-structure.png, were requested from the Simmons server 11111111.  
* **Icon**: A request for favicon.ico was made 12121212.

The requests for these various files are consistent with a user loading a web page that includes CSS styling, JavaScript functionality, and image assets.

