# Platforms and Architecture

### Cyber Attack Lifecycle
* Recon, Weaponize & Deliver, Exploitation, Installation, Command & Control, Act on Objective

### Security Operating Platform
* Network Security: Next-Generation Firewall
    * Identifies and inspects all traffic
    * Blocks known threats
    * Sense unknown to cloud
    * Extends to mobile and virtual networks
* Advanced Endpoint Protection: TRAPS protects endpoint
    * Inspects all Processes and files
    * Prevents known and unknown exploits
    * Integrates with cloud to prevent known and unknown malware
* Cloud Security: VM-series firewall
* Cortex
*    Prevention, detection and response platform that runs on fully integrated endpoint, network and cloud data
   * Intergrates with Prisma Access, firewalls, panorama, XDR and trap management service   
* Cortex Data Lake: Use data lake architect with Cortex XDR to create event and vulnerability correlation.

### Other items available
* Panorama: Centralized management of all PAN firewall points
* Prisma: Cloud Security
   * SaSE SD-WAN with secure web proxy/gateway, access brokers, DNS and firewall-as-a-service
   * SaaS (Aperture): protection for cloud-based systems like box, sales force, etc. helps manage permissions and file scans. Focused on DLP, PCI, and other personally exploitable data.
* Prisma Public Cloud: Cloud Security Posture Management. Taps into cloud provider API for read-only access to networ traffic, user-activity and configuration. Agents for host, container and serverless environments. Supported providers are:
   * Alibaba Cloud
   * Amazon Web Services
   * Docker EE
   * Google CloudPlatform
   * IBM Cloud
   * Kubernetes
   * Microsoft Azure
   * Rancher
   * Red Hat OpenShift
   * VMware Tanzu

* AutoFocus: Hosted security service, provides aggregate info on threat intel from multiple sources
* MineMeld: Aggregate data from multiple external threat intel sources (public and private)
* GlobalProtect: VPN that puts traffic back through the firewall to ensure traffic scanning, traffic visibility and security.

### Threat Intel Cloud
* Gathers potential threats from network and endpoints
* Analyzes and correlates threat intel
* Disseminates threat intel to network and endpoints

### Next Gen Firewall Architecture
* PAN is a single-pass Parallel Processing system 
* Single-Pass Architecture
    * Per-Packet Operations:
        * Traffic Classification with App-Id
        * User/group mapping
        * Content Scan (threats, URL, confidential data)
* Parallel Processing
    * Function specific parallel processing hardware engine
    * Separate data/control plane
* Dataplane
    * Signature Matching
        * IPS, virus, spyware, CC#, SSN
    * Security Processing
        * App-ID, User-ID, URL Match, Policy Match, App Decoding, SSL/IPSec, decompression
    * Network Processing
        * Flow Control, Route Lookup, MAC lookup, QoS, NAT
* Control Plane
    * Management
         * Configuration, Management UI, Logging, Reporting
* Zero Trust Security Model
    * No trust provided by default
    * Never Trust, always verify
    * Need to establish trust boundaries
    * NGFW offer several options to help approach the zero-trust model
         * App-ID, User-ID, URL filtering, Vuln filtering, anti-spyware, anti-virus, Traps, file blocking, DOS protection, Zone Protection, Wildfire

### Firewall Offerings
* Physical devices:
    * PA-220, PA-800, PA-3200, PA-5200 are Next Gen hardware
    * PA-7000 series are Chassis architecture for NGFW
    * M-200, M-500/WF-500/600 : Panorama & WildFire
* Virtual devices:
    * VM-700, VM-500, VM-300, VM-100, VM-50, VM-50lite
    * Supported environment
        * ESXi: All
        * KVM/Openstack: All
        * Hyper-V: All
        * VMWare NSX: VM100-500
        * AWS: VM100-700
        * Azure: VM100-700
    * New sessions all models: 8000 per second
    * IPSec throughput, all models: Varies according to model (originally was 250mbps, per the training, however documentation states otherwise. Please see the hardware spec sheet at the top of this post for specifics)
* Virtual Systems
    * Ability to have seperate virtual firewalls in a single physical chassis
    * Each system has its own zones, policies, administrators
    * Supported on the 3k/5k/7k models

* Machine Learning-Powered Next-Generation Firewalls
  
  * Palo Alto Networks Machine Learning (ML)–powered Next-Generation Firewalls (NGFWs) enable you
    to adopt best practices by using application, user, and content-based policies to minimize
    opportunities for attack. They are available as physical appliances, virtualized appliances, and
    cloud-delivered services–all of which can be managed with Panorama to ensure a consistent
    security stance.
