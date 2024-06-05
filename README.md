# controld-settings

My recommendations for the ultimate ControlD Configuration :)

# Filters 

Native:

**Ads & Trackers** -> ✅ Blocked (Balanced)

**Dynamic DNS** -> ✅ Blocked

**IoT Telemetry** -> ✅ Blocked

**Malware** -> ✅ Blocked (Strict)

**New Domains** -> ✅ Blocked (This will cause very rare breakage, but massively improves security)

**Phishing** -> ✅ Blocked

If you're fine with a little breakage, I would recommend setting Ads & Trackers to **Strict** instead of **Balanced**.

3rd Party:

Here's where it gets fun.

Despite popular opinion, due to the reasons WaLLy3K has listed [here](https://github.com/WaLLy3K/wally3k.github.io?tab=readme-ov-file#why-use-this-over-other-sources), I think it's a good idea to use multiple lists and sources, rather than just limiting yourself to one or two giant lists. I myself constantly notice domains being blocked that were caught by only one list and missed by others. I'm not saying you should go overboard, but I do think it's a good idea to use a variety of high quality lists.

I would generally recommend using the following lists:

* ⭐️ AdGuard Filter
* ⭐️ Dev Dan's Hosts
* ⭐️ Hagezi's DNS - Pro Plus
* ⭐️ Hagezi's DNS - TIF 
* ⭐️ OISD - Full
* ⭐️ StevenBlack Unified

It might seem like a lot, but these are high quality lists with strong coverage, and it doesn't really hurt to use multiple like this.

Additionally, if you're fine with a little breakage, I would highly recommend:

* 1Hosts **(Pro)**
* Hagezi's DNS - **Ultimate** instead of **Pro Plus**

# Services

You should add in here any services you don't use or care about. ControlD has a very comprehensive selection here, so I'd recommend going through the categories and taking a look yourself. I usually personally **block**:

* Finance -> Blackbaud ✅ - [Data broker](https://privacyrights.org/data-brokers/blackbaud-inc)
* Hosting -> AMP Project ✅ - [Fuck AMPs](https://brave.com/privacy-updates/18-de-amp/#why-is-amp-harmful)
* Social -> Douyin ✅ - TikTok
* Social -> Facebook ✅
* Social -> Instagram ✅ - Facebook
* Social -> LinkedIn ✅
* Social -> Messenger ✅ - Facebook
* Social -> Threads ✅ - Facebook
* Social -> TikTok ✅
* Social -> WhatsApp ✅ - Facebook
* Tools -> AnyDesk ✅ - Remote access software
* Tools -> Bugsnag ✅ - Tracker
* Tools -> Crashlytics ✅ - Tracker
* Tools -> LogMeIn ✅ - Remote access software
* Tools -> RemotePC ✅ - Remote access software
* Tools -> Splashtop ✅ - Remote access software
* Tools -> TeamViewer ✅ - Remote access software
* Vendors -> Fortinet ✅ - Monitoring software
* Vendors -> Oculus ✅ - Facebook
* Vendors -> Oracle ✅ - [Data broker](https://privacyrights.org/data-brokers/oracle-america-inc-oracle-data-cloud)
* Vendors -> Ruckus Networks ✅ - Monitoring software
* Vendors -> SolarWinds ✅ - Monitoring software

# Profile Options

**AI Malware Filter** -> ✅ (Balanced Mode)

**DNS Rebind Protection** -> ✅

