---
layout: page
permalink: /release-notes/
---

<!--{% include formspree.html email="my_name@gmail.com" redirect="/thanks/" name="true" subject="true" %}-->
<h1 class="uk-text-left">Release Notes</h1>

<div class="noteLeft">
    <p>January 28th, 2022</p>
</div>

<div class="noteRight">
    <h3>22.01 Updates</h3>
    <p>We are pleased to announce the 22.01 release of Intel&reg; Smart Edge Open software. This release features an updated Private Wireless Experience Kit for CentOS 7.9 that uses Intel&reg; Edge Software Provisioner to automate deployment.</p>
    <a class="uk-button uk-button-info uk-button-small uk-margin-small-bottom">Added</a>
    <p>The <a href="/docs/experience-kits/private-wireless-experience-kit/" title="Intel&reg; Private Wireless Experience Kit">Intel&reg; Private Wireless Experience Kit</a> supports a single orchestration domain, optimizing the edge node to support both applications and NG-RAN and NG-Core network functions such as DU/CU, AMF, SMF, and UPF.</p>
    <p>Autonomous Deployment Through Intel&reg; Edge Software Provisioner (Intel&reg; ESP): Easy provisioning of a multi-node environment with CentOS 7.9. Intel&reg; ESP enables ODMs, system integrators and developers to automate the installation of a complete operating system and software stack on bare-metal or virtual machines using a just-in-time provision process.</p>
    <p>A new SR-IOV FEC operator to configure the Intel&reg; vRAN Accelerator ACC100 Adapter, and a SR-IOV Network Operator to configure the Intel&reg; Ethernet Converged Network Adapter X710-DA4. This replaces the manual process that was needed in the previous version</p>
    <p>Wireless Network Ready Intelligent Traffic Management (ITM) application integration to demonstrate and test the capabilities of the experience kit. Once the application has been deployed on the edge node in a 5G network, the application pod takes in virtual/real RTSP (real time streaming protocol) addresses, performs inference, and sends metadata for each video stream to an InfluxDB database. In parallel, the visualizer overlays the analysis on the metadata, displaying pedestrians detected, collisions observed, and the processed video feed.</p>
    <p>Intel&reg; Ice Lake™ Scalable Processor Support: Support for the Dell EMC PowerEdge&reg; R750 with 3rd Generation Intel&reg; Xeon&reg; Scalable Processors</p>
    <a class="uk-button uk-button-warning uk-button-small uk-margin-small-bottom">Known Issues</a>
    <ul>
        <li>Sometimes the Dell R750 edge node hangs during reboot when using an Ethernet card based on Intel&reg; Ethernet Controller XL710. This is because Intel&reg; Ethernet Controller XL710 based Ethernet cards are not in the Dell official support list. We will upgrade the Private Wireless Experience Kit to use an E810 NIC, which is supported by Dell, in the next release.</li>
        <li>5G CNFs - User equipment sometimes fails to reattach when it moves from idle mode to active mode. This issue will be addressed with future 5G Core CNF upgrades.</li>
    </ul>
    <a href="https://github.com/smart-edge-open/docs/blob/main/release-notes/release-notes-se-open-PWEK-22-01.md" rel="nofollow" target="_blank" title="Read more">Read more</a>
    <br><br><br>
    <style>
        .uk-button.uk-button-info.uk-button-small.uk-margin-small-bottom{ 
            margin-bottom: 20px !important;
            }
    </style>
</div>

<div class="noteLeft">
    <p>December 17th, 2021</p>
</div>

<div class="noteRight">
    <h3>21.12 Updates</h3>
    <p>We are pleased to announce the 21.12 release of Intel&reg; Smart Edge Open software.</p>
    <a class="uk-button uk-button-info uk-button-small uk-margin-small-bottom">Added</a>
    <p>The <a href="/docs/experience-kits/developer-experience-kit">Developer Experience Kit</a> now supports <a href="https://www.intel.com/content/www/us/en/architecture-and-technology/security-libraries-for-data-center-article.html" target="_blank" >Intel&reg; Security Libraries for Data Center</a> (Intel&reg; SecL-DC) for platform integrity.  Platform integrity is established from a collection of both hardware and software that perform measurement and verification to ensure a platform boots into a trusted and desired state.</p>
    <p>In addition, the Developer Experience Kit also supports <a target="_blank" href="https://www.intel.com/content/www/us/en/developer/tools/software-guard-extensions/overview.html"> Intel&reg; Software Guard Extensions</a> (Intel&reg;  SGX) for protection of selected code and data within a hardened enclave. Developers can now partition their application into hardened enclaves or trusted execution environments to increase application security.</p>
    <p>We are excited to announce an O-RAN compliant near-real time RAN Interface Controller (RIC) is available for the Developer Experience Kit and will soon be available for download from the <a target="_blank" href="https://www.intel.com/content/www/us/en/developer/tools/software-catalog/full-catalog.html?s=Newest&q=%22smart%2Bedge%2Bopen%22">Intel&reg; Developer Catalog.</a> The RIC can be used for development and testing of ORAN AI/ML xAPPs. A 5G RAN simulator is provided to facilitate development and testing.</p>
    <p>Support has been added for the next generation Intel&reg; Xeon&reg;  D processor. More details will be provided after the product has launched.</p>
    <br>
    <style>
        .uk-button.uk-button-info.uk-button-small.uk-margin-small-bottom{ 
            margin-bottom: 20px !important;
            }
    </style>
</div>

<div class="noteLeft">
    <p>September 30th, 2021</p>
</div>
<div class="noteRight">
    <h3>21.09 Updates</h3>
    <p>We are pleased to announce the first release Intel&reg; Smart Edge Open.</p>
    <p>Built from an OpenNESS foundation and representing more than two years of development, the 21.09 release of Intel&reg; Smart Edge Open introduces several technical improvements including a new Developer Experience Kit and an upgraded experience kit for creating 5G private wireless networks.</p>
    <a class="uk-button uk-button-info uk-button-small uk-margin-small-bottom">Added</a>
    <p>Introduced the Developer Experience Kit</p>
    <p>Intel&reg; Smart Edge Open is shifting to Ubuntu 20.04 LTS as the default OS in order to simplify future OS support. The Developer Experience kit uses Ubuntu 20.04 LTS. Other experience kits will be updated from CentOS to Ubuntu in future releases</p>
    <ul class="uk-margin-small-top">
        <li>Automated deployment process for experience kits, based on the Intel&reg; Edge Software Provisioner (Intel® ESP). (Currently available in the Developer Experience Kit.)</li>
        <li>Developer Experience Release Notes</li>
    </ul>
    <p>5G Private Wireless Experience Kit with Integrated RAN that combines a 5G core, 5G RAN and Intel® Smart Edge Open platform in a single, validated solution, using commercial grade CNFs.</p>
    <ul class="uk-margin-small-top">
        <li>Support for 3rd Generation Intel® Xeon® Scalable Processors (code name Ice Lake)</li>
        <li>Support for Intel® vRAN Dedicated Accelerator ACC100</li>
        <li>Support for Intel® QuickAssist Adapter 8970</li>
        <li>Support for Intel® Ethernet Converged Network Adapter X710-DA4</li>
        <li>CNF support
            <ul>
                <li>DU: L1 verified FlexRAN BBU v20.11</li>
                <li>DU: L2 verified Radisys L2 DU v2.2</li>
                <li>CU: L2/L3 verified Radisys L2/L3 CU v2.2</li>
                <li>UPF, AMF and SMF: verified Radisys 5G Core v2.2</li>
            </ul>
        </li>
        <li>Support for Foxconn Sub6 4x4 RRH
            <ul>
                <li>RPQN-7800, 3.3-3.6GHz with firmware version: v1.0.3q 432</li>
            </ul>
        </li>
    </ul>
    <a class="uk-button uk-button-success uk-button-small uk-margin-small-bottom">Changed</a>
    <ul class="uk-margin-small-top">
        <li>5G On Premises Edge has been re-named to 5G Private Wireless Experience Kit with Integrated RAN</li>
        <li>Calico CNI is the default CNI for Intel® Smart Edge Open.</li>
        <li>All documentation for Intel® Smart Edge Open is now publicly available</li>
    </ul>
    <a class="uk-button uk-button-danger uk-button-small uk-margin-small-bottom">Fixed</a>
    <ul class="uk-margin-small-top">
        <li>Fixed stability and reliability with 5G Private Wireless Experience Kit with Integrated RAN.</li>
    </ul>
    <a class="uk-button uk-button-warning uk-button-small uk-margin-small-bottom">Known Issues</a>
    <ul class="uk-margin-small-top">
        <li>Radisys CU support for multiple SR-IOV virtual functions has not been validated.</li>
    </ul>
</div>
<div class="noteLeft">
    <p>Previous</p>
</div>
<div class="noteRight uk-margin-large-bottom">
    <a href="/ido-specs/smartedge-open_releasenotes/" title="Previous release notes">Previous release notes</a>
</div>
