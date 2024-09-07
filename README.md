# controld-settings

My recommendations for the ultimate ControlD Configuration :)

**NOTE:** This project can be found on both [Codeberg](https://codeberg.org/celenity/controld-settings), which will act as the main & preferred way to contribute, and [GitHub](https://github.com/celenityy/controld-settings).

# Filters 

Native:

* **Ads & Trackers** -> ✅ `Blocked` (`Balanced`)

* **Dynamic DNS** -> ✅ `Blocked`

* **IoT Telemetry** -> ✅ `Blocked`

* **Malware** -> ✅ `Blocked` (`Strict`)

* **New Domains** -> ✅ `Blocked` *(This will cause very rare breakage, but massively improves security)*

* **Phishing** -> ✅ `Blocked`

If you're fine with a little breakage, I would highly recommend setting Ads & Trackers to `**Strict**` instead of `**Balanced**`.

3rd Party:

Here's where it gets fun.

Despite popular opinion, due to the reasons WaLLy3K has listed [here](https://github.com/WaLLy3K/wally3k.github.io?tab=readme-ov-file#why-use-this-over-other-sources), I think it's a good idea to use multiple lists and sources, rather than just limiting yourself to one or two giant lists. I myself constantly notice domains being blocked that were caught by only one or two lists and missed by others. **I'm not saying you should go overboard, but I do think it's a good idea to use a variety of high quality lists for the best coverage possible.**

I would generally recommend using the following lists:

* ⭐️ `AdGuard Filter`

* ⭐️ `Dev Dan's Hosts`

* ⭐️ `Hagezi's DNS - Pro Plus`

* ⭐️ `Hagezi's DNS - TIF`

* ⭐️ `OISD - Full`

* ⭐️ `StevenBlack Unified`

It might seem like a lot, but these are carefully picked high quality lists with strong coverage, and it doesn't really hurt to use multiple like this.

Additionally, if you're fine with a little breakage, I would highly recommend:

* `1Hosts **(Pro)**`

* `Hagezi's DNS - `**Ultimate** instead of `Hagezi's DNS - `**Pro Plus**

# Services

You should use this feature to your advantage and block any services that you don't use or care about. This can dramatically improve your privacy by preventing connections to them from even being made. If you use a service, don't block it, just block what you're comfortable with and works best for you.

I personally block:

* Audio -> **Spotify** -> `Blocked` ✅

* Finance -> **Blackbaud** -> `Blocked` ✅ - *[Data broker](https://privacyrights.org/data-brokers/blackbaud-inc)*

* Finance -> **Equifax** -> `Blocked` ✅ - *[Data broker](https://privacyrights.org/data-brokers/equifax-information-services-llc)*

* Finance -> **Experian** -> `Blocked` ✅ - *[Data broker](https://privacyrights.org/data-brokers/experian-data-corp)*

* Hosting -> **AMP Project** -> `Blocked` ✅ - *[Fuck AMPs](https://brave.com/privacy-updates/18-de-amp/#why-is-amp-harmful)*

* Shop -> **Rakuten** -> `Blocked` ✅

* Social -> **Douyin** -> `Blocked` ✅ - *TikTok*

* Social -> **Facebook** -> `Blocked` ✅

* Social -> **Gravatar** -> `Blocked` ✅

* Social -> **Instagram** -> `Blocked` ✅ - *Facebook*

* Social -> **LinkedIn** -> `Blocked` ✅

* Social -> **Messenger** -> `Blocked` ✅ - *Facebook*

* Social -> **Threads** -> `Blocked` ✅ - *Facebook*

* Social -> **TikTok** -> `Blocked` ✅

* Social -> **VK** -> `Blocked` ✅

* Social -> **Viber** -> `Blocked` ✅ - *Rakuten*

* Social -> **WeChat** -> `Blocked` ✅

* Social -> **WhatsApp** -> `Blocked` ✅ - *Facebook*

* Tools -> **AnyDesk** -> `Blocked` ✅ - *Remote access software*

* Tools -> **Bugsnag** -> `Blocked` ✅ - *Tracker*

* Tools -> **Crashlytics** -> `Blocked` ✅ - *Tracker*

* Tools -> **LogMeIn** -> `Blocked` ✅ - *Remote access software*

* Tools -> **Opera Browser** -> `Blocked` ✅

* Tools -> **RemotePC** -> `Blocked` ✅ - *Remote access software*

* Tools -> **Salesforce** -> `Blocked` ✅

* Tools -> **Splashtop** -> `Blocked` ✅ - *Remote access software*

* Tools -> **TeamViewer** -> `Blocked` ✅ - *Remote access software*

* Vendors -> **AVG** -> `Blocked` ✅

* Vendors -> **Avast** -> `Blocked` ✅

* Vendors -> **Avira** -> `Blocked` ✅

* Vendors -> **Fortinet** -> `Blocked` ✅ - *Used for monitoring*

* Vendors -> **McAfee** -> `Blocked` ✅

* Vendors -> **Norton** -> `Blocked` ✅

* Vendors -> **Oculus** -> `Blocked` ✅ - *Facebook*

* Vendors -> **Oracle** -> `Blocked` ✅ - *[Data broker](https://privacyrights.org/data-brokers/oracle-america-inc-oracle-data-cloud)*

* Vendors -> **Qihoo 360** -> `Blocked` ✅

* Vendors -> **Ruckus Networks** -> `Blocked` ✅ - *Used for monitoring*

* Vendors -> **SolarWinds** -> `Blocked` ✅ - *Used for monitoring*

* Vendors -> **Symantec** -> `Blocked` ✅ - *Used for monitoring*

* Video -> **Rakuten TV** -> `Blocked` ✅ - *Rakuten*

# Custom Rules

I would recommend making a custom rule here to `bypass` *(why is it worded like this????)* `controld.com`, to ensure that we can always access the dashboard, regardless of any rogue filters or other unexpected events.

# Profile Options

**AI Malware Filter** -> ✅ (`Balanced Mode`)

**DNS Rebind Protection** -> ✅

**Disable DNSSEC** -> ❌ *(This should be the default, but I've seen some guides recommend enabling this, which is why it's here. DNSSEC is important, please leave it on)*

# Devices

**Graph icon** -> `Some analytics` *(Having some analytics is important for troubleshooting breakage)*

# Account

**Two-Factor Auth** -> ✅

**Storage Region** -> `Sydney, AU`

# Additional recommendations

* Use a privacy-respecting browser like [Firefox](https://www.mozilla.org/firefox/) with a user.js like [Arkenfox](https://github.com/arkenfox/user.js).

* Make sure to configure ControlD on **both** your OS and in your browser. This will allow you to take advantage of [Encrypted Client Hello](https://blog.cloudflare.com/announcing-encrypted-client-hello).

* Use a content blocking extension like [uBlock Origin](https://github.com/gorhill/uBlock). *(See recommended settings [here](https://codeberg.org/celenity/ublock-origin-settings))*

* Enable Safe Browsing in your browser if possible and if it's not done in a privacy-invasive way. (You should use i.e. [Google Safe Browsing on "Standard" Mode](https://safebrowsing.google.com/), [Firefox's Safe Browsing](https://support.mozilla.org/kb/how-does-phishing-and-malware-protection-work), [Brave's Safe Browsing](https://brave.com/privacy/browser/#safe-browsing), & [Safari's Fraudulent Website Warning](https://www.apple.com/legal/privacy/data/en/safari/), you should avoid most other options i.e. [Google Safe Browsing on "Enhanced" Mode](https://safebrowsing.google.com/), [Microsoft SmartScreen](https://learn.microsoft.com/windows/security/operating-system-security/virus-and-threat-protection/microsoft-defender-smartscreen/), & [Opera Sitecheck](https://blogs.opera.com/security/2021/01/making-browsing-safe-from-phishing/)).

* Use a (reputable) anti-virus if possible. On Windows, you can use the built-in [Microsoft Defender Antivirus](https://wikipedia.org/wiki/Microsoft_Defender_Antivirus), on macOS, you can stick to the built-in [XProtect](https://support.apple.com/guide/security/protecting-against-malware-sec469d47bd8/web), on Android, you can use [Hypatia](https://f-droid.org/packages/us.spotco.malwarescanner/), and on Linux, you can use [ClamAV](https://www.clamav.net/). **NOTE:** You should install Hypatia through the [DivestOS Official Repo](https://divestos.org/fdroid/official/?fingerprint=E4BE8D6ABFA4D9D4FEEF03CDDA7FF62A73FD64B75566F6DD4E5E577550BE8467) instead of F-Droid's main repo, as it will allow you to receive quicker updates directly from the developer. It's also recommended to use [F-Droid Basic](https://f-droid.org/en/packages/org.fdroid.basic/) as your F-Droid client of choice.