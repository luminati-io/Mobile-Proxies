# Bright Data Mobile Proxies

[![Promo](https://github.com/luminati-io/Rotating-Residential-Proxies/blob/main/50%25%20off%20promo.png)](https://brightdata.com/proxy-types/mobile-proxies)

## Overview
Access the internet as a real mobile user with Bright Data's [mobile proxy network](https://brightdata.com/proxy-types/mobile-proxies), featuring millions of 3G, 4G, and 5G IPs from around the world.

- **7,000,000+ Mobile IPs**
- **3G/4G/5G mobile IPs**
- **99.99% Uptime with 24/7 support**
- **Geo-location targeting (Free)**

## Key Features
- **Global Reach**: Access mobile IPs across [195 countries](https://brightdata.com/locations).
- **High Success Rates**: Achieve up to 99.9% success in data collection and testing tasks.
- **Real Mobile Connections**: Mobile IPs sourced from real devices on genuine networks.
- **Unlimited Scaling**: Scale with concurrent sessions and high-availability infrastructure.
- **Carrier-Level Targeting**: Target by specific carriers for in-depth, accurate insights.

## Pricing Plans
- **Pay As You Go**: $8.4/GB with no monthly commitment.
- **Monthly Subscriptions**:
  - **69 GB**: $7.14/GB, $499/month + VAT.
  - **158 GB**: $6.3/GB, $999/month + VAT.
  - **339 GB**: $5.88/GB, $1999/month + VAT.
  - **Enterprise Plans**: Custom pricing and packages available.

[![Promo](https://github.com/luminati-io/LinkedIn-Scraper/blob/main/Proxies%20and%20scrapers%20GitHub%20bonus%20banner.png)](https://brightdata.com/proxy-types/mobile-proxies) 

## Getting Started with Mobile Proxies
1. **Start Free Trial**: No credit card required.
2. **Integration**: Use APIs or the Bright Data Control Panel to manage IPs and configurations.
3. **Supported Languages**: Quick start examples provided for Python, Java, C#, Node.js, and Shell.

## Code Examples

### Python

```python
import sys

# Replace '[your customerID]', 'mobile', and '[your password]' with your actual Bright Data customer ID, zone, and password
if sys.version_info[0] == 2:
    import six
    from six.moves.urllib import request
    opener = request.build_opener(
        request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-mobile:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-mobile:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())

if sys.version_info[0] == 3:
    import urllib.request
    opener = urllib.request.build_opener(
        urllib.request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-mobile:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-mobile:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())
```

### Java

```java
package example;

import org.apache.http.HttpHost;
import org.apache.http.client.fluent.*;

public class Example {
    public static void main(String[] args) throws Exception {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        HttpHost proxy = new HttpHost("brd.superproxy.io", 22225);
        String res = Executor.newInstance()
            .auth(proxy, "brd-customer-[your customerID]-zone-mobile", "[your password]")
            .execute(Request.Get("https://geo.brdtest.com/mygeo.json").viaProxy(proxy))
            .returnContent().asString();
        System.out.println(res);
    }
}
```

### C#

```c#
using System;
using System.Net;

class Example
{
    static void Main()
    {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        var client = new WebClient();
        client.Proxy = new WebProxy("brd.superproxy.io:22225");
        client.Proxy.Credentials = new NetworkCredential("brd-customer-[your customerID]-zone-mobile", "[your password]");
        Console.WriteLine(client.DownloadString("https://geo.brdtest.com/mygeo.json"));
    }
}
```

### Node.js

```node.js
require('request-promise')({
    url: 'https://geo.brdtest.com/mygeo.json',
    proxy: 'http://brd-customer-[your customerID]-zone-mobile:"[your password]"@brd.superproxy.io:22225',
})
.then(function(data){ console.log(data); },
    function(err){ console.error(err); });
```

### Shell 

```shell
# Replace '[your customerID]' and '[your password]' with your actual credentials
curl --proxy brd.superproxy.io:22225 --proxy-user brd-customer-[your customerID]-zone-mobile:[your password] -k "https://geo.brdtest.com/mygeo.json"
```

## Integrations
Our mobile proxies integrate seamlessly with popular tools and frameworks:

- [**Puppeteer**](https://brightdata.com/integration/puppeteer)
- [**Selenium**](https://brightdata.com/integration/selenium)
- [**Playwright**](https://brightdata.com/integration/playwright)
- [**AdsPower**](https://brightdata.com/integration/adspower)
- [**MultiLogin**](https://brightdata.com/integration/multilogin)

## Use Cases
Common applications for mobile proxies:

- [**eCommerce**](https://brightdata.com/use-cases/ecommerce): Track pricing and product availability.
- [**Social Media**](https://brightdata.com/use-cases/social-media-for-marketing): Monitor trends and engagement.
- [**Real Estate**](https://brightdata.com/use-cases/real-estate): Collect data on property listings.
- [**Travel**](https://brightdata.com/use-cases/travel): Compare travel deals across locations.

## FAQ

### What is a Mobile Proxy?
A mobile proxy routes traffic through mobile IPs provided by real carriers, allowing access to the internet from mobile networks.

### What are Mobile Proxies used for?
Mobile proxies are commonly used for ad verification, mobile app testing, location-based data collection, social media monitoring, and a lot more.

### Why use a Mobile Proxy?
Mobile proxies offer high anonymity and are less likely to be detected, providing access to mobile network data as seen by real users.

### Do you offer 5G Mobile Proxies?
Yes, Bright Data offers fast and secure 5G mobile proxies.

### Which mobile carrier IPs can I choose?
We offer IPs from a range of popular carriers, including [AT&T](https://brightdata.com/solutions/att-proxy), [T-Mobile](https://brightdata.com/solutions/t-mobile-proxy), [Verizon](https://brightdata.com/solutions/verizon-proxy), and many others worldwide.

### Are mobile proxies legal?
Yes, Bright Data's mobile proxies comply with all relevant laws, including GDPR and CCPA, ensuring privacy and legal usage.

### Do you offer USA mobile proxies?
Yes, we provide mobile proxies in the USA and globally, including major carrier IPs like AT&T and T-Mobile.

### Can I choose mobile IPs by country and city?
Yes, Bright Data’s mobile proxy network allows targeting by specific countries and cities.

### How does Bright Data acquire its Mobile Proxies?
Bright Data partners with app developers, who integrate our SDK, allowing users to opt in to share their mobile IPs in exchange for benefits such as ad-free experiences or app upgrades.
