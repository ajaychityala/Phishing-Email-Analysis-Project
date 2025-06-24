 Phishing-Email-Analysis-Project
 Phishing Email Analysis Project

 Task 1: Understanding Phishing and Email Threat Detection

---

 1. What is phishing?
Phishing is a cyberattack where attackers impersonate trusted entities (banks, companies, or individuals) to trick recipients into revealing sensitive data such as passwords, bank details, or login credentials. It commonly spreads via email or fake websites.



 2. How to identify a phishing email?
- Generic greetings like "Dear User"
- Suspicious sender email address or domain
- Urgent or threatening language
- Mismatched URLs (hover to inspect)
- Spelling/grammar errors
- Requests for personal or financial information
- Strange or malicious attachments


 3. What is email spoofing?
Email spoofing is the practice of forging the sender's address to make an email appear to come from a trusted source. It’s used in phishing to trick recipients into trusting the message.


 4. Why are phishing emails dangerous?
- Steal sensitive credentials and data
- Install malware or ransomware
- Lead to financial loss and identity theft
- Enable further attacks via compromised accounts



 5. How can you verify the sender’s authenticity?
- Inspect the full email address (not just display name)
- Analyze email headers (check SPF/DKIM/DMARC)
- Confirm via official sources or known contacts
- Use WHOIS lookup or domain verification tools

 6. What tools can analyze email headers?
- [Google Header Analyzer](https://toolbox.googleapps.com/apps/messageheader/)
- MXToolbox
- Mailheader.org
- GCA Email Threat Analyzer


 7. What actions should be taken on suspected phishing emails?
- Do notclick on any links or attachments
- Report the email using phishing/report feature
- Forward it to your security team (e.g., SOC or CERT)
- Analyze headers and URLs before deletion
- Block domain/sender in your email client or firewall
- 
 8. How do attackers use social engineering in phishing?
Phishers manipulate human emotions like urgency, fear, trust, and curiosity:
- "Your account will be locked in 24 hours!"
- "Click here to receive a refund!"
- "Update your security information now!"

 Phishing Email Sample Analysis

 Sample Email Summary

| Field       | Detail |
|-------------|--------|
| **From**    | accounts@firstgenericbank.com |
| **Subject** | Please update your account information |
| **Link**    | `http://www.firstgenericbank.com.account-updateinfo.com` |
| **Greeting**| Generic: "Dear First Generic Bank user" |

  Phishing Indicators Found

| # | Indicator                  | Description |
|---|----------------------------|-------------|
| 1 | **Spoofed Domain**         | Looks like `firstgenericbank.com` but belongs to `account-updateinfo.com`. |
| 2 | **Urgent Language**        | Warns the user of 48-hour action deadline. |
| 3 | **Generic Salutation**     | No personal name used. |
| 4 | **Requests Sensitive Info**| ATM PIN, SSN, and personal info. |
| 5 | **Unsecure Protocol**      | Uses `http` instead of secure `https`. |
| 6 | **Fake Website**           | No real navigation, generic design. |
| 7 | **Social Engineering**     | Uses fear of account suspension. |

 Tools Used

- Google Email Header Analyzer
- Manual link inspection (hover preview)
- Browser sandbox for viewing page

 Conclusion

The email is a phishing attempt that uses spoofed domains, urgency, and social engineering to extract personal banking information. It demonstrates multiple classic phishing characteristics and should be reported immediately.


