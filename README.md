# Cribl Search ZScaler
----

This pack should be used to display data regarding ZScaler logs.


## Requirements Section

The dataset leveraged here is **zscalernss**. It is expected to be partitioned by sourcetype for best performance. The pack macros use the following sourcetype values (update the macros if your schema differs):

* **Web Logs:** `dataset="zscalernss"` `sourcetype="zscalernss-web"`
* **Firewall Logs:** `dataset="zscalernss"` `sourcetype="zscalernss-fw"`
* **CASB Logs:** `dataset="zscalernss"` `sourcetype="zscalernss-casb"`
* **Audit Logs:** `dataset="zscalernss"` `sourcetype="zscalernss-audit"`
* **VPN Logs:** `dataset="zscalernss"` `sourcetype="zscalernss-tunnel"`
* **DNS Logs:** `dataset="zscalernss"` `sourcetype="zscalernss-dns"`
* **DLP Logs:** `dataset="zscalernss"` `sourcetype="zscalernss-emaildlp"`


## Dashboards

The pack includes one dashboard per log type:

| Dashboard | Description |
|-----------|-------------|
| **ZScaler Web Logs** | NSS web traffic: threats, DLP, blocked/allowed categories, file types, top URLs. |
| **ZScaler Firewall Logs** | Firewall traffic: allow/block, categories, rules, locations, apps, top sources/destinations, traffic by country. |
| **ZScaler CASB Logs** | Cloud Access Security Broker: cloud app usage, DLP categories, threats, policy/rule actions. |
| **ZScaler Email DLP Logs** | Email DLP: scanned emails, sensitive data types (dictionaries), DLP engines, policy actions, rules, departments, file types. |
| **ZScaler Audit Logs** | Admin activity: sign-in/out, actions, categories, success vs failure, interface (API/UI), admin by login source (clientip). |
| **ZScaler DNS Logs** | DNS queries: allowed/blocked, top domains, record types, categories, rules, locations. |
| **ZScaler VPN Tunnel Logs** | VPN/tunnel: tunnel samples and events, types, locations, source/destination IPs, event types and reasons. |


## Using The Pack

To use this Pack, follow these steps:

1. Install the pack from the dispensary.
2. Check dataset naming conventions and update the macros if needed.
3. View your data using the dashboards or run searches with the pack macros.


## Release Notes

### Version 1.0.0 - 2026-02-27
Updated macros for better efficiency in searching; added dashboards for CASB, Audit, DLP, DNS, VPN logs.

### Version 0.9.1 - 2025-09-05
Updated dashboards to leverage time picker. Also removed unnecessary search.

### Version 0.1.1 - 2025-07-01
Initial Release

## Contact
To contact us please email <kprior@cribl.io> or reach out on Cribl Community Slack to @Kelsey Prior (cribl.io) or on #packs. If you have any suggestions for panels, please let us know!


## License
This Pack uses the following license: [`Apache 2.0`](http://apache.org/licenses/LICENSE-2.0).
