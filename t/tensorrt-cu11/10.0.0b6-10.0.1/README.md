# Comparing `tmp/tensorrt-cu11-10.0.0b6.tar.gz` & `tmp/tensorrt-cu11-10.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorrt-cu11-10.0.0b6.tar", last modified: Thu Mar 14 04:45:27 2024, max compression
+gzip compressed data, was "tensorrt-cu11-10.0.1.tar", last modified: Mon Apr 15 23:42:58 2024, max compression
```

## Comparing `tensorrt-cu11-10.0.0b6.tar` & `tensorrt-cu11-10.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 04:45:27.545953 tensorrt-cu11-10.0.0b6/
--rw-r--r--   0 root         (0) root         (0)    46961 2024-03-14 04:45:27.000000 tensorrt-cu11-10.0.0b6/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1527 2024-03-14 04:45:27.545953 tensorrt-cu11-10.0.0b6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      107 2024-03-14 04:45:27.545953 tensorrt-cu11-10.0.0b6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     5822 2024-03-14 04:45:27.000000 tensorrt-cu11-10.0.0b6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 04:45:27.545953 tensorrt-cu11-10.0.0b6/tensorrt/
--rw-r--r--   0 root         (0) root         (0)      763 2024-03-14 04:45:27.000000 tensorrt-cu11-10.0.0b6/tensorrt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 04:45:27.545953 tensorrt-cu11-10.0.0b6/tensorrt_cu11.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1527 2024-03-14 04:45:27.000000 tensorrt-cu11-10.0.0b6/tensorrt_cu11.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      267 2024-03-14 04:45:27.000000 tensorrt-cu11-10.0.0b6/tensorrt_cu11.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-14 04:45:27.000000 tensorrt-cu11-10.0.0b6/tensorrt_cu11.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-03-14 04:45:27.000000 tensorrt-cu11-10.0.0b6/tensorrt_cu11.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-03-14 04:45:27.000000 tensorrt-cu11-10.0.0b6/tensorrt_cu11.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-14 04:45:27.000000 tensorrt-cu11-10.0.0b6/tensorrt_cu11.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2024-04-15 23:42:58.365238 tensorrt-cu11-10.0.1/
+-rw-rw-rw-   0        0        0    47141 2024-04-15 23:42:57.000000 tensorrt-cu11-10.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1559 2024-04-15 23:42:58.364238 tensorrt-cu11-10.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      117 2024-04-15 23:42:58.368241 tensorrt-cu11-10.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     5984 2024-04-15 23:42:57.000000 tensorrt-cu11-10.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 23:42:58.309237 tensorrt-cu11-10.0.1/tensorrt/
+-rw-rw-rw-   0        0        0      782 2024-04-15 23:42:57.000000 tensorrt-cu11-10.0.1/tensorrt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 23:42:58.362239 tensorrt-cu11-10.0.1/tensorrt_cu11.egg-info/
+-rw-rw-rw-   0        0        0     1559 2024-04-15 23:42:58.000000 tensorrt-cu11-10.0.1/tensorrt_cu11.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2024-04-15 23:42:58.000000 tensorrt-cu11-10.0.1/tensorrt_cu11.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 23:42:58.000000 tensorrt-cu11-10.0.1/tensorrt_cu11.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-15 23:42:58.000000 tensorrt-cu11-10.0.1/tensorrt_cu11.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-15 23:42:58.000000 tensorrt-cu11-10.0.1/tensorrt_cu11.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-15 23:42:58.000000 tensorrt-cu11-10.0.1/tensorrt_cu11.egg-info/zip-safe
```

### Comparing `tensorrt-cu11-10.0.0b6/LICENSE.txt` & `tensorrt-cu11-10.0.1/LICENSE.txt`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,180 +1,180 @@
-Abstract
-This document is the Software License Agreement (SLA) for NVIDIA TensorRT. This document contains specific license terms and conditions for NVIDIA TensorRT. By accepting this agreement, you agree to comply with all the terms and conditions applicable to the specific product(s) included herein.
-
-If you are receiving TensorRT under the NVIDIA Prerelease License Agreement (also known as NPLA) or under the NVIDIA Software License Agreement (previously known as the NVIDIA Tegra Software License Agreement), your use of TensorRT is governed by such applicable terms and conditions. All other uses of TensorRT are governed by the terms and conditions of the below license agreement.
-
-NVIDIA SOFTWARE LICENSE AGREEMENT
-Important: READ BEFORE DOWNLOADING, INSTALLING, COPYING OR USING THE LICENSED SOFTWARE
-This Software License Agreement ("SLA”), made and entered into as of the time and date of click through action (“Effective Date”),is a legal agreement between you and NVIDIA Corporation ("NVIDIA") and governs the use of the NVIDIA computer software and the documentation made available for use with such NVIDIA software. By downloading, installing, copying, or otherwise using the NVIDIA software and/or documentation, you agree to be bound by the terms of this SLA. If you do not agree to the terms of this SLA, do not download, install, copy or use the NVIDIA software or documentation. IF YOU ARE ENTERING INTO THIS SLAON BEHALF OF A COMPANY OR OTHER LEGAL ENTITY, YOU REPRESENT THAT YOU HAVE THE LEGAL AUTHORITY TO BIND THE ENTITY TO THIS SLA, IN WHICH CASE “YOU” WILL MEAN THE ENTITY YOU REPRESENT. IF YOU DON’T HAVE SUCH AUTHORITY, OR IF YOU DON’T ACCEPT ALL THE TERMS AND CONDITIONS OF THIS SLA, THEN NVIDIA DOES NOT AGREETO LICENSE THE LICENSED SOFTWARETO YOU, AND YOU MAY NOT DOWNLOAD, INSTALL, COPY OR USE IT.
-
-Preface
-This document is the Software License Agreement (SLA) for NVIDIA TensorRT. This document contains specific license terms and conditions for NVIDIA TensorRT. By accepting this agreement, you agree to comply with all the terms and conditions applicable to the specific product(s) included herein.
-
-If you are receiving TensorRT under the NVIDIA Prerelease License Agreement (also known as NPLA) or under the NVIDIA Software License Agreement (previously known as the NVIDIA Tegra Software License Agreement), your use of TensorRT is governed by such applicable terms and conditions. All other uses of TensorRT are governed by the terms and conditions of the below license agreement.
-
-NVIDIA SOFTWARE LICENSE AGREEMENT
-Important: READ BEFORE DOWNLOADING, INSTALLING, COPYING OR USING THE LICENSED SOFTWARE
-This Software License Agreement ("SLA”), made and entered into as of the time and date of click through action (“Effective Date”),is a legal agreement between you and NVIDIA Corporation ("NVIDIA") and governs the use of the NVIDIA computer software and the documentation made available for use with such NVIDIA software. By downloading, installing, copying, or otherwise using the NVIDIA software and/or documentation, you agree to be bound by the terms of this SLA. If you do not agree to the terms of this SLA, do not download, install, copy or use the NVIDIA software or documentation. IF YOU ARE ENTERING INTO THIS SLAON BEHALF OF A COMPANY OR OTHER LEGAL ENTITY, YOU REPRESENT THAT YOU HAVE THE LEGAL AUTHORITY TO BIND THE ENTITY TO THIS SLA, IN WHICH CASE “YOU” WILL MEAN THE ENTITY YOU REPRESENT. IF YOU DON’T HAVE SUCH AUTHORITY, OR IF YOU DON’T ACCEPT ALL THE TERMS AND CONDITIONS OF THIS SLA, THEN NVIDIA DOES NOT AGREETO LICENSE THE LICENSED SOFTWARETO YOU, AND YOU MAY NOT DOWNLOAD, INSTALL, COPY OR USE IT.
-
-1. LICENSE.
-1.1. License Grant
-Subject to the terms of the AGREEMENT, NVIDIA hereby grants you a non-exclusive, non-transferable license, without the right to sublicense (except as expressly set forth in a Supplement), during the applicable license term unless earlier terminated as provided below, to have Authorized Users install and use the Software, including modifications (if expressly permitted in a Supplement), in accordance with the Documentation. You are only licensed to activate and use Licensed Software for which you a have a valid license, even if during the download or installation you are presented with other product options. No Orders are binding on NVIDIA until accepted by NVIDIA. Your Orders are subject to the AGREEMENT.
-
-SLA Supplements: Certain Licensed Software licensed under this SLA may be subject to additional terms and conditions that will be presented to you in a Supplement for acceptance prior to the delivery of such Licensed Software under this SLA and the applicable Supplement. Licensed Software will only be delivered to you upon your acceptance of all applicable terms.
-
-1.2. Limited Purpose Licenses
-If your license is provided for one of the purposes indicated below, then notwithstanding contrary terms in License Grant or in a Supplement, such licenses are for internal use and do not include any right or license to sub-license and distribute the Licensed Software or its output in any way in any public release, however limited, and/or in any manner that provides third parties with use of or access to the Licensed Software or its functionality or output, including (but not limited to) external alpha or beta testing or development phases. Further:
-Evaluation License. You may use evaluation licenses solely for your internal evaluation of the Licensed Software for broader adoption within your Enterprise or in connection with a NVIDIA product purchase decision, and such licenses have an expiration date as indicated by NVIDIA in its sole discretion (or ninety days from the date of download if no other duration is indicated).
-Educational/Academic License. You may use educational/academic licenses solely for educational purposes and all users must be enrolled or employed by an academic institution. If you do not meet NVIDIA’s academic program requirements for educational institutions, you have no rights under this license.
-Test/Development License. You may use test/development licenses solely for your internal development, testing and/or debugging of your software applications or for interoperability testing with the Licensed Software, and such licenses have an expiration date as indicated by NVIDIA in its sole discretion (or one year from the date of download if no other duration is indicated). NVIDIA Confidential Information under the AGREEMENT includes output from Licensed Software developer tools identified as “Pro” versions, where the output reveals functionality or performance data pertinent to NVIDIA hardware or software products.
-1.3. Pre-Release Licenses
-With respect to alpha, beta, preview, and other pre-release Software and Documentation (“Pre-Release Licensed Software”) delivered to you under the AGREEMENT you acknowledge and agree that such Pre-Release Licensed Software (i) may not be fully functional, may contain errors or design flaws, and may have reduced or different security, privacy, accessibility, availability, and reliability standards relative to commercially provided NVIDIA software and documentation, and (ii) use of such Pre-Release Licensed Software may result in unexpected results, loss of data, project delays or other unpredictable damage or loss. THEREFORE, PRE-RELEASE LICENSED SOFTWARE IS NOT INTENDED FOR USE, AND SHOULD NOT BE USED, IN PRODUCTION OR BUSINESS-CRITICAL SYSTEMS. NVIDIA has no obligation to make available a commercial version of any Pre-Release Licensed Software and NVIDIA has the right to abandon development of Pre-Release Licensed Software at any time without liability.
-
-1.4. Enterprise and Contractor Usage
-You may allow your Enterprise employees and Contractors to access and use the Licensed Software pursuant to the terms of the AGREEMENT solely to perform work on your behalf, provided further that with respect to Contractors: (i) you obtain a written agreement from each Contractor which contains terms and obligations with respect to access to and use of Licensed Software no less protective of NVIDIA than those set forth in the AGREEMENT, and (ii) such Contractor’s access and use expressly excludes any sublicensing or distribution rights for the Licensed Software. You are responsible for the compliance with the terms and conditions of the AGREEMENT by your Enterprise and Contractors. Any act or omission that, if committed by you, would constitute a breach of the AGREEMENT shall be deemed to constitute a breach of the AGREEMENT if committed by your Enterprise or Contractors.
-
-1.5. Services
-Except as expressly indicated in an Order, NVIDIA is under no obligation to provide support for the Licensed Software or to provide any patches, maintenance, updates or upgrades under the AGREEMENT. Unless patches, maintenance, updates or upgrades are provided with their separate governing terms and conditions, they constitute Licensed Software licensed to you under the AGREEMENT.
-
-2. LIMITATIONS.
-2.1. License Restrictions
-Except as expressly authorized in the AGREEMENT, you agree that you will not (nor authorize third parties to): (i) copy and use Software that was licensed to you for use in one or more NVIDIA hardware products in other unlicensed products (provided that copies solely for backup purposes are allowed); (ii) reverse engineer, decompile, disassemble (except to the extent applicable laws specifically require that such activities be permitted) or attempt to derive the source code, underlying ideas, algorithm or structure of Software provided to you in object code form; (iii) sell, transfer, assign, distribute, rent, loan, lease, sublicense or otherwise make available the Licensed Software or its functionality to third parties (a) as an application services provider or service bureau, (b) by operating hosted/virtual system environments, (c) by hosting, time sharing or providing any other type of services, or (d) otherwise by means of the internet; (iv) modify, translate or otherwise create any derivative works of any Licensed Software; (v) remove, alter, cover or obscure any proprietary notice that appears on or with the Licensed Software or any copies thereof; (vi) use the Licensed Software, or allow its use, transfer, transmission or export in violation of any applicable export control laws, rules or regulations; (vii) distribute, permit access to, or sublicense the Licensed Software as a stand-alone product; (viii) bypass, disable, circumvent or remove any form of copy protection, encryption, security or digital rights management or authentication mechanism used by NVIDIA in connection with the Licensed Software, or use the Licensed Software together with any authorization code, serial number, or other copy protection device not supplied by NVIDIA directly or through an authorized reseller; (ix) use the Licensed Software for the purpose of developing competing products or technologies or assisting a third party in such activities; (x) use the Licensed Software with any system or application where the use or failure of such system or application can reasonably be expected to threaten or result in personal injury, death, or catastrophic loss including, without limitation, use in connection with any nuclear, avionics, navigation, military, medical, life support or other life critical application (“Critical Applications”), unless the parties have entered into a Critical Applications agreement; (xi) distribute any modification or derivative work you make to the Licensed Software under or by reference to the same name as used by NVIDIA; or (xii) use the Licensed Software in any manner that would cause the Licensed Software to become subject to an Open Source License. Nothing in the AGREEMENT shall be construed to give you a right to use, or otherwise obtain access to, any source code from which the Software or any portion thereof is compiled or interpreted. You acknowledge that NVIDIA does not design, test, manufacture or certify the Licensed Software for use in the context of a Critical Application and NVIDIA shall not be liable to you or any third party, in whole or in part, for any claims or damages arising from such use. You agree to defend, indemnify and hold harmless NVIDIA and its Affiliates, and their respective employees, contractors, agents, officers and directors, from and against any and all claims, damages, obligations, losses, liabilities, costs or debt, fines, restitutions and expenses (including but not limited to attorney’s fees and costs incident to establishing the right of indemnification) arising out of or related to you and your Enterprise, and their respective employees, contractors, agents, distributors, resellers, end users, officers and directors use of Licensed Software outside of the scope of the AGREEMENT or any other breach of the terms of the AGREEMENT.
-
-2.2. Third Party License Obligations
-You acknowledge and agree that the Licensed Software may include or incorporate third party technology (collectively “Third Party Components”), which is provided for use in or with the Software and not otherwise used separately. If the Licensed Software includes or incorporates Third Party Components, then the third-party pass-through terms and conditions (“Third Party Terms”) for the particular Third Party Component will be bundled with the Software or otherwise made available online as indicated by NVIDIA and will be incorporated by reference into the AGREEMENT. In the event of any conflict between the terms in the AGREEMENT and the Third Party Terms, the Third Party Terms shall govern. Copyright to Third Party Components are held by the copyright holders indicated in the copyright notices indicated in the Third Party Terms.
-
-Audio/Video Encoders and Decoders: You acknowledge and agree that it is your sole responsibility to obtain any additional third party licenses required to make, have made, use, have used, sell, import, and offer for sale your products or services that include or incorporate any Third Party Components and content relating to audio and/or video encoders and decoders from, including but not limited to, Microsoft, Thomson, Fraunhofer IIS, Sisvel S.p.A., MPEG-LA, and Coding Technologies as NVIDIA does not grant to you under the AGREEMENT any necessary patent or other rights with respect to audio and/or video encoders and decoders.
-
-2.3. Limited Rights
-Your rights in the Licensed Software are limited to those expressly granted under the AGREEMENT and no other licenses are granted whether by implication, estoppel or otherwise. NVIDIA reserves all rights, title and interest in and to the Licensed Software not expressly granted under the AGREEMENT.
-
-3. CONFIDENTIALITY
-Neither party will use the other party’s Confidential Information, except as necessary for the performance of the AGREEMENT, nor will either party disclose such Confidential Information to any third party, except to personnel of NVIDIA and its Affiliates, you, your Enterprise, your Enterprise Contractors, and each party’s legal and financial advisors that have a need to know such Confidential Information for the performance of the AGREEMENT, provided that each such personnel, employee and Contractor is subject to a written agreement that includes confidentiality obligations consistent with those set forth herein. Each party will use all reasonable efforts to maintain the confidentiality of all of the other party’s Confidential Information in its possession or control, but in no event less than the efforts that it ordinarily uses with respect to its own Confidential Information of similar nature and importance. The foregoing obligations will not restrict either party from disclosing the other party’s Confidential Information or the terms and conditions of the AGREEMENT as required under applicable securities regulations or pursuant to the order or requirement of a court, administrative agency, or other governmental body, provided that the party required to make such disclosure (i) gives reasonable notice to the other party to enable it to contest such order or requirement prior to its disclosure (whether through protective orders or otherwise), (ii) uses reasonable effort to obtain confidential treatment or similar protection to the fullest extent possible to avoid such public disclosure, and (iii) discloses only the minimum amount of information necessary to comply with such requirements.
-
-4. OWNERSHIP
-You are not obligated to disclose to NVIDIA any modifications that you, your Enterprise or your Contractors make to the Licensed Software as permitted under the AGREEMENT. As between the parties, all modifications are owned by NVIDIA and licensed to you under the AGREEMENT unless otherwise expressly provided in a Supplement. The Licensed Software and all modifications owned by NVIDIA, and the respective Intellectual Property Rights therein, are and will remain the sole and exclusive property of NVIDIA or its licensors, whether the Licensed Software is separate from or combined with any other products or materials. You shall not engage in any act or omission that would impair NVIDIA’s and/or its licensors’ Intellectual Property Rights in the Licensed Software or any other materials, information, processes or subject matter proprietary to NVIDIA. NVIDIA’s licensors are intended third party beneficiaries with the right to enforce provisions of the AGREEMENT with respect to their Confidential Information and/or Intellectual Property Rights.
-
-5. FEEDBACK
-You have no obligation to provide Feedback to NVIDIA. However, NVIDIA and/or its Affiliates may use and include any Feedback that you provide to improve the Licensed Software or other NVIDIA products, technologies or materials. Accordingly, if you provide Feedback, you agree that NVIDIA and/or its Affiliates, at their option, may, and may permit their licensees, to make, have made, use, have used, reproduce, license, distribute and otherwise commercialize the Feedback in the Licensed Software or in other NVIDIA products, technologies or materials without the payment of any royalties or fees to you. All Feedback becomes the sole property of NVIDIA and may be used in any manner NVIDIA sees fit, and you hereby assign to NVIDIA all of your right, title and interest in and to any Feedback. NVIDIA has no obligation to respond to Feedback or to incorporate Feedback into the Licensed Software.
-
-6. NO WARRANTIES
-THE LICENSED SOFTWARE AND ANY OTHER CONFIDENTIAL INFORMATION AND/OR SERVICES ARE PROVIDED BY NVIDIA “AS IS” AND “WITH ALL FAULTS,” AND NVIDIA EXPRESSLY DISCLAIMS ALL OTHER WARRANTIES OF ANY KIND OR NATURE, WHETHER EXPRESS, IMPLIED OR STATUTORY, INCLUDING, BUT NOT LIMITED TO, ANY WARRANTIES OF OPERABILITY, CONDITION, VALUE, ACCURACY OF DATA, OR QUALITY, AS WELL AS ANY WARRANTIES OF MERCHANTABILITY, SYSTEM INTEGRATION, WORKMANSHIP, SUITABILITY, FITNESS FOR A PARTICULAR PURPOSE, NON-INFRINGEMENT, OR THE ABSENCE OF ANY DEFECTS THEREIN, WHETHER LATENT OR PATENT. NO WARRANTY IS MADE BY NVIDIA ON THE BASIS OF TRADE USAGE, COURSE OF DEALING OR COURSE OF TRADE. NVIDIA DOES NOT WARRANT THAT THE LICENSED SOFTWARE OR ANY OTHER CONFIDENTIAL INFORMATION AND/OR SERVICES PROVIDED BY NVIDIA UNDER THE AGREEMENT WILL MEET YOUR REQUIREMENTS OR THAT THE OPERATION THEREOF WILL BE UNINTERRUPTED OR ERROR-FREE, OR THAT ALL ERRORS WILL BE CORRECTED. YOU ACKNOWLEDGE THAT NVIDIA’S OBLIGATIONS UNDER THE AGREEMENT ARE FOR THE BENEFIT OF YOU ONLY. Nothing in this warranty section affects any statutory rights of consumers or other recipients to the extent that they cannot be waived or limited by contract under applicable law.
-
-7. LIMITATION OF LIABILITY
-TO THE MAXIMUM EXTENT PERMITTED BY LAW, NVIDIA OR ITS LICENSORS SHALL NOT BE LIABLE FOR ANY SPECIAL, INCIDENTAL, PUNITIVE OR CONSEQUENTIAL DAMAGES, OR ANY LOST PROFITS, LOSS OF USE, LOSS OF DATA OR LOSS OF GOODWILL, OR THE COSTS OF PROCURING SUBSTITUTE PRODUCTS, ARISING OUT OF OR IN CONNECTION WITH THE AGREEMENT OR THE USE OR PERFORMANCE OF THE LICENSED SOFTWARE AND ANY OTHER CONFIDENTIAL INFORMATION AND/OR SERVICES PROVIDED BY NVIDIA UNDER THE AGREEMENT, WHETHER SUCH LIABILITY ARISES FROM ANY CLAIM BASED UPON BREACH OF CONTRACT, BREACH OF WARRANTY, TORT (INCLUDING NEGLIGENCE), PRODUCT LIABILITY OR ANY OTHER CAUSE OF ACTION OR THEORY OF LIABILITY. IN NO EVENT WILL NVIDIA’S TOTAL CUMULATIVE LIABILITY UNDER OR ARISING OUT OF THE AGREEMENT EXCEED THE NET AMOUNTS RECEIVED BY NVIDIA FOR YOUR USE OF THE PARTICULAR LICENSED SOFTWARE DURING THE TWELVE (12) MONTHS BEFORE THE LIABILITY AROSE (or up to US$10.00 if you acquired the Licensed Software for no charge). THE NATURE OF THE LIABILITY, THE NUMBER OF CLAIMS OR SUITS OR THE NUMBER OF PARTIES WITHIN YOUR ENTERPRISE THAT ACCEPTED THE TERMS OF THE AGREEMENT SHALL NOT ENLARGE OR EXTEND THIS LIMIT. THE FOREGOING LIMITATIONS SHALL APPLY REGARDLESS OF WHETHER NVIDIA OR ITS LICENSORS HAVE BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES AND REGARDLESS OF WHETHER ANY REMEDY FAILS ITS ESSENTIAL PURPOSE. The disclaimers, exclusions and limitations of liability set forth in the AGREEMENT form an essential basis of the bargain between the parties, and, absent any such disclaimers, exclusions or limitations of liability, the provisions of the AGREEMENT, including, without limitation, the economic terms, would be substantially different.
-
-8. TERM AND TERMINATION.
-8.1. AGREEMENT, Licenses and Services
-This SLA shall become effective upon the Effective Date, each Supplement upon their acceptance, and both this SLA and Supplements shall continue in effect until your last access or use of the Licensed Software and/or services hereunder, unless earlier terminated as provided in this “Term and Termination” section. Each Licensed Software license ends at the earlier of (a) the expiration of the applicable license term, or (b) termination of such license or the AGREEMENT. Each service ends at the earlier of (x) the expiration of the applicable service term, (y) termination of such service or the AGREEMENT, or (z) expiration or termination of the associated license and no credit or refund will be provided upon the expiration or termination of the associated license for any service fees paid.
-
-8.2. Termination and Effect of Expiration or Termination
-NVIDIA may terminate the AGREEMENT in whole or in part: (i) if you breach any term of the AGREEMENT and fail to cure such breach within thirty (30) days following notice thereof from NVIDIA (or immediately if you violate NVIDIA’s Intellectual Property Rights); (ii) if you become the subject of a voluntary or involuntary petition in bankruptcy or any proceeding relating to insolvency, receivership, liquidation or composition for the benefit of creditors, if that petition or proceeding is not dismissed with prejudice within sixty (60) days after filing, or if you cease to do business; or (iii) if you commence or participate in any legal proceeding against NVIDIA, with respect to the Licensed Software that is the subject of the proceeding during the pendency of such legal proceeding. If you or your authorized NVIDIA reseller fail to pay license fees or service fees when due then NVIDIA may, in its sole discretion, suspend or terminate your license grants, services and any other rights provided under the AGREEMENT for the affected Licensed Software, in addition to any other remedies NVIDIA may have at law or equity. Upon any expiration or termination of the AGREEMENT, a license or a service provided hereunder, (a) any amounts owed to NVIDIA become immediately due and payable, (b) you must promptly discontinue use of the affected Licensed Software and/or service, and (c) you must promptly destroy or return to NVIDIA all copies of the affected Licensed Software and all portions thereof in your possession or control, and each party will promptly destroy or return to the other all of the other party’s Confidential Information within its possession or control. Upon written request, you will certify in writing that you have complied with your obligations under this section. Upon expiration or termination of the AGREEMENT all provisions survive except for the license grant provisions.
-
-9. CONSENT TO COLLECTION AND USE OF INFORMATION.
-You hereby agree and acknowledge that the Software may access, collect non-personally identifiable information about your Enterprise computer systems in order to properly optimize such systems for use with the Software. To the extent that you use the Software, you hereby consent to all of the foregoing, and represent and warrant that you have the right to grant such consent. In addition, you agree that you are solely responsible for maintaining appropriate data backups and system restore points for your Enterprise systems, and that NVIDIA will have no responsibility for any damage or loss to such systems (including loss of data or access) arising from or relating to (a) any changes to the configuration, application settings, environment variables, registry, drivers, BIOS, or other attributes of the systems (or any part of such systems) initiated through the Software; or (b) installation of any Software or third party software patches initiated through the Software. In certain systems you may change your system update preferences by unchecking "Automatically check for updates" in the "Preferences" tab of the control panel for the Software.
-
-In connection with the receipt of the Licensed Software or services you may receive access to links to third party websites and services and the availability of those links does not imply any endorsement by NVIDIA. NVIDIA encourages you to review the privacy statements on those sites and services that you choose to visit so that you can understand how they may collect, use and share personal information of individuals. NVIDIA is not responsible or liable for: (i) the availability or accuracy of such links; or (ii) the products, services or information available on or through such links; or (iii) the privacy statements or practices of sites and services controlled by other companies or organizations.
-
-To the extent that you or members of your Enterprise provide to NVIDIA during registration or otherwise personal information, you acknowledge that such information will be collected, used and disclosed by NVIDIA in accordance with NVIDIA's privacy policy, available at URL http://www.nvidia.com/object/privacy_policy.html.
-
-10. GENERAL.
-This SLA, any Supplements incorporated hereto, and Orders constitute the entire agreement of the parties with respect to the subject matter hereto and supersede all prior negotiations, conversations, or discussions between the parties relating to the subject matter hereto, oral or written, and all past dealings or industry custom. Any additional and/or conflicting terms and conditions on purchase order(s) or any other documents issued by you are null, void, and invalid. Any amendment or waiver under the AGREEMENT must be in writing and signed by representatives of both parties.
-
-The AGREEMENT and the rights and obligations thereunder may not be assigned by you, in whole or in part, including by merger, consolidation, dissolution, operation of law, or any other manner, without written consent of NVIDIA, and any purported assignment in violation of this provision shall be void and of no effect. NVIDIA may assign, delegate or transfer the AGREEMENT and its rights and obligations hereunder, and if to a non-Affiliate you will be notified.
-
-Each party acknowledges and agrees that the other is an independent contractor in the performance of the AGREEMENT, and each party is solely responsible for all of its employees, agents, contractors, and labor costs and expenses arising in connection therewith. The parties are not partners, joint ventures or otherwise affiliated, and neither has any authority to make any statements, representations or commitments of any kind to bind the other party without prior written consent.
-
-Neither party will be responsible for any failure or delay in its performance under the AGREEMENT (except for any payment obligations) to the extent due to causes beyond its reasonable control for so long as such force majeure event continues in effect.
-
-The AGREEMENT will be governed by and construed under the laws of the State of Delaware and the United States without regard to the conflicts of law provisions thereof and without regard to the United Nations Convention on Contracts for the International Sale of Goods. The parties consent to the personal jurisdiction of the federal and state courts located in Santa Clara County, California. You acknowledge and agree that a breach of any of your promises or agreements contained in the AGREEMENT may result in irreparable and continuing injury to NVIDIA for which monetary damages may not be an adequate remedy and therefore NVIDIA is entitled to seek injunctive relief as well as such other and further relief as may be appropriate. If any court of competent jurisdiction determines that any provision of the AGREEMENT is illegal, invalid or unenforceable, the remaining provisions will remain in full force and effect. Unless otherwise specified, remedies are cumulative.
-
-The Licensed Software has been developed entirely at private expense and is “commercial items” consisting of “commercial computer software” and “commercial computer software documentation” provided with RESTRICTED RIGHTS. Use, duplication or disclosure by the U.S. Government or a U.S. Government subcontractor is subject to the restrictions set forth in the AGREEMENT pursuant to DFARS 227.7202-3(a) or as set forth in subparagraphs (c)(1) and (2) of the Commercial Computer Software - Restricted Rights clause at FAR 52.227-19, as applicable. Contractor/manufacturer is NVIDIA, 2701 San Tomas Expressway, Santa Clara, CA 95050.
-
-You acknowledge that the Licensed Software described under the AGREEMENT is subject to export control under the U.S. Export Administration Regulations (EAR) and economic sanctions regulations administered by the U.S. Department of Treasury’s Office of Foreign Assets Control (OFAC). Therefore, you may not export, reexport or transfer in-country the Licensed Software without first obtaining any license or other approval that may be required by BIS and/or OFAC. You are responsible for any violation of the U.S. or other applicable export control or economic sanctions laws, regulations and requirements related to the Licensed Software. By accepting this SLA, you confirm that you are not a resident or citizen of any country currently embargoed by the U.S. and that you are not otherwise prohibited from receiving the Licensed Software.
-
-Any notice delivered by NVIDIA to you under the AGREEMENT will be delivered via mail, email or fax. Please direct your legal notices or other correspondence to NVIDIA Corporation, 2701 San Tomas Expressway, Santa Clara, California 95050, United States of America, Attention: Legal Department.
-
-11. GLOSSARY OF TERMS
-Certain capitalized terms, if not otherwise defined elsewhere in this SLA, shall have the meanings set forth below:
-“Affiliate”
-“Affiliate” means any legal entity that Owns, is Owned by, or is commonly Owned with a party. “Own” means having more than 50% ownership or the right to direct the management of the entity.
-“AGREEMENT”
-“AGREEMENT” means this SLA and all associated Supplements entered by the parties referencing this SLA.
-“Authorized Users”
-“Authorized Users” means your Enterprise individual employees and any of your Enterprise’s Contractors, subject to the terms of the “Enterprise and Contractors Usage” section.
-“Confidential Information”
-“Confidential Information” means the Licensed Software (unless made publicly available by NVIDIA without confidentiality obligations), and any NVIDIA business, marketing, pricing, research and development, know-how, technical, scientific, financial status, proposed new products or other information disclosed by NVIDIA to you which, at the time of disclosure, is designated in writing as confidential or proprietary (or like written designation), or orally identified as confidential or proprietary or is otherwise reasonably identifiable by parties exercising reasonable business judgment, as confidential. Confidential Information does not and will not include information that: (i) is or becomes generally known to the public through no fault of or breach of the AGREEMENT by the receiving party; (ii) is rightfully known by the receiving party at the time of disclosure without an obligation of confidentiality; (iii) is independently developed by the receiving party without use of the disclosing party’s Confidential Information; or (iv) is rightfully obtained by the receiving party from a third party without restriction on use or disclosure.
-“Contractor”
-“Contractor” means an individual who works primarily for your Enterprise on a contractor basis from your secure network. means an individual who works primarily for your Enterprise on a contractor basis from your secure network.
-“Documentation”
-“Documentation” means the NVIDIA documentation made available for use with the Software, including (without limitation) user manuals, datasheets, operations instructions, installation guides, release notes and other materials provided to you under the AGREEMENT.
-“Enterprise”
-“Enterprise” means you or any company or legal entity for which you accepted the terms of this SLA, and their subsidiaries of which your company or legal entity owns more than fifty percent (50%) of the issued and outstanding equity.
-“Feedback”
-“Feedback” means any and all suggestions, feature requests, comments or other feedback regarding the Licensed Software, including possible enhancements or modifications thereto.
-“Intellectual Property Rights”
-“Intellectual Property Rights” means all patent, copyright, trademark, trade secret, trade dress, trade names, utility models, mask work, moral rights, rights of attribution or integrity service marks, master recording and music publishing rights, performance rights, author’s rights, database rights, registered design rights and any applications for the protection or registration of these rights, or other intellectual or industrial property rights or proprietary rights, howsoever arising and in whatever media, whether now known or hereafter devised, whether or not registered, (including all claims and causes of action for infringement, misappropriation or violation and all rights in any registrations and renewals), worldwide and whether existing now or in the future.
-“Licensed Software”
-“Licensed Software” means Software, Documentation and all modifications owned by NVIDIA.
-“Open Source License”
-“Open Source License” includes, without limitation, a software license that requires as a condition of use, modification, and/or distribution of such software that the Software be (i) disclosed or distributed in source code form; (ii) be licensed for the purpose of making derivative works; or (iii) be redistributable at no charge.
-“Order”
-“Order” means a purchase order issued by you, a signed purchase agreement with you, or other ordering document issued by you to NVIDIA or a NVIDIA authorized reseller (including any on-line acceptance process) that references and incorporates the AGREEMENT and is accepted by NVIDIA.
-“Software”
-“Software” means the NVIDIA software programs licensed to you under the AGREEMENT including, without limitation, libraries, sample code, utility programs and programming code.
-“Supplement”
-“Supplement” means the additional terms and conditions beyond those stated in this SLA that apply to certain Licensed Software licensed hereunder.
-12. TensorRT SUPPLEMENT TO SOFTWARE LICENSE AGREEMENT
-TensorRT SUPPLEMENT TO SOFTWARE LICENSE AGREEMENT
-The terms set forth in this TensorRT Supplement (“Supplement”) govern your use of the NVIDIA GPU inference engine (the “TensorRT Licensed Software”) under the terms of your software license agreement (“SLA”) as modified by this Supplement. This Supplement is an exhibit to the SLA and is hereby incorporated as an integral part thereto. Capitalized terms used but not defined herein shall have the meaning assigned to them in the SLA. In the event of conflict between the terms in this Supplement and the terms in the SLA, this Supplement shall control.
-
-12.1. TensorRT DISTRIBUTION
-Subject to the terms of the SLA and this Supplement, NVIDIA hereby grants you a non-exclusive, nontransferable license during the applicable license term unless earlier terminated pursuant to the SLA, to distribute the libnvinfer and libnvinfer_plugin libraries when delivered to you as part of the TensorRT Licensed Software in source code form or binary form (but not when provided to you as part of a hardware product), subject to the following: such distribution is solely in binary form to your licensees (“Customers”) only as a component of your own software products having additional material functionality beyond the TensorRT Licensed Software (each, a “Licensee Application"). Subject to the terms and conditions of the SLA and this Supplement, you may further authorize Customers to redistribute the libnvinfer and libnvinfer_plugin libraries as incorporated into a Licensee Application, solely in binary form, provided, however, that you shall require in your agreements with your Customers that their distributions be on terms at least as restrictive as those applicable for your use of such TensorRT Licensed Software within a Licensee Application. The expiration or termination of your licenses to the above described TensorRT Licensed Software under the SLA and this Supplement will not affect rights previously granted by you to recipients that were in compliance with the SLA and this Supplement.
-
-In addition to the rights above, for parties that are developing software intended solely for use on Jetson development kits or Jetson modules and running Linux for Tegra software the following shall apply: TensorRT Licensed Software licensed hereunder may be distributed in its entirety, as provided by NVIDIA and without separation of its components, for you and/or your licensees to create software development kits for use only on the Jetson platform and running Linux for Tegra software. You shall require in your agreements with your licensees that their distributions be on terms at least as restrictive as those applicable for your distribution of TensorRT Licensed Software as described in this Section 1.
-
-In addition to the rights above, for parties that are developing software intended solely for use on Jetson development kits or Jetson modules and running Linux for Tegra software the following shall apply: TensorRT Licensed Software licensed hereunder may be distributed in its entirety, as provided by NVIDIA and without separation of its components, for you and/or your licensees to create software development kits for use only on the Jetson platform and running Linux for Tegra software. You shall require in your agreements with your licensees that their distributions be on terms at least as restrictive as those applicable for your distribution of TensorRT Licensed Software as described in this Section 1.
-
-12.2. LICENSE DURATION
-Each TensorRT Licensed Software is licensed to you for an initial duration of one year starting from the date of delivery or download. The licenses granted will automatically renew for successive one year periods, provided that NVIDIA reserves the right to terminate licenses upon ninety days (90) days written notice to you prior to the commencement of a renewal year in addition to the termination rights set forth in the SLA.
-
-12.3. EXPIRATION OF TERMINATION OF THIS SUPPLEMENT
-Your failure to comply with the terms of this Supplement is ground for termination for breach by NVIDIA under the SLA. This Supplement will automatically expire or terminate upon the expiration or termination of your rights to TensorRT Licensed Software under the SLA or this Supplement.
-
-Notices
-Notice
-This document is provided for information purposes only and shall not be regarded as a warranty of a certain functionality, condition, or quality of a product. NVIDIA Corporation (“NVIDIA”) makes no representations or warranties, expressed or implied, as to the accuracy or completeness of the information contained in this document and assumes no responsibility for any errors contained herein. NVIDIA shall have no liability for the consequences or use of such information or for any infringement of patents or other rights of third parties that may result from its use. This document is not a commitment to develop, release, or deliver any Material (defined below), code, or functionality.
-
-NVIDIA reserves the right to make corrections, modifications, enhancements, improvements, and any other changes to this document, at any time without notice.
-
-Customer should obtain the latest relevant information before placing orders and should verify that such information is current and complete.
-
-NVIDIA products are sold subject to the NVIDIA standard terms and conditions of sale supplied at the time of order acknowledgement, unless otherwise agreed in an individual sales agreement signed by authorized representatives of NVIDIA and customer (“Terms of Sale”). NVIDIA hereby expressly objects to applying any customer general terms and conditions with regards to the purchase of the NVIDIA product referenced in this document. No contractual obligations are formed either directly or indirectly by this document.
-
-NVIDIA products are not designed, authorized, or warranted to be suitable for use in medical, military, aircraft, space, or life support equipment, nor in applications where failure or malfunction of the NVIDIA product can reasonably be expected to result in personal injury, death, or property or environmental damage. NVIDIA accepts no liability for inclusion and/or use of NVIDIA products in such equipment or applications and therefore such inclusion and/or use is at customer’s own risk.
-
-NVIDIA makes no representation or warranty that products based on this document will be suitable for any specified use. Testing of all parameters of each product is not necessarily performed by NVIDIA. It is customer’s sole responsibility to evaluate and determine the applicability of any information contained in this document, ensure the product is suitable and fit for the application planned by customer, and perform the necessary testing for the application in order to avoid a default of the application or the product. Weaknesses in customer’s product designs may affect the quality and reliability of the NVIDIA product and may result in additional or different conditions and/or requirements beyond those contained in this document. NVIDIA accepts no liability related to any default, damage, costs, or problem which may be based on or attributable to: (i) the use of the NVIDIA product in any manner that is contrary to this document or (ii) customer product designs.
-
-No license, either expressed or implied, is granted under any NVIDIA patent right, copyright, or other NVIDIA intellectual property right under this document. Information published by NVIDIA regarding third-party products or services does not constitute a license from NVIDIA to use such products or services or a warranty or endorsement thereof. Use of such information may require a license from a third party under the patents or other intellectual property rights of the third party, or a license from NVIDIA under the patents or other intellectual property rights of NVIDIA.
-
-Reproduction of information in this document is permissible only if approved in advance by NVIDIA in writing, reproduced without alteration and in full compliance with all applicable export laws and regulations, and accompanied by all associated conditions, limitations, and notices.
-
-THIS DOCUMENT AND ALL NVIDIA DESIGN SPECIFICATIONS, REFERENCE BOARDS, FILES, DRAWINGS, DIAGNOSTICS, LISTS, AND OTHER DOCUMENTS (TOGETHER AND SEPARATELY, “MATERIALS”) ARE BEING PROVIDED “AS IS.” NVIDIA MAKES NO WARRANTIES, EXPRESSED, IMPLIED, STATUTORY, OR OTHERWISE WITH RESPECT TO THE MATERIALS, AND EXPRESSLY DISCLAIMS ALL IMPLIED WARRANTIES OF NONINFRINGEMENT, MERCHANTABILITY, AND FITNESS FOR A PARTICULAR PURPOSE. TO THE EXTENT NOT PROHIBITED BY LAW, IN NO EVENT WILL NVIDIA BE LIABLE FOR ANY DAMAGES, INCLUDING WITHOUT LIMITATION ANY DIRECT, INDIRECT, SPECIAL, INCIDENTAL, PUNITIVE, OR CONSEQUENTIAL DAMAGES, HOWEVER CAUSED AND REGARDLESS OF THE THEORY OF LIABILITY, ARISING OUT OF ANY USE OF THIS DOCUMENT, EVEN IF NVIDIA HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES. Notwithstanding any damages that customer might incur for any reason whatsoever, NVIDIA’s aggregate and cumulative liability towards customer for the products described herein shall be limited in accordance with the Terms of Sale for the product.
-
-VESA DisplayPort
-DisplayPort and DisplayPort Compliance Logo, DisplayPort Compliance Logo for Dual-mode Sources, and DisplayPort Compliance Logo for Active Cables are trademarks owned by the Video Electronics Standards Association in the United States and other countries.
-
-HDMI
-HDMI, the HDMI logo, and High-Definition Multimedia Interface are trademarks or registered trademarks of HDMI Licensing LLC.
-
-ARM
-ARM, AMBA and ARM Powered are registered trademarks of ARM Limited. Cortex, MPCore and Mali are trademarks of ARM Limited. All other brands or product names are the property of their respective holders. "ARM" is used to represent ARM Holdings plc; its operating company ARM Limited; and the regional subsidiaries ARM Inc.; ARM KK; ARM Korea Limited.; ARM Taiwan Limited; ARM France SAS; ARM Consulting (Shanghai) Co. Ltd.; ARM Germany GmbH; ARM Embedded Technologies Pvt. Ltd.; ARM Norway, AS and ARM Sweden AB.
-
-OpenCL
-OpenCL is a trademark of Apple Inc. used under license to the Khronos Group Inc.
-
-Trademarks
-NVIDIA, the NVIDIA logo, and cuBLAS, CUDA, CUDA Toolkit, cuDNN, DALI, DIGITS, DGX, DGX-1, DGX-2, DGX Station, DLProf, GPU, JetPack, Jetson, Kepler, Maxwell, NCCL, Nsight Compute, Nsight Systems, NVCaffe, NVIDIA Ampere GPU architecture, NVIDIA Deep Learning SDK, NVIDIA Developer Program, NVIDIA GPU Cloud, NVLink, NVSHMEM, PerfWorks, Pascal, SDK Manager, T4, Tegra, TensorRT, TensorRT Inference Server, Tesla, TF-TRT, Triton Inference Server, Turing, and Volta are trademarks and/or registered trademarks of NVIDIA Corporation in the United States and other countries. Other company and product names may be trademarks of the respective companies with which they are associated.
-
-Copyright
-© 2021 NVIDIA Corporation. All rights reserved.
+Abstract
+This document is the Software License Agreement (SLA) for NVIDIA TensorRT. This document contains specific license terms and conditions for NVIDIA TensorRT. By accepting this agreement, you agree to comply with all the terms and conditions applicable to the specific product(s) included herein.
+
+If you are receiving TensorRT under the NVIDIA Prerelease License Agreement (also known as NPLA) or under the NVIDIA Software License Agreement (previously known as the NVIDIA Tegra Software License Agreement), your use of TensorRT is governed by such applicable terms and conditions. All other uses of TensorRT are governed by the terms and conditions of the below license agreement.
+
+NVIDIA SOFTWARE LICENSE AGREEMENT
+Important: READ BEFORE DOWNLOADING, INSTALLING, COPYING OR USING THE LICENSED SOFTWARE
+This Software License Agreement ("SLA”), made and entered into as of the time and date of click through action (“Effective Date”),is a legal agreement between you and NVIDIA Corporation ("NVIDIA") and governs the use of the NVIDIA computer software and the documentation made available for use with such NVIDIA software. By downloading, installing, copying, or otherwise using the NVIDIA software and/or documentation, you agree to be bound by the terms of this SLA. If you do not agree to the terms of this SLA, do not download, install, copy or use the NVIDIA software or documentation. IF YOU ARE ENTERING INTO THIS SLAON BEHALF OF A COMPANY OR OTHER LEGAL ENTITY, YOU REPRESENT THAT YOU HAVE THE LEGAL AUTHORITY TO BIND THE ENTITY TO THIS SLA, IN WHICH CASE “YOU” WILL MEAN THE ENTITY YOU REPRESENT. IF YOU DON’T HAVE SUCH AUTHORITY, OR IF YOU DON’T ACCEPT ALL THE TERMS AND CONDITIONS OF THIS SLA, THEN NVIDIA DOES NOT AGREETO LICENSE THE LICENSED SOFTWARETO YOU, AND YOU MAY NOT DOWNLOAD, INSTALL, COPY OR USE IT.
+
+Preface
+This document is the Software License Agreement (SLA) for NVIDIA TensorRT. This document contains specific license terms and conditions for NVIDIA TensorRT. By accepting this agreement, you agree to comply with all the terms and conditions applicable to the specific product(s) included herein.
+
+If you are receiving TensorRT under the NVIDIA Prerelease License Agreement (also known as NPLA) or under the NVIDIA Software License Agreement (previously known as the NVIDIA Tegra Software License Agreement), your use of TensorRT is governed by such applicable terms and conditions. All other uses of TensorRT are governed by the terms and conditions of the below license agreement.
+
+NVIDIA SOFTWARE LICENSE AGREEMENT
+Important: READ BEFORE DOWNLOADING, INSTALLING, COPYING OR USING THE LICENSED SOFTWARE
+This Software License Agreement ("SLA”), made and entered into as of the time and date of click through action (“Effective Date”),is a legal agreement between you and NVIDIA Corporation ("NVIDIA") and governs the use of the NVIDIA computer software and the documentation made available for use with such NVIDIA software. By downloading, installing, copying, or otherwise using the NVIDIA software and/or documentation, you agree to be bound by the terms of this SLA. If you do not agree to the terms of this SLA, do not download, install, copy or use the NVIDIA software or documentation. IF YOU ARE ENTERING INTO THIS SLAON BEHALF OF A COMPANY OR OTHER LEGAL ENTITY, YOU REPRESENT THAT YOU HAVE THE LEGAL AUTHORITY TO BIND THE ENTITY TO THIS SLA, IN WHICH CASE “YOU” WILL MEAN THE ENTITY YOU REPRESENT. IF YOU DON’T HAVE SUCH AUTHORITY, OR IF YOU DON’T ACCEPT ALL THE TERMS AND CONDITIONS OF THIS SLA, THEN NVIDIA DOES NOT AGREETO LICENSE THE LICENSED SOFTWARETO YOU, AND YOU MAY NOT DOWNLOAD, INSTALL, COPY OR USE IT.
+
+1. LICENSE.
+1.1. License Grant
+Subject to the terms of the AGREEMENT, NVIDIA hereby grants you a non-exclusive, non-transferable license, without the right to sublicense (except as expressly set forth in a Supplement), during the applicable license term unless earlier terminated as provided below, to have Authorized Users install and use the Software, including modifications (if expressly permitted in a Supplement), in accordance with the Documentation. You are only licensed to activate and use Licensed Software for which you a have a valid license, even if during the download or installation you are presented with other product options. No Orders are binding on NVIDIA until accepted by NVIDIA. Your Orders are subject to the AGREEMENT.
+
+SLA Supplements: Certain Licensed Software licensed under this SLA may be subject to additional terms and conditions that will be presented to you in a Supplement for acceptance prior to the delivery of such Licensed Software under this SLA and the applicable Supplement. Licensed Software will only be delivered to you upon your acceptance of all applicable terms.
+
+1.2. Limited Purpose Licenses
+If your license is provided for one of the purposes indicated below, then notwithstanding contrary terms in License Grant or in a Supplement, such licenses are for internal use and do not include any right or license to sub-license and distribute the Licensed Software or its output in any way in any public release, however limited, and/or in any manner that provides third parties with use of or access to the Licensed Software or its functionality or output, including (but not limited to) external alpha or beta testing or development phases. Further:
+Evaluation License. You may use evaluation licenses solely for your internal evaluation of the Licensed Software for broader adoption within your Enterprise or in connection with a NVIDIA product purchase decision, and such licenses have an expiration date as indicated by NVIDIA in its sole discretion (or ninety days from the date of download if no other duration is indicated).
+Educational/Academic License. You may use educational/academic licenses solely for educational purposes and all users must be enrolled or employed by an academic institution. If you do not meet NVIDIA’s academic program requirements for educational institutions, you have no rights under this license.
+Test/Development License. You may use test/development licenses solely for your internal development, testing and/or debugging of your software applications or for interoperability testing with the Licensed Software, and such licenses have an expiration date as indicated by NVIDIA in its sole discretion (or one year from the date of download if no other duration is indicated). NVIDIA Confidential Information under the AGREEMENT includes output from Licensed Software developer tools identified as “Pro” versions, where the output reveals functionality or performance data pertinent to NVIDIA hardware or software products.
+1.3. Pre-Release Licenses
+With respect to alpha, beta, preview, and other pre-release Software and Documentation (“Pre-Release Licensed Software”) delivered to you under the AGREEMENT you acknowledge and agree that such Pre-Release Licensed Software (i) may not be fully functional, may contain errors or design flaws, and may have reduced or different security, privacy, accessibility, availability, and reliability standards relative to commercially provided NVIDIA software and documentation, and (ii) use of such Pre-Release Licensed Software may result in unexpected results, loss of data, project delays or other unpredictable damage or loss. THEREFORE, PRE-RELEASE LICENSED SOFTWARE IS NOT INTENDED FOR USE, AND SHOULD NOT BE USED, IN PRODUCTION OR BUSINESS-CRITICAL SYSTEMS. NVIDIA has no obligation to make available a commercial version of any Pre-Release Licensed Software and NVIDIA has the right to abandon development of Pre-Release Licensed Software at any time without liability.
+
+1.4. Enterprise and Contractor Usage
+You may allow your Enterprise employees and Contractors to access and use the Licensed Software pursuant to the terms of the AGREEMENT solely to perform work on your behalf, provided further that with respect to Contractors: (i) you obtain a written agreement from each Contractor which contains terms and obligations with respect to access to and use of Licensed Software no less protective of NVIDIA than those set forth in the AGREEMENT, and (ii) such Contractor’s access and use expressly excludes any sublicensing or distribution rights for the Licensed Software. You are responsible for the compliance with the terms and conditions of the AGREEMENT by your Enterprise and Contractors. Any act or omission that, if committed by you, would constitute a breach of the AGREEMENT shall be deemed to constitute a breach of the AGREEMENT if committed by your Enterprise or Contractors.
+
+1.5. Services
+Except as expressly indicated in an Order, NVIDIA is under no obligation to provide support for the Licensed Software or to provide any patches, maintenance, updates or upgrades under the AGREEMENT. Unless patches, maintenance, updates or upgrades are provided with their separate governing terms and conditions, they constitute Licensed Software licensed to you under the AGREEMENT.
+
+2. LIMITATIONS.
+2.1. License Restrictions
+Except as expressly authorized in the AGREEMENT, you agree that you will not (nor authorize third parties to): (i) copy and use Software that was licensed to you for use in one or more NVIDIA hardware products in other unlicensed products (provided that copies solely for backup purposes are allowed); (ii) reverse engineer, decompile, disassemble (except to the extent applicable laws specifically require that such activities be permitted) or attempt to derive the source code, underlying ideas, algorithm or structure of Software provided to you in object code form; (iii) sell, transfer, assign, distribute, rent, loan, lease, sublicense or otherwise make available the Licensed Software or its functionality to third parties (a) as an application services provider or service bureau, (b) by operating hosted/virtual system environments, (c) by hosting, time sharing or providing any other type of services, or (d) otherwise by means of the internet; (iv) modify, translate or otherwise create any derivative works of any Licensed Software; (v) remove, alter, cover or obscure any proprietary notice that appears on or with the Licensed Software or any copies thereof; (vi) use the Licensed Software, or allow its use, transfer, transmission or export in violation of any applicable export control laws, rules or regulations; (vii) distribute, permit access to, or sublicense the Licensed Software as a stand-alone product; (viii) bypass, disable, circumvent or remove any form of copy protection, encryption, security or digital rights management or authentication mechanism used by NVIDIA in connection with the Licensed Software, or use the Licensed Software together with any authorization code, serial number, or other copy protection device not supplied by NVIDIA directly or through an authorized reseller; (ix) use the Licensed Software for the purpose of developing competing products or technologies or assisting a third party in such activities; (x) use the Licensed Software with any system or application where the use or failure of such system or application can reasonably be expected to threaten or result in personal injury, death, or catastrophic loss including, without limitation, use in connection with any nuclear, avionics, navigation, military, medical, life support or other life critical application (“Critical Applications”), unless the parties have entered into a Critical Applications agreement; (xi) distribute any modification or derivative work you make to the Licensed Software under or by reference to the same name as used by NVIDIA; or (xii) use the Licensed Software in any manner that would cause the Licensed Software to become subject to an Open Source License. Nothing in the AGREEMENT shall be construed to give you a right to use, or otherwise obtain access to, any source code from which the Software or any portion thereof is compiled or interpreted. You acknowledge that NVIDIA does not design, test, manufacture or certify the Licensed Software for use in the context of a Critical Application and NVIDIA shall not be liable to you or any third party, in whole or in part, for any claims or damages arising from such use. You agree to defend, indemnify and hold harmless NVIDIA and its Affiliates, and their respective employees, contractors, agents, officers and directors, from and against any and all claims, damages, obligations, losses, liabilities, costs or debt, fines, restitutions and expenses (including but not limited to attorney’s fees and costs incident to establishing the right of indemnification) arising out of or related to you and your Enterprise, and their respective employees, contractors, agents, distributors, resellers, end users, officers and directors use of Licensed Software outside of the scope of the AGREEMENT or any other breach of the terms of the AGREEMENT.
+
+2.2. Third Party License Obligations
+You acknowledge and agree that the Licensed Software may include or incorporate third party technology (collectively “Third Party Components”), which is provided for use in or with the Software and not otherwise used separately. If the Licensed Software includes or incorporates Third Party Components, then the third-party pass-through terms and conditions (“Third Party Terms”) for the particular Third Party Component will be bundled with the Software or otherwise made available online as indicated by NVIDIA and will be incorporated by reference into the AGREEMENT. In the event of any conflict between the terms in the AGREEMENT and the Third Party Terms, the Third Party Terms shall govern. Copyright to Third Party Components are held by the copyright holders indicated in the copyright notices indicated in the Third Party Terms.
+
+Audio/Video Encoders and Decoders: You acknowledge and agree that it is your sole responsibility to obtain any additional third party licenses required to make, have made, use, have used, sell, import, and offer for sale your products or services that include or incorporate any Third Party Components and content relating to audio and/or video encoders and decoders from, including but not limited to, Microsoft, Thomson, Fraunhofer IIS, Sisvel S.p.A., MPEG-LA, and Coding Technologies as NVIDIA does not grant to you under the AGREEMENT any necessary patent or other rights with respect to audio and/or video encoders and decoders.
+
+2.3. Limited Rights
+Your rights in the Licensed Software are limited to those expressly granted under the AGREEMENT and no other licenses are granted whether by implication, estoppel or otherwise. NVIDIA reserves all rights, title and interest in and to the Licensed Software not expressly granted under the AGREEMENT.
+
+3. CONFIDENTIALITY
+Neither party will use the other party’s Confidential Information, except as necessary for the performance of the AGREEMENT, nor will either party disclose such Confidential Information to any third party, except to personnel of NVIDIA and its Affiliates, you, your Enterprise, your Enterprise Contractors, and each party’s legal and financial advisors that have a need to know such Confidential Information for the performance of the AGREEMENT, provided that each such personnel, employee and Contractor is subject to a written agreement that includes confidentiality obligations consistent with those set forth herein. Each party will use all reasonable efforts to maintain the confidentiality of all of the other party’s Confidential Information in its possession or control, but in no event less than the efforts that it ordinarily uses with respect to its own Confidential Information of similar nature and importance. The foregoing obligations will not restrict either party from disclosing the other party’s Confidential Information or the terms and conditions of the AGREEMENT as required under applicable securities regulations or pursuant to the order or requirement of a court, administrative agency, or other governmental body, provided that the party required to make such disclosure (i) gives reasonable notice to the other party to enable it to contest such order or requirement prior to its disclosure (whether through protective orders or otherwise), (ii) uses reasonable effort to obtain confidential treatment or similar protection to the fullest extent possible to avoid such public disclosure, and (iii) discloses only the minimum amount of information necessary to comply with such requirements.
+
+4. OWNERSHIP
+You are not obligated to disclose to NVIDIA any modifications that you, your Enterprise or your Contractors make to the Licensed Software as permitted under the AGREEMENT. As between the parties, all modifications are owned by NVIDIA and licensed to you under the AGREEMENT unless otherwise expressly provided in a Supplement. The Licensed Software and all modifications owned by NVIDIA, and the respective Intellectual Property Rights therein, are and will remain the sole and exclusive property of NVIDIA or its licensors, whether the Licensed Software is separate from or combined with any other products or materials. You shall not engage in any act or omission that would impair NVIDIA’s and/or its licensors’ Intellectual Property Rights in the Licensed Software or any other materials, information, processes or subject matter proprietary to NVIDIA. NVIDIA’s licensors are intended third party beneficiaries with the right to enforce provisions of the AGREEMENT with respect to their Confidential Information and/or Intellectual Property Rights.
+
+5. FEEDBACK
+You have no obligation to provide Feedback to NVIDIA. However, NVIDIA and/or its Affiliates may use and include any Feedback that you provide to improve the Licensed Software or other NVIDIA products, technologies or materials. Accordingly, if you provide Feedback, you agree that NVIDIA and/or its Affiliates, at their option, may, and may permit their licensees, to make, have made, use, have used, reproduce, license, distribute and otherwise commercialize the Feedback in the Licensed Software or in other NVIDIA products, technologies or materials without the payment of any royalties or fees to you. All Feedback becomes the sole property of NVIDIA and may be used in any manner NVIDIA sees fit, and you hereby assign to NVIDIA all of your right, title and interest in and to any Feedback. NVIDIA has no obligation to respond to Feedback or to incorporate Feedback into the Licensed Software.
+
+6. NO WARRANTIES
+THE LICENSED SOFTWARE AND ANY OTHER CONFIDENTIAL INFORMATION AND/OR SERVICES ARE PROVIDED BY NVIDIA “AS IS” AND “WITH ALL FAULTS,” AND NVIDIA EXPRESSLY DISCLAIMS ALL OTHER WARRANTIES OF ANY KIND OR NATURE, WHETHER EXPRESS, IMPLIED OR STATUTORY, INCLUDING, BUT NOT LIMITED TO, ANY WARRANTIES OF OPERABILITY, CONDITION, VALUE, ACCURACY OF DATA, OR QUALITY, AS WELL AS ANY WARRANTIES OF MERCHANTABILITY, SYSTEM INTEGRATION, WORKMANSHIP, SUITABILITY, FITNESS FOR A PARTICULAR PURPOSE, NON-INFRINGEMENT, OR THE ABSENCE OF ANY DEFECTS THEREIN, WHETHER LATENT OR PATENT. NO WARRANTY IS MADE BY NVIDIA ON THE BASIS OF TRADE USAGE, COURSE OF DEALING OR COURSE OF TRADE. NVIDIA DOES NOT WARRANT THAT THE LICENSED SOFTWARE OR ANY OTHER CONFIDENTIAL INFORMATION AND/OR SERVICES PROVIDED BY NVIDIA UNDER THE AGREEMENT WILL MEET YOUR REQUIREMENTS OR THAT THE OPERATION THEREOF WILL BE UNINTERRUPTED OR ERROR-FREE, OR THAT ALL ERRORS WILL BE CORRECTED. YOU ACKNOWLEDGE THAT NVIDIA’S OBLIGATIONS UNDER THE AGREEMENT ARE FOR THE BENEFIT OF YOU ONLY. Nothing in this warranty section affects any statutory rights of consumers or other recipients to the extent that they cannot be waived or limited by contract under applicable law.
+
+7. LIMITATION OF LIABILITY
+TO THE MAXIMUM EXTENT PERMITTED BY LAW, NVIDIA OR ITS LICENSORS SHALL NOT BE LIABLE FOR ANY SPECIAL, INCIDENTAL, PUNITIVE OR CONSEQUENTIAL DAMAGES, OR ANY LOST PROFITS, LOSS OF USE, LOSS OF DATA OR LOSS OF GOODWILL, OR THE COSTS OF PROCURING SUBSTITUTE PRODUCTS, ARISING OUT OF OR IN CONNECTION WITH THE AGREEMENT OR THE USE OR PERFORMANCE OF THE LICENSED SOFTWARE AND ANY OTHER CONFIDENTIAL INFORMATION AND/OR SERVICES PROVIDED BY NVIDIA UNDER THE AGREEMENT, WHETHER SUCH LIABILITY ARISES FROM ANY CLAIM BASED UPON BREACH OF CONTRACT, BREACH OF WARRANTY, TORT (INCLUDING NEGLIGENCE), PRODUCT LIABILITY OR ANY OTHER CAUSE OF ACTION OR THEORY OF LIABILITY. IN NO EVENT WILL NVIDIA’S TOTAL CUMULATIVE LIABILITY UNDER OR ARISING OUT OF THE AGREEMENT EXCEED THE NET AMOUNTS RECEIVED BY NVIDIA FOR YOUR USE OF THE PARTICULAR LICENSED SOFTWARE DURING THE TWELVE (12) MONTHS BEFORE THE LIABILITY AROSE (or up to US$10.00 if you acquired the Licensed Software for no charge). THE NATURE OF THE LIABILITY, THE NUMBER OF CLAIMS OR SUITS OR THE NUMBER OF PARTIES WITHIN YOUR ENTERPRISE THAT ACCEPTED THE TERMS OF THE AGREEMENT SHALL NOT ENLARGE OR EXTEND THIS LIMIT. THE FOREGOING LIMITATIONS SHALL APPLY REGARDLESS OF WHETHER NVIDIA OR ITS LICENSORS HAVE BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES AND REGARDLESS OF WHETHER ANY REMEDY FAILS ITS ESSENTIAL PURPOSE. The disclaimers, exclusions and limitations of liability set forth in the AGREEMENT form an essential basis of the bargain between the parties, and, absent any such disclaimers, exclusions or limitations of liability, the provisions of the AGREEMENT, including, without limitation, the economic terms, would be substantially different.
+
+8. TERM AND TERMINATION.
+8.1. AGREEMENT, Licenses and Services
+This SLA shall become effective upon the Effective Date, each Supplement upon their acceptance, and both this SLA and Supplements shall continue in effect until your last access or use of the Licensed Software and/or services hereunder, unless earlier terminated as provided in this “Term and Termination” section. Each Licensed Software license ends at the earlier of (a) the expiration of the applicable license term, or (b) termination of such license or the AGREEMENT. Each service ends at the earlier of (x) the expiration of the applicable service term, (y) termination of such service or the AGREEMENT, or (z) expiration or termination of the associated license and no credit or refund will be provided upon the expiration or termination of the associated license for any service fees paid.
+
+8.2. Termination and Effect of Expiration or Termination
+NVIDIA may terminate the AGREEMENT in whole or in part: (i) if you breach any term of the AGREEMENT and fail to cure such breach within thirty (30) days following notice thereof from NVIDIA (or immediately if you violate NVIDIA’s Intellectual Property Rights); (ii) if you become the subject of a voluntary or involuntary petition in bankruptcy or any proceeding relating to insolvency, receivership, liquidation or composition for the benefit of creditors, if that petition or proceeding is not dismissed with prejudice within sixty (60) days after filing, or if you cease to do business; or (iii) if you commence or participate in any legal proceeding against NVIDIA, with respect to the Licensed Software that is the subject of the proceeding during the pendency of such legal proceeding. If you or your authorized NVIDIA reseller fail to pay license fees or service fees when due then NVIDIA may, in its sole discretion, suspend or terminate your license grants, services and any other rights provided under the AGREEMENT for the affected Licensed Software, in addition to any other remedies NVIDIA may have at law or equity. Upon any expiration or termination of the AGREEMENT, a license or a service provided hereunder, (a) any amounts owed to NVIDIA become immediately due and payable, (b) you must promptly discontinue use of the affected Licensed Software and/or service, and (c) you must promptly destroy or return to NVIDIA all copies of the affected Licensed Software and all portions thereof in your possession or control, and each party will promptly destroy or return to the other all of the other party’s Confidential Information within its possession or control. Upon written request, you will certify in writing that you have complied with your obligations under this section. Upon expiration or termination of the AGREEMENT all provisions survive except for the license grant provisions.
+
+9. CONSENT TO COLLECTION AND USE OF INFORMATION.
+You hereby agree and acknowledge that the Software may access, collect non-personally identifiable information about your Enterprise computer systems in order to properly optimize such systems for use with the Software. To the extent that you use the Software, you hereby consent to all of the foregoing, and represent and warrant that you have the right to grant such consent. In addition, you agree that you are solely responsible for maintaining appropriate data backups and system restore points for your Enterprise systems, and that NVIDIA will have no responsibility for any damage or loss to such systems (including loss of data or access) arising from or relating to (a) any changes to the configuration, application settings, environment variables, registry, drivers, BIOS, or other attributes of the systems (or any part of such systems) initiated through the Software; or (b) installation of any Software or third party software patches initiated through the Software. In certain systems you may change your system update preferences by unchecking "Automatically check for updates" in the "Preferences" tab of the control panel for the Software.
+
+In connection with the receipt of the Licensed Software or services you may receive access to links to third party websites and services and the availability of those links does not imply any endorsement by NVIDIA. NVIDIA encourages you to review the privacy statements on those sites and services that you choose to visit so that you can understand how they may collect, use and share personal information of individuals. NVIDIA is not responsible or liable for: (i) the availability or accuracy of such links; or (ii) the products, services or information available on or through such links; or (iii) the privacy statements or practices of sites and services controlled by other companies or organizations.
+
+To the extent that you or members of your Enterprise provide to NVIDIA during registration or otherwise personal information, you acknowledge that such information will be collected, used and disclosed by NVIDIA in accordance with NVIDIA's privacy policy, available at URL http://www.nvidia.com/object/privacy_policy.html.
+
+10. GENERAL.
+This SLA, any Supplements incorporated hereto, and Orders constitute the entire agreement of the parties with respect to the subject matter hereto and supersede all prior negotiations, conversations, or discussions between the parties relating to the subject matter hereto, oral or written, and all past dealings or industry custom. Any additional and/or conflicting terms and conditions on purchase order(s) or any other documents issued by you are null, void, and invalid. Any amendment or waiver under the AGREEMENT must be in writing and signed by representatives of both parties.
+
+The AGREEMENT and the rights and obligations thereunder may not be assigned by you, in whole or in part, including by merger, consolidation, dissolution, operation of law, or any other manner, without written consent of NVIDIA, and any purported assignment in violation of this provision shall be void and of no effect. NVIDIA may assign, delegate or transfer the AGREEMENT and its rights and obligations hereunder, and if to a non-Affiliate you will be notified.
+
+Each party acknowledges and agrees that the other is an independent contractor in the performance of the AGREEMENT, and each party is solely responsible for all of its employees, agents, contractors, and labor costs and expenses arising in connection therewith. The parties are not partners, joint ventures or otherwise affiliated, and neither has any authority to make any statements, representations or commitments of any kind to bind the other party without prior written consent.
+
+Neither party will be responsible for any failure or delay in its performance under the AGREEMENT (except for any payment obligations) to the extent due to causes beyond its reasonable control for so long as such force majeure event continues in effect.
+
+The AGREEMENT will be governed by and construed under the laws of the State of Delaware and the United States without regard to the conflicts of law provisions thereof and without regard to the United Nations Convention on Contracts for the International Sale of Goods. The parties consent to the personal jurisdiction of the federal and state courts located in Santa Clara County, California. You acknowledge and agree that a breach of any of your promises or agreements contained in the AGREEMENT may result in irreparable and continuing injury to NVIDIA for which monetary damages may not be an adequate remedy and therefore NVIDIA is entitled to seek injunctive relief as well as such other and further relief as may be appropriate. If any court of competent jurisdiction determines that any provision of the AGREEMENT is illegal, invalid or unenforceable, the remaining provisions will remain in full force and effect. Unless otherwise specified, remedies are cumulative.
+
+The Licensed Software has been developed entirely at private expense and is “commercial items” consisting of “commercial computer software” and “commercial computer software documentation” provided with RESTRICTED RIGHTS. Use, duplication or disclosure by the U.S. Government or a U.S. Government subcontractor is subject to the restrictions set forth in the AGREEMENT pursuant to DFARS 227.7202-3(a) or as set forth in subparagraphs (c)(1) and (2) of the Commercial Computer Software - Restricted Rights clause at FAR 52.227-19, as applicable. Contractor/manufacturer is NVIDIA, 2701 San Tomas Expressway, Santa Clara, CA 95050.
+
+You acknowledge that the Licensed Software described under the AGREEMENT is subject to export control under the U.S. Export Administration Regulations (EAR) and economic sanctions regulations administered by the U.S. Department of Treasury’s Office of Foreign Assets Control (OFAC). Therefore, you may not export, reexport or transfer in-country the Licensed Software without first obtaining any license or other approval that may be required by BIS and/or OFAC. You are responsible for any violation of the U.S. or other applicable export control or economic sanctions laws, regulations and requirements related to the Licensed Software. By accepting this SLA, you confirm that you are not a resident or citizen of any country currently embargoed by the U.S. and that you are not otherwise prohibited from receiving the Licensed Software.
+
+Any notice delivered by NVIDIA to you under the AGREEMENT will be delivered via mail, email or fax. Please direct your legal notices or other correspondence to NVIDIA Corporation, 2701 San Tomas Expressway, Santa Clara, California 95050, United States of America, Attention: Legal Department.
+
+11. GLOSSARY OF TERMS
+Certain capitalized terms, if not otherwise defined elsewhere in this SLA, shall have the meanings set forth below:
+“Affiliate”
+“Affiliate” means any legal entity that Owns, is Owned by, or is commonly Owned with a party. “Own” means having more than 50% ownership or the right to direct the management of the entity.
+“AGREEMENT”
+“AGREEMENT” means this SLA and all associated Supplements entered by the parties referencing this SLA.
+“Authorized Users”
+“Authorized Users” means your Enterprise individual employees and any of your Enterprise’s Contractors, subject to the terms of the “Enterprise and Contractors Usage” section.
+“Confidential Information”
+“Confidential Information” means the Licensed Software (unless made publicly available by NVIDIA without confidentiality obligations), and any NVIDIA business, marketing, pricing, research and development, know-how, technical, scientific, financial status, proposed new products or other information disclosed by NVIDIA to you which, at the time of disclosure, is designated in writing as confidential or proprietary (or like written designation), or orally identified as confidential or proprietary or is otherwise reasonably identifiable by parties exercising reasonable business judgment, as confidential. Confidential Information does not and will not include information that: (i) is or becomes generally known to the public through no fault of or breach of the AGREEMENT by the receiving party; (ii) is rightfully known by the receiving party at the time of disclosure without an obligation of confidentiality; (iii) is independently developed by the receiving party without use of the disclosing party’s Confidential Information; or (iv) is rightfully obtained by the receiving party from a third party without restriction on use or disclosure.
+“Contractor”
+“Contractor” means an individual who works primarily for your Enterprise on a contractor basis from your secure network. means an individual who works primarily for your Enterprise on a contractor basis from your secure network.
+“Documentation”
+“Documentation” means the NVIDIA documentation made available for use with the Software, including (without limitation) user manuals, datasheets, operations instructions, installation guides, release notes and other materials provided to you under the AGREEMENT.
+“Enterprise”
+“Enterprise” means you or any company or legal entity for which you accepted the terms of this SLA, and their subsidiaries of which your company or legal entity owns more than fifty percent (50%) of the issued and outstanding equity.
+“Feedback”
+“Feedback” means any and all suggestions, feature requests, comments or other feedback regarding the Licensed Software, including possible enhancements or modifications thereto.
+“Intellectual Property Rights”
+“Intellectual Property Rights” means all patent, copyright, trademark, trade secret, trade dress, trade names, utility models, mask work, moral rights, rights of attribution or integrity service marks, master recording and music publishing rights, performance rights, author’s rights, database rights, registered design rights and any applications for the protection or registration of these rights, or other intellectual or industrial property rights or proprietary rights, howsoever arising and in whatever media, whether now known or hereafter devised, whether or not registered, (including all claims and causes of action for infringement, misappropriation or violation and all rights in any registrations and renewals), worldwide and whether existing now or in the future.
+“Licensed Software”
+“Licensed Software” means Software, Documentation and all modifications owned by NVIDIA.
+“Open Source License”
+“Open Source License” includes, without limitation, a software license that requires as a condition of use, modification, and/or distribution of such software that the Software be (i) disclosed or distributed in source code form; (ii) be licensed for the purpose of making derivative works; or (iii) be redistributable at no charge.
+“Order”
+“Order” means a purchase order issued by you, a signed purchase agreement with you, or other ordering document issued by you to NVIDIA or a NVIDIA authorized reseller (including any on-line acceptance process) that references and incorporates the AGREEMENT and is accepted by NVIDIA.
+“Software”
+“Software” means the NVIDIA software programs licensed to you under the AGREEMENT including, without limitation, libraries, sample code, utility programs and programming code.
+“Supplement”
+“Supplement” means the additional terms and conditions beyond those stated in this SLA that apply to certain Licensed Software licensed hereunder.
+12. TensorRT SUPPLEMENT TO SOFTWARE LICENSE AGREEMENT
+TensorRT SUPPLEMENT TO SOFTWARE LICENSE AGREEMENT
+The terms set forth in this TensorRT Supplement (“Supplement”) govern your use of the NVIDIA GPU inference engine (the “TensorRT Licensed Software”) under the terms of your software license agreement (“SLA”) as modified by this Supplement. This Supplement is an exhibit to the SLA and is hereby incorporated as an integral part thereto. Capitalized terms used but not defined herein shall have the meaning assigned to them in the SLA. In the event of conflict between the terms in this Supplement and the terms in the SLA, this Supplement shall control.
+
+12.1. TensorRT DISTRIBUTION
+Subject to the terms of the SLA and this Supplement, NVIDIA hereby grants you a non-exclusive, nontransferable license during the applicable license term unless earlier terminated pursuant to the SLA, to distribute the libnvinfer and libnvinfer_plugin libraries when delivered to you as part of the TensorRT Licensed Software in source code form or binary form (but not when provided to you as part of a hardware product), subject to the following: such distribution is solely in binary form to your licensees (“Customers”) only as a component of your own software products having additional material functionality beyond the TensorRT Licensed Software (each, a “Licensee Application"). Subject to the terms and conditions of the SLA and this Supplement, you may further authorize Customers to redistribute the libnvinfer and libnvinfer_plugin libraries as incorporated into a Licensee Application, solely in binary form, provided, however, that you shall require in your agreements with your Customers that their distributions be on terms at least as restrictive as those applicable for your use of such TensorRT Licensed Software within a Licensee Application. The expiration or termination of your licenses to the above described TensorRT Licensed Software under the SLA and this Supplement will not affect rights previously granted by you to recipients that were in compliance with the SLA and this Supplement.
+
+In addition to the rights above, for parties that are developing software intended solely for use on Jetson development kits or Jetson modules and running Linux for Tegra software the following shall apply: TensorRT Licensed Software licensed hereunder may be distributed in its entirety, as provided by NVIDIA and without separation of its components, for you and/or your licensees to create software development kits for use only on the Jetson platform and running Linux for Tegra software. You shall require in your agreements with your licensees that their distributions be on terms at least as restrictive as those applicable for your distribution of TensorRT Licensed Software as described in this Section 1.
+
+In addition to the rights above, for parties that are developing software intended solely for use on Jetson development kits or Jetson modules and running Linux for Tegra software the following shall apply: TensorRT Licensed Software licensed hereunder may be distributed in its entirety, as provided by NVIDIA and without separation of its components, for you and/or your licensees to create software development kits for use only on the Jetson platform and running Linux for Tegra software. You shall require in your agreements with your licensees that their distributions be on terms at least as restrictive as those applicable for your distribution of TensorRT Licensed Software as described in this Section 1.
+
+12.2. LICENSE DURATION
+Each TensorRT Licensed Software is licensed to you for an initial duration of one year starting from the date of delivery or download. The licenses granted will automatically renew for successive one year periods, provided that NVIDIA reserves the right to terminate licenses upon ninety days (90) days written notice to you prior to the commencement of a renewal year in addition to the termination rights set forth in the SLA.
+
+12.3. EXPIRATION OF TERMINATION OF THIS SUPPLEMENT
+Your failure to comply with the terms of this Supplement is ground for termination for breach by NVIDIA under the SLA. This Supplement will automatically expire or terminate upon the expiration or termination of your rights to TensorRT Licensed Software under the SLA or this Supplement.
+
+Notices
+Notice
+This document is provided for information purposes only and shall not be regarded as a warranty of a certain functionality, condition, or quality of a product. NVIDIA Corporation (“NVIDIA”) makes no representations or warranties, expressed or implied, as to the accuracy or completeness of the information contained in this document and assumes no responsibility for any errors contained herein. NVIDIA shall have no liability for the consequences or use of such information or for any infringement of patents or other rights of third parties that may result from its use. This document is not a commitment to develop, release, or deliver any Material (defined below), code, or functionality.
+
+NVIDIA reserves the right to make corrections, modifications, enhancements, improvements, and any other changes to this document, at any time without notice.
+
+Customer should obtain the latest relevant information before placing orders and should verify that such information is current and complete.
+
+NVIDIA products are sold subject to the NVIDIA standard terms and conditions of sale supplied at the time of order acknowledgement, unless otherwise agreed in an individual sales agreement signed by authorized representatives of NVIDIA and customer (“Terms of Sale”). NVIDIA hereby expressly objects to applying any customer general terms and conditions with regards to the purchase of the NVIDIA product referenced in this document. No contractual obligations are formed either directly or indirectly by this document.
+
+NVIDIA products are not designed, authorized, or warranted to be suitable for use in medical, military, aircraft, space, or life support equipment, nor in applications where failure or malfunction of the NVIDIA product can reasonably be expected to result in personal injury, death, or property or environmental damage. NVIDIA accepts no liability for inclusion and/or use of NVIDIA products in such equipment or applications and therefore such inclusion and/or use is at customer’s own risk.
+
+NVIDIA makes no representation or warranty that products based on this document will be suitable for any specified use. Testing of all parameters of each product is not necessarily performed by NVIDIA. It is customer’s sole responsibility to evaluate and determine the applicability of any information contained in this document, ensure the product is suitable and fit for the application planned by customer, and perform the necessary testing for the application in order to avoid a default of the application or the product. Weaknesses in customer’s product designs may affect the quality and reliability of the NVIDIA product and may result in additional or different conditions and/or requirements beyond those contained in this document. NVIDIA accepts no liability related to any default, damage, costs, or problem which may be based on or attributable to: (i) the use of the NVIDIA product in any manner that is contrary to this document or (ii) customer product designs.
+
+No license, either expressed or implied, is granted under any NVIDIA patent right, copyright, or other NVIDIA intellectual property right under this document. Information published by NVIDIA regarding third-party products or services does not constitute a license from NVIDIA to use such products or services or a warranty or endorsement thereof. Use of such information may require a license from a third party under the patents or other intellectual property rights of the third party, or a license from NVIDIA under the patents or other intellectual property rights of NVIDIA.
+
+Reproduction of information in this document is permissible only if approved in advance by NVIDIA in writing, reproduced without alteration and in full compliance with all applicable export laws and regulations, and accompanied by all associated conditions, limitations, and notices.
+
+THIS DOCUMENT AND ALL NVIDIA DESIGN SPECIFICATIONS, REFERENCE BOARDS, FILES, DRAWINGS, DIAGNOSTICS, LISTS, AND OTHER DOCUMENTS (TOGETHER AND SEPARATELY, “MATERIALS”) ARE BEING PROVIDED “AS IS.” NVIDIA MAKES NO WARRANTIES, EXPRESSED, IMPLIED, STATUTORY, OR OTHERWISE WITH RESPECT TO THE MATERIALS, AND EXPRESSLY DISCLAIMS ALL IMPLIED WARRANTIES OF NONINFRINGEMENT, MERCHANTABILITY, AND FITNESS FOR A PARTICULAR PURPOSE. TO THE EXTENT NOT PROHIBITED BY LAW, IN NO EVENT WILL NVIDIA BE LIABLE FOR ANY DAMAGES, INCLUDING WITHOUT LIMITATION ANY DIRECT, INDIRECT, SPECIAL, INCIDENTAL, PUNITIVE, OR CONSEQUENTIAL DAMAGES, HOWEVER CAUSED AND REGARDLESS OF THE THEORY OF LIABILITY, ARISING OUT OF ANY USE OF THIS DOCUMENT, EVEN IF NVIDIA HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES. Notwithstanding any damages that customer might incur for any reason whatsoever, NVIDIA’s aggregate and cumulative liability towards customer for the products described herein shall be limited in accordance with the Terms of Sale for the product.
+
+VESA DisplayPort
+DisplayPort and DisplayPort Compliance Logo, DisplayPort Compliance Logo for Dual-mode Sources, and DisplayPort Compliance Logo for Active Cables are trademarks owned by the Video Electronics Standards Association in the United States and other countries.
+
+HDMI
+HDMI, the HDMI logo, and High-Definition Multimedia Interface are trademarks or registered trademarks of HDMI Licensing LLC.
+
+ARM
+ARM, AMBA and ARM Powered are registered trademarks of ARM Limited. Cortex, MPCore and Mali are trademarks of ARM Limited. All other brands or product names are the property of their respective holders. "ARM" is used to represent ARM Holdings plc; its operating company ARM Limited; and the regional subsidiaries ARM Inc.; ARM KK; ARM Korea Limited.; ARM Taiwan Limited; ARM France SAS; ARM Consulting (Shanghai) Co. Ltd.; ARM Germany GmbH; ARM Embedded Technologies Pvt. Ltd.; ARM Norway, AS and ARM Sweden AB.
+
+OpenCL
+OpenCL is a trademark of Apple Inc. used under license to the Khronos Group Inc.
+
+Trademarks
+NVIDIA, the NVIDIA logo, and cuBLAS, CUDA, CUDA Toolkit, cuDNN, DALI, DIGITS, DGX, DGX-1, DGX-2, DGX Station, DLProf, GPU, JetPack, Jetson, Kepler, Maxwell, NCCL, Nsight Compute, Nsight Systems, NVCaffe, NVIDIA Ampere GPU architecture, NVIDIA Deep Learning SDK, NVIDIA Developer Program, NVIDIA GPU Cloud, NVLink, NVSHMEM, PerfWorks, Pascal, SDK Manager, T4, Tegra, TensorRT, TensorRT Inference Server, Tesla, TF-TRT, Triton Inference Server, Turing, and Volta are trademarks and/or registered trademarks of NVIDIA Corporation in the United States and other countries. Other company and product names may be trademarks of the respective companies with which they are associated.
+
+Copyright
+© 2021 NVIDIA Corporation. All rights reserved.
```

### Comparing `tensorrt-cu11-10.0.0b6/PKG-INFO` & `tensorrt-cu11-10.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1
-Name: tensorrt-cu11
-Version: 10.0.0b6
-Summary: A high performance deep learning inference library
-Home-page: https://developer.nvidia.com/tensorrt
-Download-URL: https://github.com/nvidia/tensorrt/tags
-Author: NVIDIA Corporation
-License: Proprietary
-Keywords: nvidia tensorrt deeplearning inference
-Classifier: License :: Other/Proprietary License
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Provides-Extra: numpy
-Requires-Dist: numpy; extra == "numpy"
-
-
-NVIDIA TensorRT is an SDK that facilitates high-performance machine learning inference. It is designed to work in a complementary fashion with training frameworks such as TensorFlow, PyTorch, and MXNet. It focuses specifically on running an already-trained network quickly and efficiently on NVIDIA hardware.
-
-**IMPORTANT:** This is a special release of TensorRT designed to work only with TensorRT-LLM.
-Please refrain from upgrading to this version if you are not using TensorRT-LLM.
-
-To install, please execute the following:
-```
-pip install tensorrt --extra-index-url https://pypi.nvidia.com
-```
-Or add the index URL to the (space-separated) PIP_EXTRA_INDEX_URL environment variable:
-```
-export PIP_EXTRA_INDEX_URL='https://pypi.nvidia.com'
-pip install tensorrt
-```
-When the extra index url does not contain `https://pypi.nvidia.com`, a nested `pip install` will run with the proper extra index url hard-coded.
+Metadata-Version: 2.1
+Name: tensorrt-cu11
+Version: 10.0.1
+Summary: A high performance deep learning inference library
+Home-page: https://developer.nvidia.com/tensorrt
+Download-URL: https://github.com/nvidia/tensorrt/tags
+Author: NVIDIA Corporation
+License: Proprietary
+Keywords: nvidia tensorrt deeplearning inference
+Classifier: License :: Other/Proprietary License
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Provides-Extra: numpy
+Requires-Dist: numpy; extra == "numpy"
+
+
+NVIDIA TensorRT is an SDK that facilitates high-performance machine learning inference. It is designed to work in a complementary fashion with training frameworks such as TensorFlow, PyTorch, and MXNet. It focuses specifically on running an already-trained network quickly and efficiently on NVIDIA hardware.
+
+**IMPORTANT:** This is a special release of TensorRT designed to work only with TensorRT-LLM.
+Please refrain from upgrading to this version if you are not using TensorRT-LLM.
+
+To install, please execute the following:
+```
+pip install tensorrt --extra-index-url https://pypi.nvidia.com
+```
+Or add the index URL to the (space-separated) PIP_EXTRA_INDEX_URL environment variable:
+```
+export PIP_EXTRA_INDEX_URL='https://pypi.nvidia.com'
+pip install tensorrt
+```
+When the extra index url does not contain `https://pypi.nvidia.com`, a nested `pip install` will run with the proper extra index url hard-coded.
```

### Comparing `tensorrt-cu11-10.0.0b6/setup.py` & `tensorrt-cu11-10.0.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,164 +1,164 @@
-#
-# SPDX-FileCopyrightText: Copyright (c) 1993-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
-# SPDX-License-Identifier: Apache-2.0
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-
-import os
-import platform
-import subprocess
-import sys
-import glob
-
-from setuptools import setup
-from setuptools.command.install import install
-
-tensorrt_module = "tensorrt-cu11"
-tensorrt_package = "tensorrt"
-tensorrt_version = "10.0.0b6"
-tensorrt_submodules = [
-    "{}_libs=={}".format(tensorrt_module, tensorrt_version),
-    "{}_bindings=={}".format(tensorrt_module, tensorrt_version),
-]
-nvidia_pip_index_url = os.environ.get("NVIDIA_PIP_INDEX_URL", "https://pypi.nvidia.com")
-disable_internal_pip = os.environ.get("NVIDIA_TENSORRT_DISABLE_INTERNAL_PIP", False)
-
-
-def run_pip_command(args, call_func):
-    env = os.environ.copy()
-    env["PYTHONPATH"] = sys.exec_prefix
-    try:
-        return call_func([sys.executable, "-m", "pip"] + args, env=env)
-    except subprocess.CalledProcessError:
-
-        def find_pip():
-            pip_name = "pip"
-            if sys.platform.startswith("win"):
-                pip_name = "pip.exe"
-            for path in glob.iglob(os.path.join(sys.exec_prefix, "**"), recursive=True):
-                if os.path.isfile(path) and os.path.basename(path) == pip_name:
-                    return path
-            return None
-
-        pip_path = find_pip()
-        if pip_path is None:
-            # Couldn't find `pip` in `sys.exec_prefix`, so we have no option but to abort.
-            raise
-        return call_func([pip_path] + args, env=env)
-
-
-# check wheel availability using information from https://github.com/pypa/packaging/blob/23.1/src/packaging/markers.py#L175-L190
-if sys.platform not in ("linux", "win32"):
-    raise RuntimeError("TensorRT currently only builds wheels for Linux and Windows")
-if sys.implementation.name != "cpython":
-    raise RuntimeError("TensorRT currently only builds wheels for CPython")
-if platform.machine() not in ("x86_64", "AMD64"):
-    raise RuntimeError("TensorRT currently only builds wheels for x86_64 processors")
-
-
-class InstallCommand(install):
-    def run(self):
-        # pip-inside-pip hack ref #3080
-        run_pip_command(
-            [
-                "install",
-                "--extra-index-url",
-                nvidia_pip_index_url,
-                *tensorrt_submodules,
-            ],
-            subprocess.check_call,
-        )
-
-        super().run()
-
-
-def pip_config_list():
-    """Get the current pip config (env vars, config file, etc)."""
-    try:
-        return run_pip_command(["config", "list"], subprocess.check_output).decode()
-    except:
-        return ""
-
-
-def parent_command_line():
-    """Get the command line of the parent PID."""
-    pid = os.getppid()
-
-    # try retrieval using psutil
-    try:
-        import psutil
-
-        return " ".join(psutil.Process(pid).cmdline())
-    except:
-        pass
-    # fall back to shell
-    try:
-        return subprocess.check_output(["ps", "-p", str(pid), "-o", "command", "--no-headers"]).decode()
-    except:
-        return ""
-
-
-# use pip-inside-pip hack only if the nvidia index is not set in the environment
-install_requires = []
-if disable_internal_pip or nvidia_pip_index_url in parent_command_line() or nvidia_pip_index_url in pip_config_list():
-    install_requires.extend(tensorrt_submodules)
-    cmdclass = {}
-else:
-    cmdclass = {"install": InstallCommand}
-
-
-setup(
-    name=tensorrt_module,
-    version=tensorrt_version,
-    description="A high performance deep learning inference library",
-    long_description="""
-NVIDIA TensorRT is an SDK that facilitates high-performance machine learning inference. It is designed to work in a complementary fashion with training frameworks such as TensorFlow, PyTorch, and MXNet. It focuses specifically on running an already-trained network quickly and efficiently on NVIDIA hardware.
-
-**IMPORTANT:** This is a special release of TensorRT designed to work only with TensorRT-LLM.
-Please refrain from upgrading to this version if you are not using TensorRT-LLM.
-
-To install, please execute the following:
-```
-pip install tensorrt --extra-index-url {}
-```
-Or add the index URL to the (space-separated) PIP_EXTRA_INDEX_URL environment variable:
-```
-export PIP_EXTRA_INDEX_URL='{}'
-pip install tensorrt
-```
-When the extra index url does not contain `{}`, a nested `pip install` will run with the proper extra index url hard-coded.
-""".format(
-        nvidia_pip_index_url, nvidia_pip_index_url, nvidia_pip_index_url
-    ),
-    long_description_content_type="text/markdown",
-    author="NVIDIA Corporation",
-    license="Proprietary",
-    classifiers=[
-        "License :: Other/Proprietary License",
-        "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
-    ],
-    packages=[tensorrt_package],
-    install_requires=install_requires,
-    setup_requires=["wheel"],
-    python_requires=">=3.6",  # ref https://pypi.nvidia.com/tensorrt-bindings/
-    cmdclass=cmdclass,
-    extras_require={"numpy": "numpy"},
-    package_data={tensorrt_package: ["*.so*", "*.pyd", "*.pdb", "*.dll*"]},
-    include_package_data=True,
-    zip_safe=True,
-    keywords="nvidia tensorrt deeplearning inference",
-    url="https://developer.nvidia.com/tensorrt",
-    download_url="https://github.com/nvidia/tensorrt/tags",
-)
+#
+# SPDX-FileCopyrightText: Copyright (c) 1993-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-License-Identifier: Apache-2.0
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+
+import os
+import platform
+import subprocess
+import sys
+import glob
+
+from setuptools import setup
+from setuptools.command.install import install
+
+tensorrt_module = "tensorrt-cu11"
+tensorrt_package = "tensorrt"
+tensorrt_version = "10.0.1"
+tensorrt_submodules = [
+    "{}_libs=={}".format(tensorrt_module, tensorrt_version),
+    "{}_bindings=={}".format(tensorrt_module, tensorrt_version),
+]
+nvidia_pip_index_url = os.environ.get("NVIDIA_PIP_INDEX_URL", "https://pypi.nvidia.com")
+disable_internal_pip = os.environ.get("NVIDIA_TENSORRT_DISABLE_INTERNAL_PIP", False)
+
+
+def run_pip_command(args, call_func):
+    env = os.environ.copy()
+    env["PYTHONPATH"] = sys.exec_prefix
+    try:
+        return call_func([sys.executable, "-m", "pip"] + args, env=env)
+    except subprocess.CalledProcessError:
+
+        def find_pip():
+            pip_name = "pip"
+            if sys.platform.startswith("win"):
+                pip_name = "pip.exe"
+            for path in glob.iglob(os.path.join(sys.exec_prefix, "**"), recursive=True):
+                if os.path.isfile(path) and os.path.basename(path) == pip_name:
+                    return path
+            return None
+
+        pip_path = find_pip()
+        if pip_path is None:
+            # Couldn't find `pip` in `sys.exec_prefix`, so we have no option but to abort.
+            raise
+        return call_func([pip_path] + args, env=env)
+
+
+# check wheel availability using information from https://github.com/pypa/packaging/blob/23.1/src/packaging/markers.py#L175-L190
+if sys.platform not in ("linux", "win32"):
+    raise RuntimeError("TensorRT currently only builds wheels for Linux and Windows")
+if sys.implementation.name != "cpython":
+    raise RuntimeError("TensorRT currently only builds wheels for CPython")
+if platform.machine() not in ("x86_64", "AMD64"):
+    raise RuntimeError("TensorRT currently only builds wheels for x86_64 processors")
+
+
+class InstallCommand(install):
+    def run(self):
+        # pip-inside-pip hack ref #3080
+        run_pip_command(
+            [
+                "install",
+                "--extra-index-url",
+                nvidia_pip_index_url,
+                *tensorrt_submodules,
+            ],
+            subprocess.check_call,
+        )
+
+        super().run()
+
+
+def pip_config_list():
+    """Get the current pip config (env vars, config file, etc)."""
+    try:
+        return run_pip_command(["config", "list"], subprocess.check_output).decode()
+    except:
+        return ""
+
+
+def parent_command_line():
+    """Get the command line of the parent PID."""
+    pid = os.getppid()
+
+    # try retrieval using psutil
+    try:
+        import psutil
+
+        return " ".join(psutil.Process(pid).cmdline())
+    except:
+        pass
+    # fall back to shell
+    try:
+        return subprocess.check_output(["ps", "-p", str(pid), "-o", "command", "--no-headers"]).decode()
+    except:
+        return ""
+
+
+# use pip-inside-pip hack only if the nvidia index is not set in the environment
+install_requires = []
+if disable_internal_pip or nvidia_pip_index_url in parent_command_line() or nvidia_pip_index_url in pip_config_list():
+    install_requires.extend(tensorrt_submodules)
+    cmdclass = {}
+else:
+    cmdclass = {"install": InstallCommand}
+
+
+setup(
+    name=tensorrt_module,
+    version=tensorrt_version,
+    description="A high performance deep learning inference library",
+    long_description="""
+NVIDIA TensorRT is an SDK that facilitates high-performance machine learning inference. It is designed to work in a complementary fashion with training frameworks such as TensorFlow, PyTorch, and MXNet. It focuses specifically on running an already-trained network quickly and efficiently on NVIDIA hardware.
+
+**IMPORTANT:** This is a special release of TensorRT designed to work only with TensorRT-LLM.
+Please refrain from upgrading to this version if you are not using TensorRT-LLM.
+
+To install, please execute the following:
+```
+pip install tensorrt --extra-index-url {}
+```
+Or add the index URL to the (space-separated) PIP_EXTRA_INDEX_URL environment variable:
+```
+export PIP_EXTRA_INDEX_URL='{}'
+pip install tensorrt
+```
+When the extra index url does not contain `{}`, a nested `pip install` will run with the proper extra index url hard-coded.
+""".format(
+        nvidia_pip_index_url, nvidia_pip_index_url, nvidia_pip_index_url
+    ),
+    long_description_content_type="text/markdown",
+    author="NVIDIA Corporation",
+    license="Proprietary",
+    classifiers=[
+        "License :: Other/Proprietary License",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3",
+    ],
+    packages=[tensorrt_package],
+    install_requires=install_requires,
+    setup_requires=["wheel"],
+    python_requires=">=3.6",  # ref https://pypi.nvidia.com/tensorrt-bindings/
+    cmdclass=cmdclass,
+    extras_require={"numpy": "numpy"},
+    package_data={tensorrt_package: ["*.so*", "*.pyd", "*.pdb", "*.dll*"]},
+    include_package_data=True,
+    zip_safe=True,
+    keywords="nvidia tensorrt deeplearning inference",
+    url="https://developer.nvidia.com/tensorrt",
+    download_url="https://github.com/nvidia/tensorrt/tags",
+)
```

### Comparing `tensorrt-cu11-10.0.0b6/tensorrt/__init__.py` & `tensorrt-cu11-10.0.1/tensorrt/__init__.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-#
-# SPDX-FileCopyrightText: Copyright (c) 1993-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
-# SPDX-License-Identifier: Apache-2.0
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-
-from tensorrt_bindings import *
-from tensorrt_bindings import __version__
+#
+# SPDX-FileCopyrightText: Copyright (c) 1993-2023 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
+# SPDX-License-Identifier: Apache-2.0
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+
+from tensorrt_bindings import *
+from tensorrt_bindings import __version__
```

### Comparing `tensorrt-cu11-10.0.0b6/tensorrt_cu11.egg-info/PKG-INFO` & `tensorrt-cu11-10.0.1/tensorrt_cu11.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1
-Name: tensorrt-cu11
-Version: 10.0.0b6
-Summary: A high performance deep learning inference library
-Home-page: https://developer.nvidia.com/tensorrt
-Download-URL: https://github.com/nvidia/tensorrt/tags
-Author: NVIDIA Corporation
-License: Proprietary
-Keywords: nvidia tensorrt deeplearning inference
-Classifier: License :: Other/Proprietary License
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Provides-Extra: numpy
-Requires-Dist: numpy; extra == "numpy"
-
-
-NVIDIA TensorRT is an SDK that facilitates high-performance machine learning inference. It is designed to work in a complementary fashion with training frameworks such as TensorFlow, PyTorch, and MXNet. It focuses specifically on running an already-trained network quickly and efficiently on NVIDIA hardware.
-
-**IMPORTANT:** This is a special release of TensorRT designed to work only with TensorRT-LLM.
-Please refrain from upgrading to this version if you are not using TensorRT-LLM.
-
-To install, please execute the following:
-```
-pip install tensorrt --extra-index-url https://pypi.nvidia.com
-```
-Or add the index URL to the (space-separated) PIP_EXTRA_INDEX_URL environment variable:
-```
-export PIP_EXTRA_INDEX_URL='https://pypi.nvidia.com'
-pip install tensorrt
-```
-When the extra index url does not contain `https://pypi.nvidia.com`, a nested `pip install` will run with the proper extra index url hard-coded.
+Metadata-Version: 2.1
+Name: tensorrt-cu11
+Version: 10.0.1
+Summary: A high performance deep learning inference library
+Home-page: https://developer.nvidia.com/tensorrt
+Download-URL: https://github.com/nvidia/tensorrt/tags
+Author: NVIDIA Corporation
+License: Proprietary
+Keywords: nvidia tensorrt deeplearning inference
+Classifier: License :: Other/Proprietary License
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Provides-Extra: numpy
+Requires-Dist: numpy; extra == "numpy"
+
+
+NVIDIA TensorRT is an SDK that facilitates high-performance machine learning inference. It is designed to work in a complementary fashion with training frameworks such as TensorFlow, PyTorch, and MXNet. It focuses specifically on running an already-trained network quickly and efficiently on NVIDIA hardware.
+
+**IMPORTANT:** This is a special release of TensorRT designed to work only with TensorRT-LLM.
+Please refrain from upgrading to this version if you are not using TensorRT-LLM.
+
+To install, please execute the following:
+```
+pip install tensorrt --extra-index-url https://pypi.nvidia.com
+```
+Or add the index URL to the (space-separated) PIP_EXTRA_INDEX_URL environment variable:
+```
+export PIP_EXTRA_INDEX_URL='https://pypi.nvidia.com'
+pip install tensorrt
+```
+When the extra index url does not contain `https://pypi.nvidia.com`, a nested `pip install` will run with the proper extra index url hard-coded.
```
