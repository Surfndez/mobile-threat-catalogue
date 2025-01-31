---
layout: threat
ThreatCategory: Malicious or privacy-invasive application
ID: APP-24
Threat: Covertly Track Device Location
ThreatDescription: Apps that have been granted permission to Location Services or similar OS-provided services can abuse this permission to report device outside of what may be needed to support legitimate app functionality (e.g. navigation). Device location data may facilitate further attacks such as geo-physical or behavioral tracking of the user.
ThreatOrigin: 'Dissecting Android Malware: Characterization and Evolution [^85]'
ExploitExample:
  - An investigation of Chrysaor Malware on Android [^AndroidDevBlog-1]
CVEExample:
PossibleCountermeasures:
    Enterprise:
      - Deploy MAM or MDM solutions with policies that prohibit the side-loading of apps, which may bypass security checks on the app.
      - Deploy MAM or MDM solutions with policies that prohibit the installation of apps from 3rd party (unofficial) app stores.
      - Use application threat intelligence data about potential abuse of location services associated with apps installed on COPE or BYOD devices
    Mobile Device User:
      - Use Android Verify Apps feature to identify apps that may abuse location services.
      - When apps that require location services (e.g., map services) are not in use, use OS-provided settings to globally disable access to location services
      - When using untrusted apps that require locations services (e.g., map services), use OS-provided settings to revoke access to location services once the app is no longer in use.
title: APP-24
rawID: 24
---
