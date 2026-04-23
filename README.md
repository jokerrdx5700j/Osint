# Complete OSINT Guide: Core Basics + 100 Advanced Techniques + 100 Passive Recon + 100 Active Recon

## **SECTION 1: OSINT FUNDAMENTALS**

---

## **What is OSINT?**

**OSINT (Open Source Intelligence)** is gathering intelligence from **publicly available sources**. These are sources legally accessible to anyone:

- Websites (news, social media, blogs)
- Public records (government databases, registries)
- Forums and message boards
- Images and videos
- Published research and reports

---

## **PCPAD Methodology**

PCPAD is the foundational 5-step framework for OSINT investigations:

| Step | What It Means |
|------|--------------|
| **P - Preparation** | Define what you're looking for and your limits |
| **C - Collection** | Gather data from sources |
| **P - Processing** | Organize and clean the data |
| **A - Analysis** | Find patterns and meaning in the data |
| **D - Dissemination** | Share your findings |

---

## **Passive Reconnaissance (Stealth Gathering)**

**Definition:** Collect information WITHOUT directly contacting the target. They won't know you're looking.

**How it works:**
- No interaction with the target
- Low risk of being detected
- Data may not be current

**Basic Examples:**
- Google searching public profiles
- Looking up WHOIS information on domains
- Checking DNS records via third-party websites
- Reading news articles about a person/company
- Browsing someone's public social media

**Why it matters:** You gather info without alerting anyone.

---

## **Active Reconnaissance (Direct Probing)**

**Definition:** Directly interact with the target. They may know you're investigating.

**How it works:**
- Direct contact with the target
- High risk of being detected
- Data is current and real

**Basic Examples:**
- Scanning a website with tools like Nmap
- Searching Shodan to find devices
- Sending emails to see responses
- Probing web applications for information
- Directly querying target systems

**Why it matters:** You get fresh, specific information but risk alerting the target.

---

## **The Core Difference**

| Aspect | Passive | Active |
|--------|---------|--------|
| **Contact** | None | Direct |
| **Detection Risk** | Low | High |
| **Data Type** | Public/Archived | Real-time |
| **Example** | Reading a blog post | Scanning a server |

---

## **Most Basic OSINT Workflow**

1. **Start with Passive** → Search public info (Google, social media, WHOIS)
2. **Analyze What You Find** → Look for patterns and connections
3. **Go Deeper with Passive** → Check archives, old pages, leaked databases
4. **Only Then Go Active** → If needed, directly probe the target
5. **Compile Results** → Document everything you found

---

## **Core OSINT Techniques (The Essentials)**

### **Search Engines**
- Use Google with special commands (site:, filetype:, intitle:)
- Bing, DuckDuckGo also have advanced search

### **Social Media**
- Look at public profiles on Facebook, Twitter, Instagram
- Find email addresses and phone numbers
- Track connections between people

### **Public Records**
- WHOIS lookups (who owns a domain)
- DNS records (what servers run a domain)
- Government records, business registrations

### **Images & Metadata**
- Reverse image search (TinEye, Google Images)
- Extract EXIF data (location, camera info from photos)
- Geolocation from photos

### **People Searches**
- Email lookup (Hunter.io)
- Username searches (KnowEm, Namechk)
- Phone number lookup
- Data breach searches (HaveIBeenPwned)

### **Domain & Website Info**
- WHOIS history
- DNS records
- Website change tracking
- SSL certificate info

---

## **Most Basic Tools**

These are the **core tools** every OSINT person should know:

1. **Google** - Search engine mastery
2. **WHOIS lookup sites** - Find domain owners
3. **Wayback Machine** - See old versions of websites
4. **Hunter.io** - Find email addresses
5. **Maltego** - Map relationships between data
6. **Shodan** - Search internet-connected devices
7. **TheHarvester** - Gather emails and subdomains
8. **TinEye** - Reverse image search
9. **HaveIBeenPwned** - Check leaked passwords
10. **Spiderfoot** - Automated reconnaissance

---

## **The Golden Rule of OSINT**

✅ **Start Passive, Stay Legal, Document Everything**

- Gather as much as possible without contacting the target
- Only use publicly available information
- Keep records of what you found and where from
- Respect privacy laws and regulations

---

## **Why OSINT Matters**

- **Security Teams** use it to find vulnerabilities before attackers
- **Journalists** use it to verify stories
- **Law Enforcement** uses it to investigate crimes
- **Businesses** use it for competitive intelligence
- **Individuals** use it for personal security

---

**The absolute core:** OSINT is finding public information efficiently, organizing it, understanding what it means, and sharing those insights—without breaking laws or alerting the target.

---

---

# SECTION 2: 100+ ADVANCED OSINT TECHNIQUES & METHODS

---

## **1. Search Engine Mastery (7 techniques)**

1. Advanced Google Dorking (site:, intitle:, filetype:, inurl:, etc.)
2. Bing Advanced Search operators
3. Yandex Reverse Search
4. DuckDuckGo search modifiers
5. Dark web search engines (Ahmia via TOR)
6. Metadata extraction via search (filetype:pdf site:gov)
7. Cached content exploration (Wayback Machine, Google cache)

---

## **2. Social Media Intelligence - SOCMINT (10 techniques)**

8. Facebook Graph Search and legacy API extraction
9. Twitter/X API scraping and archive searches
10. LinkedIn Sales Navigator filters and profile mapping
11. Instagram account & hashtag mapping
12. Reddit topic tracking (Pushshift, SubredditStats)
13. TikTok profile mapping and geolocation
14. Snapchat Snap Map exploration
15. Telegram channel and group scraping
16. Mastodon and decentralized platform intelligence
17. Social connection analysis via Maltego

---

## **3. People & Entity Tracing (8 techniques)**

18. Email tracing (Hunter.io, EmailRep.io)
19. Username research (KnowEm, Namechk, WhatsMyName)
20. Phone number lookup (NumVerify, TrueCaller)
21. Address and property records search
22. Deep people search (Pipl, Spokeo, BeenVerified)
23. Data breach searching (HaveIBeenPwned, Dehashed)
24. Paste site monitoring (Pastebin, Ghostbin)
25. Public records analysis (corporate filings, SEC.gov)

---

## **4. Geolocation & GeoINT (8 techniques)**

26. Satellite imagery comparison (Google Earth Pro, Sentinel Hub)
27. EXIF data extraction (ExifTool)
28. Crowd-sourced map analysis (OpenStreetMap, Wikimapia)
29. Social media geo-tag correlation (Geofeedia)
30. Sun/shadow analysis for time/location confirmation (SunCalc)
31. Video geolocation with frame analysis
32. Terrain and structure identification (Terraserver)
33. Air traffic tracking (Flightradar24, ADS-B)

---

## **5. Image & Video Analysis (6 techniques)**

34. Reverse image search (Google, TinEye, Yandex)
35. Deepfake and manipulation detection (FotoForensics, InVID)
36. Hash-based similarity searching (PDQ, pHash)
37. Forensic watermark recovery
38. Crowd-sourced photo verification (Bellingcat)
39. Facial recognition tools (PimEyes, FindClone)

---

## **6. Domain & Network Investigation (7 techniques)**

40. WHOIS history and DNS discovery (DomainTools, SecurityTrails)
41. Subdomain enumeration (Amass, Sublist3r)
42. Passive DNS history lookup
43. SSL certificate transparency logs
44. Website change detection (Visualping, ChangeTower)
45. Hosting infrastructure tracking
46. IoT and host discovery (Censys, Shodan, ZoomEye)

---

## **7. Dark Web & Threat Monitoring (4 techniques)**

47. Onion site scraping and indexing (OnionSearch, Recon-ng)
48. Forum and marketplace monitoring
49. Surface and dark web credential leakage checks
50. Dark web reputation network mapping

---

## **8. Data Analytics & Visualization (5 techniques)**

51. Relationship pivoting in Maltego
52. Graph analysis (Linkurious, Gephi)
53. Email network visualization
54. Time-series analysis (Excel, Kibana, Splunk)
55. Cluster analysis from leaks/dumps

---

## **9. Automation & Scripting (5 techniques)**

56. Scrapy for large-scale web scraping
57. Python BeautifulSoup for targeted extraction
58. Selenium and Puppeteer for browser automation
59. OSINT automation with Spiderfoot
60. Google Dork automation scripts

---

## **10. Specialized Topic Research (6 techniques)**

61. Cryptocurrency transaction tracking (Blockchair, Etherscan)
62. Scam/phishing tracking (PhishTank, URLscan.io)
63. Shipping/logistics tracing (MarineTraffic, VesselFinder)
64. Vehicle identification via VIN lookup
65. News leak and publication monitoring
66. Financial due diligence (OpenCorporates, Orbis)

---

## **11. Email Investigation (3 techniques)**

67. Email header analysis for source location
68. Mail server and MX record verification
69. Alias finding with Hunter.io/LinkedIn

---

## **12. Code & Software OSINT (4 techniques)**

70. Code search on GitHub, GitLab
71. Exposed credential discovery in public repos
72. StackOverflow sensitive information monitoring
73. Dependency and package vulnerability enumeration

---

## **13. Password & Hash Analysis (2 techniques)**

74. Hash lookup (haveibeenpwned, hashdd.com)
75. Weak hash brute-forcing for leaks

---

## **14. Monitoring & Alerting (3 techniques)**

76. Google Alerts for names and entities
77. Content theft and infringement monitoring
78. RSS feed aggregation for news

---

## **15. Physical/Real-World OSINT (3 techniques)**

79. FOIA (Freedom of Information Act) requests
80. Utility and business license lookups
81. Patent and trademark searches

---

## **16. Advanced Techniques (4 techniques)**

82. OpSec: Anonymization (Tails, Qubes OS, VPN, TOR)
83. Digital evidence chain of custody
84. Complex network path tracing (BGPView, RIPEstat)
85. Cross-language OSINT (Baidu, Sogou, Cyrillic queries)

---

## **17. Essential OSINT Tools & Frameworks (15+ tools)**

86. **Maltego** - Entity resolution and relationship mapping
87. **Spiderfoot** - Automated reconnaissance framework
88. **Recon-ng** - Modular intelligence reconnaissance
89. **TheHarvester** - Email and host enumeration
90. **FOCA** - Metadata extraction tool
91. **Shodan** - Internet device search engine
92. **Censys** - Host and certificate search
93. **OSINT Framework** - Web-based tool repository
94. **Social-Searcher** - Multi-platform social search
95. **InVID** - Video verification suite
96. **IntelligenceX** - Archives and leak searches
97. **GreyNoise** - Internet noise context
98. **AIL Framework** - Automated leak analysis
99. **Bellingcat Toolkit** - Visual investigation tools
100. **Dehashed** - Data breach search platform

---

## **Key Principles for Effective OSINT**

✅ **Remain Anonymous** - Use VPNs, TOR, and operational security practices  
✅ **Document Everything** - Maintain chain of custody for findings  
✅ **Cross-Reference** - Verify information from multiple sources  
✅ **Stay Legal & Ethical** - Only use publicly available data; respect privacy laws  
✅ **Automate Strategically** - Use tools and scripts to scale investigations  
✅ **Think Visually** - Use mind maps and graphs to understand relationships  
✅ **Go Passive First** - Gather as much as possible before active techniques  

---

## **Summary: From Basic to Advanced**

**Basic Level:**
- Google Dorking
- Social media searching
- WHOIS lookups
- Reverse image search
- Email finding

**Intermediate Level:**
- Subdomain enumeration
- DNS analysis
- Data breach checking
- Website monitoring
- Metadata extraction

**Advanced Level:**
- Maltego relationship mapping
- Dark web monitoring
- Cryptocurrency tracking
- Facial recognition
- Automated frameworks (Spiderfoot, Recon-ng)
- Custom scripting and automation

---

---

# SECTION 3: 100 PASSIVE RECONNAISSANCE TECHNIQUES

---

## **PASSIVE RECON - NO DIRECT CONTACT, UNDETECTED**

### **Category 1: Search Engine & Web-Based Passive Recon (12 techniques)**

1. **Google Dorking for publicly exposed files** (site:, filetype:pdf, filetype:xls)
2. **Google Dorking for directory listings** (intitle:"index of" site:target.com)
3. **Google Dorking for admin pages** (intitle:"admin" OR intitle:"administrator" site:target.com)
4. **Google Dorking for sensitive documents** (filetype:doc OR filetype:docx "confidential")
5. **Google Dorking for login pages** (intitle:"login" OR inurl:"login" site:target.com)
6. **Google Dorking for backup files** (filetype:bak OR filetype:backup site:target.com)
7. **Bing Advanced Search operators** (ip:xxx.xxx.xxx.xxx, domain:target.com)
8. **DuckDuckGo site-specific searches** (site:target.com)
9. **Yandex search for non-indexed content** (searching Russian/Cyrillic sources)
10. **Cached content via Google Cache** (cache:target.com)
11. **Cached content via Bing Cache** (searching archived versions)
12. **Search operator combinations** (Multiple operators for refined searches)

---

### **Category 2: Wayback Machine & Web Archives (8 techniques)**

13. **Wayback Machine basic searches** (Finding historical snapshots of websites)
14. **Wayback Machine calendar view** (Identifying when changes were made)
15. **Wayback Machine robots.txt checking** (See what was hidden)
16. **Wayback Machine admin/config files** (Finding exposed configuration)
17. **Archive.org snapshots analysis** (Historical data extraction)
18. **Common Crawl dataset searches** (Large-scale web archive)
19. **Alternate Archive services** (archive.is, archive.ph)
20. **DNS history via Wayback** (Seeing historical DNS records)

---

### **Category 3: WHOIS & DNS Passive Lookups (10 techniques)**

21. **WHOIS domain registration lookup** (Who owns the domain)
22. **WHOIS registrar information** (Registration company details)
23. **WHOIS creation date analysis** (How old is the domain)
24. **WHOIS historical lookups** (DomainTools, SecurityTrails)
25. **WHOIS name server information** (DNS server providers)
26. **Reverse WHOIS lookups** (Find other domains by registrant)
27. **DNS A record lookup** (IP address of domain)
28. **DNS MX record lookup** (Mail server information)
29. **DNS TXT record lookup** (SPF, DKIM, DMARC records)
30. **DNS NS record lookup** (Nameserver information)

---

### **Category 4: IP Address & Geolocation Passive Recon (10 techniques)**

31. **IP geolocation lookup** (MaxMind, IPinfo.io, GeoIP databases)
32. **IP ASN (Autonomous System Number) lookup** (Network owner info)
33. **IP reverse DNS lookups** (What domain points to this IP)
34. **IP WHOIS information** (Regional Internet Registry data)
35. **IP historical data** (Past configurations of IPs)
36. **IP reputation checks** (GreyNoise, AbuseIPDB)
37. **IP blocking status** (Is IP blacklisted)
38. **IP range mapping** (Finding other IPs in same range)
39. **BGP route analysis** (Path to IP address)
40. **IP fingerprinting** (OS and service identification via passive means)

---

### **Category 5: Domain Intelligence & SSL Certificates (9 techniques)**

41. **SSL certificate analysis** (Certificate transparency logs)
42. **SSL certificate subject alternative names (SANs)** (Finding subdomains)
43. **SSL certificate history** (crt.sh, Censys)
44. **SSL certificate issuer analysis** (CA details)
45. **SSL certificate fingerprinting** (Identifying services)
46. **Subdomain discovery via certificates** (All subdomains with certs)
47. **Email addresses from certificates** (Admin contact info)
48. **Organization names from certificates** (Business entity research)
49. **Certificate validity period analysis** (When cert expires/renewed)

---

### **Category 6: Subdomain & DNS Enumeration (Passive) (8 techniques)**

50. **Passive subdomain enumeration via DNS** (SecurityTrails, VirusTotal)
51. **Subdomain discovery via certificate transparency** (crt.sh, Google)
52. **Subdomain discovery via DNS history** (Looking for old records)
53. **Subdomain discovery via search engines** (Bing, Google)
54. **Subdomain discovery via archives** (Wayback Machine)
55. **Passive DNS database queries** (SecurityTrails, Farsight)
56. **AXFR zone transfer (passive observation)** (Watching DNS responses)
57. **DNS forwarder identification** (Finding DNS providers)

---

### **Category 7: Social Media Intelligence (SOCMINT) - Passive (12 techniques)**

58. **Facebook profile search** (Public information only)
59. **Twitter/X advanced search** (User, keyword, date filters)
60. **LinkedIn profile analysis** (Public profile information)
61. **Instagram hashtag research** (Public posts, geolocation)
62. **Instagram bio analysis** (Username, location, website links)
63. **TikTok profile research** (Public videos, follower data)
64. **Reddit user history** (Public post analysis)
65. **Reddit subreddit analysis** (Community information)
66. **Telegram public channel analysis** (Open channel info)
67. **Discord server research** (Public server information)
68. **Snapchat username lookups** (Public profile data)
69. **BeReal post analysis** (Geolocation data from shared posts)

---

### **Category 8: Email & People Search - Passive (11 techniques)**

70. **Email finding via Hunter.io** (Email format discovery)
71. **Email finding via RocketReach** (Professional email databases)
72. **Email finding via Clearbit** (Company employee discovery)
73. **Email finding via Pipl** (Email & people data)
74. **Username research via KnowEm** (Username availability checks)
75. **Username research via Namechk** (Username existence checks)
76. **Username research via WhatsMyName** (Social media username search)
77. **Data breach searching via HaveIBeenPwned** (Leaked password checking)
78. **Data breach searching via Dehashed** (Breach database searches)
79. **Alias discovery via email variations** (firstname.lastname, first+last)
80. **Phone number OSINT** (TrueCaller, NumVerify reverse lookup)

---

### **Category 9: Image & Metadata Analysis - Passive (10 techniques)**

81. **Reverse image search via Google Images** (Finding where image appears)
82. **Reverse image search via TinEye** (Image source tracking)
83. **Reverse image search via Yandex** (Image location on internet)
84. **EXIF data extraction** (Location, camera, timestamp from photos)
85. **Metadata extraction from documents** (PDF, Office files via FOCA)
86. **Image geolocation via landmarks** (Visual analysis)
87. **Image geolocation via Google Maps** (Matching locations)
88. **Image geolocation via reverse streets view** (Street View analysis)
89. **Deepfake detection** (FotoForensics analysis)
90. **Image manipulation detection** (Forensic analysis tools)

---

### **Category 10: Company & Organization Research - Passive (10 techniques)**

91. **SEC filings research** (edgar.sec.gov for public companies)
92. **Corporate records lookup** (State business registries)
93. **Business license verification** (Local government databases)
94. **Patent & trademark searches** (USPTO, WIPO)
95. **News archive searches** (Company mentions in news)
96. **Press release databases** (PR Newswire, Business Wire)
97. **Company financials** (OpenCorporates, Crunchbase)
98. **Company website analysis** (Technology used, hosting provider)
99. **Company employee lists** (LinkedIn, Crunchbase)
100. **Company API documentation** (Publicly exposed API docs)

---

### **Tools Used for Passive Recon (Top 25):**

1. **Google** - Search engine
2. **Wayback Machine** (archive.org) - Web archive
3. **DomainTools** - WHOIS & DNS
4. **SecurityTrails** - DNS & subdomain
5. **Censys** - Certificate & host search
6. **VirusTotal** - Domain/IP analysis
7. **Hunter.io** - Email finding
8. **HaveIBeenPwned** - Breach checking
9. **Maltego** - Relationship mapping
10. **Shodan** - Device search (passive queries)
11. **Recon-ng** - Automated framework
12. **Spiderfoot** - Automated OSINT
13. **TheHarvester** - Email/subdomain enumeration
14. **crt.sh** - Certificate search
15. **Pipl** - People search
16. **Clearbit** - Email/company data
17. **Robtex** - DNS/IP research
18. **OSINT Framework** - Tool compilation
19. **IntelligenceX** - Search engine for leaks
20. **Dehashed** - Breach database
21. **TinEye** - Reverse image search
22. **FOCA** - Metadata extraction
23. **Exiftool** - Metadata analysis
24. **Social-Searcher** - Multi-platform search
25. **Bellingcat Toolkit** - Visual investigation

---

---

# SECTION 4: 100 ACTIVE RECONNAISSANCE TECHNIQUES

---

## **ACTIVE RECON - DIRECT INTERACTION, HIGH DETECTION RISK**

### **Category 1: Port Scanning & Service Enumeration (12 techniques)**

101. **Nmap basic port scan** (TCP SYN scan)
102. **Nmap UDP port scan** (UDP service discovery)
103. **Nmap service version detection** (-sV flag)
104. **Nmap OS detection** (-O flag)
105. **Nmap aggressive scanning** (-A flag with version, OS, scripts)
106. **Nmap script scanning** (NSE - Nmap Scripting Engine)
107. **Nmap vulnerability scanning** (vuln scripts)
108. **Masscan for rapid port scanning** (Fast port discovery)
109. **Zmap for internet-wide scanning** (Large-scale port scanning)
110. **Nessus vulnerability scanning** (Comprehensive vulnerability assessment)
111. **OpenVAS scanning** (Open-source vulnerability scanner)
112. **GVM (Greenbone Vulnerability Manager)** (Advanced scanning)

---

### **Category 2: Web Application Scanning (12 techniques)**

113. **Burp Suite web crawling** (Mapping application)
114. **Burp Suite active scanning** (Vulnerability detection)
115. **OWASP ZAP active scanning** (Web app vulnerability scanning)
116. **Nikto web server scanning** (Web server vulnerability check)
117. **WPScan for WordPress** (WordPress vulnerability scanning)
118. **Joomscan for Joomla** (Joomla vulnerability scanning)
119. **Drupal security scanning** (Drupal-specific checks)
120. **SQLmap SQL injection testing** (Database vulnerability testing)
121. **XSStrike XSS vulnerability testing** (Cross-site scripting check)
122. **WAFW00F WAF detection** (Web Application Firewall detection)
123. **Wappalyzer technology detection** (Identifying web technologies)
124. **Whatweb web scanner** (Web server identification)

---

### **Category 3: DNS Enumeration & Brute Force (10 techniques)**

125. **DNS zone transfer attempts** (AXFR requests)
126. **DNS brute force attacks** (Sublist3r, Amass active mode)
127. **DNS wildcard detection** (Testing for wildcard records)
128. **DNS NSEC walking** (DNS enumeration via NSEC records)
129. **DNS DIG queries** (Direct DNS queries)
130. **DNS NSLOOKUP queries** (Direct DNS interrogation)
131. **DNS reverse lookup brute force** (Reverse IP enumeration)
132. **DNS cache snooping** (DNS recursion abuse)
133. **Dnsrecon enumeration** (Multi-technique DNS tool)
134. **Fierce DNS enumeration** (Subdomain brute force)

---

### **Category 4: Network Mapping & Traceroute (8 techniques)**

135. **Traceroute to target** (Route path discovery)
136. **MTR (My Traceroute)** (Continuous route analysis)
137. **Ping sweeps** (Network host discovery)
138. **ARP scanning** (Local network host discovery)
139. **Network topology mapping** (Graphing network structure)
140. **BGP route analysis** (Tracing AS paths)
141. **Ping sweep with nmap** (Host discovery)
142. **ICMP echo requests** (Ping probes)

---

### **Category 5: Email & SMTP Enumeration (9 techniques)**

143. **SMTP user enumeration** (VRFY, EXPN commands)
144. **SMTP banner grabbing** (Server version identification)
145. **Email address verification** (Sending test emails)
146. **SMTP open relay testing** (Testing for relay vulnerabilities)
147. **Email header analysis** (Sending test messages)
148. **SPF record testing** (Mail authentication check)
149. **DKIM record testing** (Email signature verification)
150. **DMARC record testing** (Email policy checking)
151. **Haraka SMTP testing** (Direct SMTP probing)

---

### **Category 6: Directory & File Enumeration (11 techniques)**

152. **Directory brute force with Gobuster** (Common directory discovery)
153. **Directory enumeration with DirBuster** (Web directory scanning)
154. **Directory fuzzing with Fuff** (Fast fuzzing)
155. **Parameter fuzzing** (Testing unknown parameters)
156. **File enumeration with extensions** (.bak, .old, .tmp)
157. **Hidden file discovery** (.git, .svn folders)
158. **Backup file detection** (*.backup, *.sql)
159. **Configuration file discovery** (web.config, config.php)
160. **Source code exposure checks** (.env, .htaccess)
161. **API endpoint discovery** (/api/v1/, /api/v2/)
162. **Admin panel discovery** (/admin, /administrator)

---

### **Category 7: SSL/TLS Certificate Enumeration (8 techniques)**

163. **SSL certificate grabbing** (openssl s_client)
164. **Certificate validity checking** (Expiration date verification)
165. **Certificate chain analysis** (Full cert path examination)
166. **Cipher suite enumeration** (nmap, ssllabs)
167. **TLS version detection** (sslscan, testssl.sh)
168. **SSL/TLS vulnerability scanning** (Heartbleed, POODLE check)
169. **Certificate pinning detection** (Testing for pinning)
170. **Self-signed certificate identification** (Cert validation checks)

---

### **Category 8: Credential & Authentication Testing (10 techniques)**

171. **Default credential testing** (Common username/password pairs)
172. **Hydra brute force** (Multi-protocol password cracking)
173. **Medusa brute force** (Parallel password testing)
174. **Hashcat offline cracking** (Hash password cracking)
175. **John the Ripper** (Password cracking)
176. **Dictionary attacks** (Password list testing)
177. **Common password lists** (rockyou.txt, etc.)
178. **Credential spraying** (Multiple username/password attempts)
179. **OAuth token testing** (Bearer token analysis)
180. **API key discovery** (Scanning for exposed keys)

---

### **Category 9: Shodan & Internet Search Scanning (8 techniques)**

181. **Shodan API queries** (Device search)
182. **Shodan filters for vulnerabilities** (Vulnerable device search)
183. **Censys API queries** (Host & certificate search)
184. **ZoomEye scanning** (Chinese search engine for devices)
185. **Censys.io host probing** (Direct device enumeration)
186. **Internet-wide scanning** (Zmap for specific ports)
187. **IoT device discovery** (Searching for specific devices)
188. **Industrial control system scanning** (SCADA device detection)

---

### **Category 10: Virtual Host Enumeration (7 techniques)**

189. **Host header enumeration** (Testing different Host headers)
190. **Virtual host brute force** (Testing subdomain variations)
191. **SNI (Server Name Indication) enumeration** (TLS SNI probing)
192. **Reverse DNS lookups** (IP to hostname mapping)
193. **HTTP method testing** (OPTIONS, TRACE, etc.)
194. **Vhost scanning with Burp** (Web app virtual host discovery)
195. **Subdomain takeover scanning** (Finding vulnerable subdomains)

---

### **Category 11: Crawling & Spidering (7 techniques)**

196. **Burp Suite Spider** (Web application crawling)
197. **OWASP ZAP Spider** (Automated crawling)
198. **Wget recursive download** (Full site mirroring)
199. **Curl with follow redirects** (Manual page discovery)
200. **Python Scrapy** (Custom crawling scripts)
201. **Selenium browser automation** (JavaScript-enabled crawling)
202. **HTTrack website copying** (Full site mirroring)

---

### **Category 12: Database Scanning & Enumeration (8 techniques)**

203. **SQL injection vulnerability scanning** (SQLmap)
204. **Database version detection** (SQL injection for version)
205. **Database user enumeration** (SQL queries)
206. **Database table discovery** (Schema enumeration)
207. **Database credential testing** (Direct database connection)
208. **Oracle database scanning** (TNS listener probing)
209. **MongoDB unauth access testing** (Direct connection attempts)
210. **MySQL unauth access testing** (Default credential attempts)

---

### **Category 13: Firewall & IDS Evasion Testing (9 techniques)**

211. **Firewall rule testing** (Packet filtering checks)
212. **IDS evasion techniques** (Fragmentation, spoofing)
213. **WAF evasion methods** (Web Application Firewall bypass)
214. **Proxy detection** (Testing for proxy presence)
215. **Rate limiting detection** (Testing request thresholds)
216. **Bot detection evasion** (User-agent manipulation)
217. **Geo-blocking bypass** (VPN/proxy testing)
218. **DDoS protection detection** (Cloudflare, Akamai detection)
219. **Anti-bot detection** (CAPTCHA, JavaScript challenges)

---

### **Category 14: Exploit & Vulnerability Testing (9 techniques)**

220. **Known CVE testing** (Exploiting known vulnerabilities)
221. **Metasploit exploit modules** (Vulnerability exploitation)
222. **Custom exploit development** (Creating specific exploits)
223. **Buffer overflow testing** (Memory vulnerability checks)
224. **Format string attacks** (Printf vulnerability testing)
225. **Command injection testing** (OS command execution)
226. **Path traversal testing** (Directory traversal attacks)
227. **LDAP injection testing** (LDAP query manipulation)
228. **XXE (XML External Entity) testing** (XML vulnerability checks)

---

### **Category 15: Wireless & Network Protocol Scanning (8 techniques)**

229. **WiFi network scanning** (Aircrack-ng, kismet)
230. **WiFi WEP/WPA cracking** (Aircrack-ng)
231. **Bluetooth scanning** (Bluetoothctl, bleah)
232. **SNMP enumeration** (UDP port 161 probing)
233. **SNMP community string brute force** (Default credentials)
234. **NetBIOS enumeration** (nmblookup, nbtscan)
235. **SMB enumeration** (smbclient, enum4linux)
236. **LDAP enumeration** (ldapsearch, LdapMiner)

---

### **Category 16: API Endpoint Testing (9 techniques)**

237. **API endpoint discovery** (Burp Suite, Postman)
238. **API authentication testing** (Bearer token checks)
239. **API rate limiting bypass** (Header manipulation)
240. **API parameter fuzzing** (Testing various parameters)
241. **API response analysis** (Error message disclosure)
242. **GraphQL introspection** (Schema enumeration)
243. **REST API enumeration** (Endpoint discovery)
244. **API version detection** (Version identification)
245. **API documentation discovery** (/docs, /swagger, /graphql)

---

### **Category 17: Privilege Escalation Testing (7 techniques)**

246. **Local file inclusion (LFI) testing** (File read vulnerabilities)
247. **Remote file inclusion (RFI) testing** (Remote code execution)
248. **Sudo privilege testing** (Privilege escalation via sudo)
249. **SUID binary enumeration** (Special permission checks)
250. **Kernel vulnerability testing** (OS-level exploit testing)
251. **Misconfiguration exploitation** (Service privilege abuse)
252. **Weak password policy testing** (Password strength checks)

---

### **Category 18: Source Code & Configuration Exposure (8 techniques)**

253. **Git repository exposure** (.git folder access)
254. **SVN repository exposure** (.svn folder access)
255. **Backup file discovery** (web.config.bak, config.php.bak)
256. **Environment variable exposure** (.env files)
257. **Private key discovery** (SSH keys, API keys)
258. **Hardcoded credentials discovery** (Credentials in code)
259. **Build file analysis** (pom.xml, package.json, Dockerfile)
260. **Docker container enumeration** (Image scanning)

---

### **Category 19: Client-Side Vulnerability Testing (7 techniques)**

261. **Reflected XSS testing** (Cookie/session stealing)
262. **Stored XSS testing** (Persistent script injection)
263. **DOM-based XSS testing** (Client-side script manipulation)
264. **CSRF testing** (Cross-site request forgery)
265. **Session fixation testing** (Session hijacking)
266. **Clickjacking testing** (UI redressing)
267. **Insecure deserialization testing** (Object injection)

---

### **Category 20: Infrastructure & Cloud Testing (10 techniques)**

268. **AWS S3 bucket enumeration** (Cloud storage discovery)
269. **Azure blob storage probing** (Cloud storage testing)
270. **GCP bucket enumeration** (Google Cloud storage)
271. **Cloud IAM role enumeration** (Permission discovery)
272. **CDN configuration testing** (Content delivery network checks)
273. **Cloud function discovery** (Serverless function enumeration)
274. **Load balancer detection** (ALB, NLB identification)
275. **DNS amplification testing** (DDoS vector check)
276. **NTP amplification testing** (DDoS vector check)
277. **Container registry scanning** (Docker Hub, ECR, ACR)

---

### **Tools Used for Active Recon (Top 30):**

1. **Nmap** - Port scanning & service enumeration
2. **Masscan** - Fast port scanning
3. **Burp Suite** - Web application testing
4. **OWASP ZAP** - Web vulnerability scanning
5. **Nikto** - Web server scanner
6. **SQLmap** - SQL injection testing
7. **Nessus** - Vulnerability assessment
8. **OpenVAS** - Open vulnerability scanner
9. **Metasploit** - Exploitation framework
10. **WPScan** - WordPress vulnerability scanner
11. **Joomscan** - Joomla vulnerability scanner
12. **Hydra** - Brute force password cracking
13. **Medusa** - Parallel password testing
14. **Hashcat** - GPU password cracking
15. **John the Ripper** - Password cracking
16. **Sublist3r** - Subdomain brute force
17. **Amass** - Subdomain enumeration
18. **Fierce** - DNS enumeration
19. **Dnsrecon** - DNS reconnaissance
20. **Dirb/Dirbuster** - Directory brute force
21. **Gobuster** - Directory/DNS/vhost brute force
22. **Ffuf** - Fast web fuzzer
23. **ZAProxy** - Web proxy & scanner
24. **Shodan CLI** - Internet search queries
25. **Censys API** - Host/certificate probing
26. **SSL Labs** - SSL/TLS testing
27. **testssl.sh** - TLS/SSL scanning
28. **OpenSSL** - Certificate examination
29. **Wireshark** - Network packet capture
30. **Aircrack-ng** - WiFi cracking suite

---

---

# COMPLETE SUMMARY

## **OSINT Framework Breakdown:**

| Category | Passive Techniques | Active Techniques | Risk Level |
|----------|-------------------|-------------------|------------|
| **Search & Web** | 12 | 12 | Low → High |
| **DNS & Network** | 18 | 18 | Low → High |
| **Social Media** | 12 | 0 | Low |
| **People Search** | 11 | 10 | Low → Medium |
| **Images & Metadata** | 10 | 0 | Low |
| **Company Research** | 10 | 10 | Low → Medium |
| **Scanning & Enumeration** | 0 | 90 | High |
| **Exploitation** | 0 | 30 | Critical |
| **Infrastructure** | 0 | 10 | High |
| **Total** | **100** | **100+** | Varies |

---

## **Best Practices:**

✅ Always start with **Passive Recon** first  
✅ **Document everything** for chain of custody  
✅ Use **VPN/TOR** for anonymity in active recon  
✅ **Get written permission** before active scanning  
✅ Know your **legal jurisdiction** (CFAA in US, GDPR in EU)  
✅ **Cross-reference** multiple sources  
✅ Keep findings **organized and searchable**  
✅ Maintain **operational security (OpSec)**  

---

This comprehensive guide covers everything from the absolute basics of OSINT through 100 passive reconnaissance techniques, 100+ active reconnaissance techniques, and all essential tools!
