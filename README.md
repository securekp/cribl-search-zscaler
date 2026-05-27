# Cribl Search ZScaler
----

This pack should be used to display data regarding ZScaler logs and used in conjunction with the Cribl Stream ZScaler pack https://packs.cribl.io/packs/cribl-zscaler. 


## Requirements Section

The dataset leveraged here is zscalernss. It is expected to be partitioned by sourcetype for best performance. Below are the sourcetypes that are set up currently. If you do not use this schema, make sure to update the macros in this pack to fit what your datasets look like. 
* Web Logs: dataset="zscalernss" sourcetype="zscalernss-web"
* Firewall Logs: dataset="zscalernss" sourcetype="zscalernss-fw"
* CASB Logs: dataset="zscalernss" sourcetype="zscalernss-casb"
* Audit Logs: dataset="zscalernss" sourcetype="zscalernss-audit"
* VPN Logs: dataset="zscalernss" sourcetype="zscalernss-tunnel"
* DNS Logs: dataset="zscalernss" sourcetype="zscalernss-dns"
* DLP Logs: dataset="zscalernss" sourcetype="zscalernss-emaildlp"


## Using The Pack

To use this Pack, follow these steps:

1. Install the pack from the dispensary.
2. Check dataset naming conventions and update the macros if needed. 
3. Ensure that the dataset has the correct datatype from the pack applied to ensure parsing occurs.
    a. If your data is coming from Stream using the ZScaler pack, use the "ZScaler Datatypes" datatype. This is what is configured by default.
    b. If your data is coming via passthru, use the "Zscaler Raw Datatypes" datatype.
4. View your data!

## Dashboards

The pack includes one dashboard per log type.

## Release Notes
### Version 1.0.3 - 2026-05-27
Update naming mechanisms

### Version 1.0.2 - 2026-05-01
Added separate datatypes for passthru vs using the Cribl Stream ZScaler pack. Cleaned up readme. Switched to using parent searches for each dashboard that operates better with parent searches.

### Version 1.0.1 - 2026-03-12
Added parser for _raw.event to each datatype rule. This is necessary when using the Stream ZScaler pack. 

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
