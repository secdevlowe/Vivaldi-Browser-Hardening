# Vivaldi-Browser-Hardening

This repository uses security-focused addons, tweaks configuration settings, and refers to best practices to enhance the security and privacy of the Vivaldi browser. Implementing these settings will reduce the chances of a user having malware infections, data breaches, and/or privacy exploits while using the Vivaldi (Chromium) Browser.

## Features

* Null/decreased home calling
* Privacy improvements 
	* Network-state partitioning system & user-agent, color scheme, preventing media devices native spoofing, 
	* Client hints, sensors, idle detection, Federated Learning of Cohorts (FLoC), reporting, & other privacy vulnerable features blocked
	* Encrypt client hello enabled, previously known as encrypted SNI
* Security improvments
	* Just-In-Time-Less [JITLess](https://v8.dev/blog/jitless) mode
	* GPU, renderer, & network services in AppContainers enabled
	* Arbitrary Code Guard (ACG) & Code Integrity Guard (CIG) mitigations in the renderer & network processes
	* Client/Server Runtime Subsystem (Csrss.exe) lockdown
* Better performance & resource management
	* Improved caching & throttling system
	* Parallel downloading
* Ameliorated browsing usage without degradation privacy

## Credits

* [melo936](https://github.com/melo936/ChromiumHardening)
* [JITLess](https://v8.dev/blog/jitless)
* [Super Duper Secure Mode](https://microsoftedge.github.io/edgevr/posts/Super-Duper-Secure-Mode)
* [List of Chromium Command Line Switches](https://peter.sh/experiments/chromium-command-line-switches/)
* [Chromium Docs](https://chromium.googlesource.com/chromium/src/+/main/docs/configuration.md)
* [Vivaldi Help](https://help.vivaldi.com)

## License

Licensed under the MIT open source license.

## DISCLAIMER

THE INFORMATION PROVIDED IN THIS DOCUMENT ON BROWSER HARDENING IS INTENDED FOR GENERAL INFORMATIONAL PURPOSES ONLY. WHILE I STRIVE TO ENSURE THE ACCURACY AND RELIABILITY OF THE INFORMATION, IT IS PROVIDED "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED. THE STEPS AND SUGGESTIONS PROVIDED ARE BASED ON CURRENT BEST PRACTICES AND KNOWN SECURITY TECHNIQUES AT THE TIME OF WRITING.

I DO NOT GUARANTEE THAT FOLLOWING THESE STEPS WILL MAKE YOUR BROWSER COMPLETELY SECURE. USERS ARE ENCOURAGED TO STAY INFORMED ABOUT THE LATEST SECURITY DEVELOPMENTS AND CONTINUOUSLY UPDATE THEIR SECURITY PRACTICES.

IMPLEMENTING SOME OF THESE MEASURES MAY AFFECT THE FUNCTIONALITY OF CERTAIN WEBSITES OR APPLICATIONS. USERS SHOULD CONSIDER THEIR SPECIFIC NEEDS AND BALANCE SECURITY WITH USABILITY VIA TESTING THE SETTINGS PRESENTED IN THIS REPOSITORY/RESEARCHING ON THEIR OWN.

I AM NOT RESPONSIBLE FOR ANY ISSUES OR DAMAGES ARISING FROM THE USE OR MISUSE OF THE INFORMATION PROVIDED. ALWAYS EXERCISE CAUTION AND CONSIDER CONSULTING WITH A CYBERSECURITY PROFESSIONAL FOR PERSONALIZED ADVICE TAILORED TO YOUR SPECIFIC SITUATION.
