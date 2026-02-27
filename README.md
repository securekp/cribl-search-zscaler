# Cribl Search ZScaler
----

This pack should be used to display data regarding ZScaler logs.


## Requirements Section

The dataset leveraged here is zscalernss. It is expected to be partitioned by sourcetype for best performance. Below are the sourcetypes that are set up currently. If you do not use this schema, make sure to update the macros in this pack to fit what your datasets look like. 
* Web Logs: dataset="zscalernss" sourcetype="zscalernss_web"
* Firewall Logs: dataset="zscalernss" sourcetype="zscalernss_fw"
* CASB Logs: dataset="zscalernss" sourcetype="zscalernss_casb"
* Audit Logs: dataset="zscalernss" sourcetype="zscalernss_audit"
* VPN Logs: dataset="zscalernss" sourcetype="zscalernss_tunnel"
* DNS Logs: dataset="zscalernss" sourcetype="zscalernss_dns"
* DLP Logs: dataset="zscalernss" sourcetype="zscalernss_emaildlp"


## Using The Pack

To use this Pack, follow these steps:

1. Install the pack from the dispensary.
2. Check dataset naming conventions and update the macros if needed. 
3. View your data!


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
