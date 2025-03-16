# **⚠️Vulnerability Assessment  for *[gascgobi.ac.in](www.gascgobi.ac.in)*** 


### **<span style="color:coral">SSL Vulnerability Scan Results</span>**  

**<span style="color:skyblue">SSL/TLS Protocols</span>**

- SSLv2: disabled
- SSLv3: disabled
- TLSv1.0: disabled
- TLSv1.1: disabled
- **`TLSv1.2: enabled`**
- TLSv1.3: disabled

**<span style="color:coral">Heartbleed: </span>`Not vulnerable to Heartbleed.`**

**<span style="color:skyblue">Encryption Strength</span>**
- Preferred Cipher: ECDHE-RSA-AES256-GCM-SHA384 (256 bits)
- Other Accepted Ciphers:
    - ECDHE-RSA-AES128-GCM-SHA256 (128 bits)
    - Various AES configurations

**<span style="color:skyblue">Certificate Information</span>**
- Issuer: Starfield Secure Certificate Authority - G2
- Validity: From Aug 30, 2024 to Aug 31, 2025
- Subject: gascgobi.ac.in
### **<span style="color:coral">Nmap Scan Results:</span>**
**<span style="color:skyblue">Open Ports:</span>**

- 21 (FTP): Microsoft ftpd
- 80 (HTTP): Microsoft HTTPAPI httpd 2.0
    - Title: Gobi Arts & Science College, Gobichettipalayam
    - HTTP Methods: Potentially risky methods (e.g., TRACE)
- 443 (HTTPS): Microsoft HTTPAPI httpd 2.0
    - Used for secure HTTP communications
    - Potentially risky HTTP methods (e.g., TRACE)
- 8443 (HTTPS, Plesk): Microsoft IIS httpd 10.0
    - Title: Plesk Obsidian
    - HTTP Methods: Contains an entry in robots.txt: 1 disallowed entry /

# **<span style="color:red">Summary of Vulnerabilities:</span>**

>### **Potentially Risky HTTP Methods:**
> The server allows the TRACE method which can be exploited in certain attacks such as Cross-Site Tracing (XST).

>### **Service Versions:**
> Using older versions of Microsoft IIS can expose the site to known vulnerabilities.

>### **Certificate Validity:**
> Ensure timely renewal of the SSL certificate before its expiration on Aug 31, 2025.



### **Recommendations:**
▪ Disable weak and unnecessary HTTP methods, particularly TRACE.<br>
▪ Regularly update the web server software to mitigate any known vulnerabilities.<br>
▪ Ensure that the server's configuration for SSL/TLS is reviewed periodically to enhance security.<br>
▪ If you need further assistance or detailed analysis, feel free to ask!
