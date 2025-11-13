# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_Coverity_Detailed_Sample/main`
- **Build Number:** #2
- **Build Status:** 🟢 **SUCCESS**
- **Duration:** 5 min 24 sec and counting
- **Timestamp:** 2025-11-13 21:27:01 UTC

---

## Console Output

```
Branch indexing
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from 839159479d8d6b0bd4736aad0c839ac2ceefe62d
Loading library blackduck-logs-publisher@main
Attempting to resolve main from remote references...
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git ls-remote -h -- https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Found match: refs/heads/main revision e969196a63b1be83b84541b022f7aa52928bd5e5
The recommended git tool is: NONE
using credential Github_Username_PAT
 > git rev-parse --resolve-git-dir /Users/madhusud/.jenkins/workspace/ub_Coverity_Detailed_Sample_main@libs/a0dda568bac7bbb4a171f59ba3f2660c21c69edc6356524e9ae8bb4500c12bbb/.git # timeout=10
Fetching changes from the remote Git repository
 > git config remote.origin.url https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Fetching without tags
Fetching upstream changes from https://github.com/integrations-garage/blackduck-logs-publisher
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/integrations-garage/blackduck-logs-publisher +refs/heads/*:refs/remotes/origin/* # timeout=10
Checking out Revision e969196a63b1be83b84541b022f7aa52928bd5e5 (main)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f e969196a63b1be83b84541b022f7aa52928bd5e5 # timeout=10
Commit message: "Phase 3 - 2"
 > git rev-list --no-walk e969196a63b1be83b84541b022f7aa52928bd5e5 # timeout=10
[Pipeline] Start of Pipeline
[Pipeline] node
Running on mac-sh in /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
The recommended git tool is: NONE
using credential Github_Username_PAT
Cloning the remote Git repository
Cloning with configured refspecs honoured and without tags
Cloning repository https://github.com/coverity-cnc-jenkins-samples/detailed-example.git
 > git init /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2 # timeout=10
Fetching upstream changes from https://github.com/coverity-cnc-jenkins-samples/detailed-example.git
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/coverity-cnc-jenkins-samples/detailed-example.git +refs/heads/main:refs/remotes/origin/main # timeout=10
Avoid second fetch
Checking out Revision 839159479d8d6b0bd4736aad0c839ac2ceefe62d (main)
Commit message: "Coverity Detailed Sample"
First time build. Skipping changelog.
 > git config remote.origin.url https://github.com/coverity-cnc-jenkins-samples/detailed-example.git # timeout=10
 > git config --add remote.origin.fetch +refs/heads/main:refs/remotes/origin/main # timeout=10
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 839159479d8d6b0bd4736aad0c839ac2ceefe62d # timeout=10
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Build)
[Pipeline] script
[Pipeline] {
[Pipeline] echo
JOB_NAME: MBP_Github_Coverity_Detailed_Sample/main
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm
[Pipeline] {
[Pipeline] sh
+ node --version
v22.16.0
[Pipeline] sh
+ npm --version
10.9.2
[Pipeline] sh
+ npm install
npm warn deprecated fsevents@1.2.9: fsevents 1 will break on node v14+ and could be using insecure binaries. Upgrade to fsevents 2.
npm warn deprecated set-value@2.0.0: Critical bug fixed in v3.0.1, please upgrade to the latest version.
npm warn deprecated mixin-deep@1.3.1: Critical bug fixed in v2.0.1, please upgrade to the latest version.
npm warn deprecated ini@1.3.5: Please update to ini >=1.3.6 to avoid a prototype pollution issue
npm warn deprecated set-value@0.4.3: Critical bug fixed in v3.0.1, please upgrade to the latest version.
npm warn deprecated path-is-absolute@2.0.0: This package is no longer relevant as Node.js 0.12 is unmaintained.
npm warn deprecated urix@0.1.0: Please see https://github.com/lydell/urix#deprecated
npm warn deprecated har-validator@5.1.3: this library is no longer supported
npm warn deprecated to-iso-string@0.0.2: to-iso-string has been deprecated, use @segment/to-iso-string instead.
npm warn deprecated cryptiles@2.0.5: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated resolve-url@0.2.1: https://github.com/lydell/resolve-url#deprecated
npm warn deprecated bcrypt-nodejs@0.0.3: bcrypt-nodejs is no longer actively maintained. Please use bcrypt or bcryptjs. See https://github.com/kelektiv/node.bcrypt.js/wiki/bcrypt-vs-brypt.js to learn more about these two options
npm warn deprecated cryptiles@0.2.2: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated source-map-url@0.4.0: See https://github.com/lydell/source-map-url#deprecated
npm warn deprecated boom@0.4.2: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated boom@2.10.1: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated chokidar@2.1.6: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
npm warn deprecated sntp@0.2.4: This module moved to @hapi/sntp. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated minimatch@0.3.0: Please update to minimatch 3.0.2 or higher to avoid a RegExp DoS issue
npm warn deprecated chokidar@2.1.8: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
npm warn deprecated sntp@1.0.9: This module moved to @hapi/sntp. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated querystring@0.2.0: The querystring API is considered Legacy. new code should use the URLSearchParams API instead.
npm warn deprecated request@2.36.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated mkdirp@0.3.0: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
npm warn deprecated tough-cookie@2.2.2: ReDoS vulnerability parsing Set-Cookie https://nodesecurity.io/advisories/130
npm warn deprecated hoek@0.9.1: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated node-uuid@1.4.8: Use uuid module instead
npm warn deprecated node-uuid@1.4.8: Use uuid module instead
npm warn deprecated uuid@3.3.2: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
npm warn deprecated source-map-resolve@0.5.2: See https://github.com/lydell/source-map-resolve#deprecated
npm warn deprecated har-validator@2.0.6: this library is no longer supported
npm warn deprecated mkdirp@0.5.1: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
npm warn deprecated hoek@2.16.3: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated request@2.79.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated request@2.88.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated request@2.67.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated readdir-scoped-modules@1.0.2: This functionality has been moved to @npmcli/fs
npm warn deprecated hawk@1.0.0: This module moved to @hapi/hawk. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated hawk@3.1.3: This module moved to @hapi/hawk. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated jade@0.26.3: Jade has been renamed to pug, please install the latest version of pug instead of jade
npm warn deprecated swig@1.4.2: This package is no longer maintained
npm warn deprecated bson@1.0.9: Fixed a critical issue with BSON serialization documented in CVE-2019-2391, see https://bit.ly/2KcpXdo for more details
npm warn deprecated nodeunit@0.9.5: you are strongly encouraged to use other testing options

added 962 packages, and audited 1412 packages in 13s

32 packages are looking for funding
  run `npm fund` for details

137 vulnerabilities (9 low, 35 moderate, 57 high, 36 critical)

To address issues that do not require attention, run:
  npm audit fix

To address all issues possible (including breaking changes), run:
  npm audit fix --force

Some issues need review, and may require choosing
a different dependency.

Run `npm audit` for details.
[Pipeline] }
[Pipeline] // dir
[Pipeline] }
[Pipeline] // script
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (polaris-detailed-workflow)
[Pipeline] script
[Pipeline] {
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm
[Pipeline] {
[Pipeline] security_scan
**************************** START EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Security Scan] INFO: Jenkins Job name: MBP_Github_Coverity_Detailed_Sample
-------------------------------- Connection to node --------------------------------
[Security Scan] INFO: Jenkins job is running on agent node remotely
-------------------------- Parameter Validation Initiated --------------------------
[Security Scan] INFO:  --- product = [COVERITY]
[Security Scan] INFO: Parameters for coverity:
[Security Scan] INFO:  --- coverity_passphrase = ******************************************************************************
[Security Scan] INFO:  --- coverity_waitForScan = true
[Security Scan] INFO:  --- coverity_clean_command = npm cache clean --force
[Security Scan] INFO:  --- coverity_prComment_enabled = true
[Security Scan] INFO:  --- coverity_url = https://integrations-qa.dev.cnc.duckutil.net
[Security Scan] INFO:  --- coverity_prComment_impacts = HIGH, MEDIUM
[Security Scan] INFO:  --- coverity_user = admin
[Security Scan] INFO:  --- coverity_build_command = npm install
------------------------------------------------------------------------------------
[Security Scan] INFO: Parameters for additional configuration:
[Security Scan] INFO:  --- network_ssl_trustAll = false
[Security Scan] INFO:  --- mark_build_status = SUCCESS
[Security Scan] INFO:  --- network_airgap = false
[Security Scan] INFO: Coverity parameters are validated successfully
[Security Scan] INFO: Bridge download parameters are validated successfully
[Security Scan] INFO: Bridge download is not required. Found installed in: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
------------------------------------------------------------------------------------
[Security Scan] INFO: Bridge CLI version is - 3.9.2
[Security Scan] INFO: Jenkins Job name: MBP_Github_Coverity_Detailed_Sample
[Security Scan] INFO: Coverity Project Name: detailed-example
[Security Scan] INFO: Coverity Stream Name: detailed-example-main
[Security Scan] INFO: Coverity PR Comment is ignored for non pull request scan
[Security Scan] INFO: Jenkins Job name: MBP_Github_Coverity_Detailed_Sample
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage connect --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/coverity_input4364128528095459070.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-13 21:22:03.6836 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-13 21:22:03.6960 IST [Bridge CLI] INFO: Found version "3.0.128" in registry for workflow "connect", trying to load it from local cache
2025-11-13 21:22:03.7585 IST [Bridge CLI] INFO: Input Resources:
2025-11-13 21:22:03.7586 IST [Bridge CLI] INFO: resource = value [source]
2025-11-13 21:22:03.7586 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 21:22:03.7586 IST [Bridge CLI] INFO: coverity.build.command = npm install [coverity_input4364128528095459070.json]
2025-11-13 21:22:03.7586 IST [Bridge CLI] INFO: coverity.clean.command = npm cache clean --force [coverity_input4364128528095459070.json]
2025-11-13 21:22:03.7586 IST [Bridge CLI] INFO: coverity.connect.project.name = detailed-example [coverity_input4364128528095459070.json]
2025-11-13 21:22:03.7586 IST [Bridge CLI] INFO: coverity.connect.stream.name = detailed-example-main [coverity_input4364128528095459070.json]
2025-11-13 21:22:03.7586 IST [Bridge CLI] INFO: coverity.connect.url = https://integrations-qa.dev.cnc.duckutil.net [coverity_input4364128528095459070.json]
2025-11-13 21:22:03.7586 IST [Bridge CLI] INFO: coverity.connect.user.name = admin [coverity_input4364128528095459070.json]
2025-11-13 21:22:03.7586 IST [Bridge CLI] INFO: coverity.connect.user.password = ***************************************** [coverity_input4364128528095459070.json]
2025-11-13 21:22:03.7587 IST [Bridge CLI] INFO: coverity.waitForScan = true [coverity_input4364128528095459070.json]
2025-11-13 21:22:03.7587 IST [Bridge CLI] INFO: network.airgap = false [coverity_input4364128528095459070.json]
2025-11-13 21:22:03.7587 IST [Bridge CLI] INFO: network.ssl.trustAll = false [coverity_input4364128528095459070.json]
2025-11-13 21:22:03.7587 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 21:22:03.7587 IST [Bridge CLI] INFO: Starting adapters for stage connect
2025-11-13 21:22:03.7590 IST [Bridge CLI] INFO: Starting Adapter: Coverity Connect Controller
2025-11-13 21:22:03.7631 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-13 21:22:03.7918 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-13 21:22:03.7921 IST [Check pull request] INFO: Adapter finished
2025-11-13 21:22:06.1689 IST [Coverity Connect Controller] INFO: No coverity version is configured, will use the default or latest supported version from the server
2025-11-13 21:22:06.2165 IST [Coverity Connect Controller] INFO: Provided value for resource 'coverity.execution.path'
2025-11-13 21:22:06.2166 IST [Bridge CLI] INFO: Starting adapters for stage connect-post-processing
2025-11-13 21:22:06.2166 IST [Bridge CLI] INFO: Starting adapters for stage scm
2025-11-13 21:22:06.2166 IST [Bridge CLI] INFO: Starting adapters for stage connect-scan
2025-11-13 21:22:06.2170 IST [Bridge CLI] INFO: Starting Adapter: Coverity Connect Scan
2025-11-13 21:22:06.2170 IST [Bridge CLI] INFO: Starting Adapter: Coverity Connect Post Scan
2025-11-13 21:22:06.2171 IST [Bridge CLI] INFO: Starting Adapter: SCM Checker
2025-11-13 21:22:06.2173 IST [Coverity Connect Controller] INFO: Adapter finished
2025-11-13 21:22:06.2240 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for Set Version for Coverity
2025-11-13 21:22:06.2243 IST [Default Adapter for Set Version for Coverity] INFO: Provided value for resource 'coverity.version'
2025-11-13 21:22:06.2244 IST [Default Adapter for Set Version for Coverity] INFO: Adapter finished
2025-11-13 21:22:06.2842 IST [Coverity Connect Scan] INFO: Identified workflow: Coverity
2025-11-13 21:22:06.2843 IST [Coverity Connect Scan] INFO: command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity scan --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir -o capture.build.clean-command=npm cache clean --force -o analyze.location=connect -o commit.connect.url=https://integrations-qa.dev.cnc.duckutil.net -o commit.connect.stream=detailed-example-main -o commit.connect.project=detailed-example -- npm install
2025-11-13 21:22:06.3432 IST [Coverity Connect Scan] INFO: coverity 2025.9.0 covcli-2025.9-push-12
2025-11-13 21:22:06.3438 IST [Coverity Connect Scan] WARNING: No setting for 'commit.connect.on-new-cert' specified.
2025-11-13 21:22:06.3438 IST [Coverity Connect Scan] WARNING: Using default value of 'distrust'.
2025-11-13 21:22:06.3438 IST [Coverity Connect Scan] WARNING: This may result in a certificate validation error when uploading defects to Coverity Connect.
2025-11-13 21:22:06.3438 IST [Coverity Connect Scan] WARNING: If you trust the Coverity Connect instance and certificate validation fails, set 'commit.connect.on-new-cert' to 'trust'.
2025-11-13 21:22:06.3438 IST [Coverity Connect Scan] WARNING: If you are unfamiliar with what this means, please talk to your Coverity Connect administrator.
2025-11-13 21:22:06.3464 IST [Coverity Connect Scan] INFO: Detected that stdout is not connected to a terminal.  Defaulting ticker mode to 'none'.
2025-11-13 21:22:06.3464 IST [Coverity Connect Scan] INFO: If this is not correct, explicitly set the ticker mode to the desired value using the '--ticker-mode' option.
2025-11-13 21:22:06.3471 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir create
2025-11-13 21:22:08.1650 IST [Coverity Connect Scan] INFO: Cloud analysis is enabled.
2025-11-13 21:22:11.4114 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-manage-cache check
2025-11-13 21:22:12.3189 IST [Coverity Connect Scan] INFO: Caching is enabled.
2025-11-13 21:22:13.7073 IST [Coverity Connect Scan] INFO: Telemetry is enabled
2025-11-13 21:22:14.2311 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir list-capture-diagnostics
2025-11-13 21:22:14.2448 IST [Coverity Connect Scan] INFO: Executing action no-op: nothing to do for initialization
2025-11-13 21:22:14.7331 IST [Coverity Connect Scan] INFO: Executing action Delete compiler configurations for intermediate directory '/Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir'
2025-11-13 21:22:14.7332 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler gcc --comptype clangcc --template
2025-11-13 21:22:14.9635 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler cc --comptype gcc --template
2025-11-13 21:22:15.2049 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler c++ --comptype g++ --template
2025-11-13 21:22:15.4590 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler clang --comptype clangcc --template
2025-11-13 21:22:15.7099 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler java --comptype java --template
2025-11-13 21:22:15.9624 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler go --comptype go --template
2025-11-13 21:22:16.2151 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler ccache --comptype prefix --template
2025-11-13 21:22:16.4637 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler kotlinc --comptype kotlinc --template
2025-11-13 21:22:16.6973 IST [Coverity Connect Scan] WARNING: Template config template-java-config-0 already exists for java and will be reused. 
2025-11-13 21:22:16.6973 IST [Coverity Connect Scan] WARNING: Template config template-apt-config-0 already exists for apt and will be reused. 
2025-11-13 21:22:16.6973 IST [Coverity Connect Scan] WARNING: Template config template-javaw-config-0 already exists for javaw and will be reused. 
2025-11-13 21:22:16.7024 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --dart
2025-11-13 21:22:16.9606 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --javascript
2025-11-13 21:22:17.2089 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --php
2025-11-13 21:22:17.4614 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --python
2025-11-13 21:22:17.7114 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ruby
2025-11-13 21:22:17.9606 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --comptype capture-config-files --file-regex $capture-config-files$ --template
2025-11-13 21:22:17.9781 IST [Coverity Connect Scan] WARNING: Configuration already exists for file regex $capture-config-files$
2025-11-13 21:22:17.9782 IST [Coverity Connect Scan] INFO:           and it will not be updated.
2025-11-13 21:22:18.4724 IST [Coverity Connect Scan] INFO: Executing action no-op: no compilers need to be unconfigured
2025-11-13 21:22:18.9516 IST [Coverity Connect Scan] INFO: Executing action no-op: compiler configurations loaded
2025-11-13 21:22:19.4648 IST [Coverity Connect Scan] INFO: Executing action Execute clean command: sh -c npm cache clean --force
2025-11-13 21:22:19.6195 IST [Coverity Connect Scan] INFO: npm warn using --force Recommended protections disabled.
2025-11-13 21:22:20.9160 IST [Coverity Connect Scan] INFO: Executing action Invoke build capture: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-build --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --append-log --no-security-da --record-with-source --enable-scan-transparency-data --bytecode-caching --force npm install
2025-11-13 21:22:20.9581 IST [Coverity Connect Scan] INFO: Coverity Build Capture (64-bit) version 2025.9.0 on Darwin 24.6.0 arm64
2025-11-13 21:22:20.9581 IST [Coverity Connect Scan] INFO: Internal version numbers: 477d3c5ddd p-2025.9-push-57
2025-11-13 21:22:20.9582 IST [Coverity Connect Scan] INFO: 
2025-11-13 21:22:20.9723 IST [Coverity Connect Scan] INFO: 
2025-11-13 21:23:16.6361 IST [Coverity Connect Scan] INFO: npm warn deprecated resolve-url@0.2.1: https://github.com/lydell/resolve-url#deprecated
2025-11-13 21:23:16.6528 IST [Coverity Connect Scan] INFO: npm warn deprecated source-map-url@0.4.1: See https://github.com/lydell/source-map-url#deprecated
2025-11-13 21:23:16.6535 IST [Coverity Connect Scan] INFO: npm warn deprecated urix@0.1.0: Please see https://github.com/lydell/urix#deprecated
2025-11-13 21:23:17.1540 IST [Coverity Connect Scan] INFO: npm warn deprecated source-map-resolve@0.5.3: See https://github.com/lydell/source-map-resolve#deprecated
2025-11-13 21:23:18.6596 IST [Coverity Connect Scan] INFO: npm warn deprecated stable@0.1.8: Modern JS already guarantees Array#sort() is a stable sort, so this library is deprecated. See the compatibility table on MDN: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort#browser_compatibility
2025-11-13 21:23:18.9154 IST [Coverity Connect Scan] INFO: npm warn deprecated try-resolve@1.0.1: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 21:23:19.0842 IST [Coverity Connect Scan] INFO: npm warn deprecated babel-plugin-undefined-to-void@1.1.6: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 21:23:19.1080 IST [Coverity Connect Scan] INFO: npm warn deprecated babel-plugin-remove-debugger@1.0.1: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 21:23:19.1213 IST [Coverity Connect Scan] INFO: npm warn deprecated babel-plugin-remove-console@1.0.1: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 21:23:19.1326 IST [Coverity Connect Scan] INFO: npm warn deprecated babel-plugin-react-display-name@1.0.3: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 21:23:19.1446 IST [Coverity Connect Scan] INFO: npm warn deprecated babel-plugin-runtime@1.0.7: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 21:23:19.1542 IST [Coverity Connect Scan] INFO: npm warn deprecated babel-plugin-jscript@1.0.4: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 21:23:19.1617 IST [Coverity Connect Scan] INFO: npm warn deprecated babel-plugin-react-constant-elements@1.0.3: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 21:23:19.1621 IST [Coverity Connect Scan] INFO: npm warn deprecated babel-plugin-proto-to-assign@1.0.4: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 21:23:19.1995 IST [Coverity Connect Scan] INFO: npm warn deprecated babel-plugin-property-literals@1.0.1: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 21:23:19.2793 IST [Coverity Connect Scan] INFO: npm warn deprecated babel-plugin-member-expression-literals@1.0.1: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 21:23:19.3314 IST [Coverity Connect Scan] INFO: npm warn deprecated babel-plugin-constant-folding@1.0.1: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 21:23:19.3488 IST [Coverity Connect Scan] INFO: npm warn deprecated babel-plugin-eval@1.0.1: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 21:23:19.3765 IST [Coverity Connect Scan] INFO: npm warn deprecated babel-plugin-inline-environment-variables@1.0.1: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 21:23:19.4090 IST [Coverity Connect Scan] INFO: npm warn deprecated babel-plugin-dead-code-elimination@1.0.2: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
2025-11-13 21:23:20.3533 IST [Coverity Connect Scan] INFO: npm warn deprecated q@0.8.12: You or someone you depend on is using Q, the JavaScript Promise library that gave JavaScript developers strong feelings about promises. They can almost certainly migrate to the native JavaScript promise now. Thank you literally everyone for joining me in this bet against the odds. Be excellent to each other.
2025-11-13 21:23:20.3534 IST [Coverity Connect Scan] INFO: npm warn deprecated
2025-11-13 21:23:20.3534 IST [Coverity Connect Scan] INFO: npm warn deprecated (For a CapTP with native promises, see @endo/eventual-send and @endo/captp)
2025-11-13 21:23:21.2227 IST [Coverity Connect Scan] INFO: npm warn deprecated json3@3.3.2: Please use the native JSON object instead of JSON 3
2025-11-13 21:23:22.1408 IST [Coverity Connect Scan] INFO: npm warn deprecated constantinople@3.0.2: Please update to at least constantinople 3.1.1
2025-11-13 21:23:22.1483 IST [Coverity Connect Scan] INFO: npm warn deprecated transformers@2.1.0: Deprecated, use jstransformer
2025-11-13 21:23:23.1127 IST [Coverity Connect Scan] INFO: npm warn deprecated inflight@1.0.6: This module is not supported, and leaks memory. Do not use it. Check out lru-cache if you want a good and tested way to coalesce async requests by a key value, which is much more comprehensive and powerful.
2025-11-13 21:23:23.1529 IST [Coverity Connect Scan] INFO: npm warn deprecated circular-json@0.3.3: CircularJSON is in maintenance only, flatted is its successor.
2025-11-13 21:23:23.1744 IST [Coverity Connect Scan] INFO: npm warn deprecated rimraf@2.6.3: Rimraf versions prior to v4 are no longer supported
2025-11-13 21:23:24.0104 IST [Coverity Connect Scan] INFO: npm warn deprecated coffee-script@1.12.7: CoffeeScript on NPM has moved to "coffeescript" (no hyphen)
2025-11-13 21:23:24.0478 IST [Coverity Connect Scan] INFO: npm warn deprecated glob@7.2.3: Glob versions prior to v9 are no longer supported
2025-11-13 21:23:24.6020 IST [Coverity Connect Scan] INFO: npm warn deprecated core-js@2.6.12: core-js@<3.23.3 is no longer maintained and not recommended for usage due to the number of issues. Because of the V8 engine whims, feature detection in old core-js versions could cause a slowdown up to 100x even if nothing is polyfilled. Some versions have web compatibility issues. Please, upgrade your dependencies to the actual version of core-js.
2025-11-13 21:23:25.1966 IST [Coverity Connect Scan] INFO: npm warn deprecated swig@1.4.2: This package is no longer maintained
2025-11-13 21:23:25.6418 IST [Coverity Connect Scan] INFO: npm warn deprecated jade@1.11.0: Jade has been renamed to pug, please install the latest version of pug instead of jade
2025-11-13 21:23:25.9822 IST [Coverity Connect Scan] INFO: npm warn deprecated eslint@3.19.0: This version is no longer supported. Please see https://eslint.org/version-support for other options.
2025-11-13 21:23:26.9970 IST [Coverity Connect Scan] INFO: npm warn deprecated q@1.5.1: You or someone you depend on is using Q, the JavaScript Promise library that gave JavaScript developers strong feelings about promises. They can almost certainly migrate to the native JavaScript promise now. Thank you literally everyone for joining me in this bet against the odds. Be excellent to each other.
2025-11-13 21:23:26.9970 IST [Coverity Connect Scan] INFO: npm warn deprecated
2025-11-13 21:23:26.9971 IST [Coverity Connect Scan] INFO: npm warn deprecated (For a CapTP with native promises, see @endo/eventual-send and @endo/captp)
2025-11-13 21:23:27.0344 IST [Coverity Connect Scan] INFO: npm warn deprecated glob@5.0.15: Glob versions prior to v9 are no longer supported
2025-11-13 21:23:27.3707 IST [Coverity Connect Scan] INFO: npm warn deprecated core-js@1.2.7: core-js@<3.23.3 is no longer maintained and not recommended for usage due to the number of issues. Because of the V8 engine whims, feature detection in old core-js versions could cause a slowdown up to 100x even if nothing is polyfilled. Some versions have web compatibility issues. Please, upgrade your dependencies to the actual version of core-js.
2025-11-13 21:23:27.5819 IST [Coverity Connect Scan] INFO: npm warn deprecated q@1.5.1: You or someone you depend on is using Q, the JavaScript Promise library that gave JavaScript developers strong feelings about promises. They can almost certainly migrate to the native JavaScript promise now. Thank you literally everyone for joining me in this bet against the odds. Be excellent to each other.
2025-11-13 21:23:27.5819 IST [Coverity Connect Scan] INFO: npm warn deprecated
2025-11-13 21:23:27.5819 IST [Coverity Connect Scan] INFO: npm warn deprecated (For a CapTP with native promises, see @endo/eventual-send and @endo/captp)
2025-11-13 21:23:27.7475 IST [Coverity Connect Scan] INFO: npm warn deprecated minimatch@0.3.0: Please update to minimatch 3.0.2 or higher to avoid a RegExp DoS issue
2025-11-13 21:23:27.8075 IST [Coverity Connect Scan] INFO: npm warn deprecated glob@3.2.11: Glob versions prior to v9 are no longer supported
2025-11-13 21:23:28.5189 IST [Coverity Connect Scan] INFO: npm warn deprecated core-js@1.2.7: core-js@<3.23.3 is no longer maintained and not recommended for usage due to the number of issues. Because of the V8 engine whims, feature detection in old core-js versions could cause a slowdown up to 100x even if nothing is polyfilled. Some versions have web compatibility issues. Please, upgrade your dependencies to the actual version of core-js.
2025-11-13 21:23:28.6132 IST [Coverity Connect Scan] INFO: npm warn deprecated glob@7.1.1: Glob versions prior to v9 are no longer supported
2025-11-13 21:23:28.6253 IST [Coverity Connect Scan] INFO: npm warn deprecated mkdirp@0.5.1: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
2025-11-13 21:23:29.0339 IST [Coverity Connect Scan] INFO: npm warn deprecated mkdirp@0.3.0: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
2025-11-13 21:23:29.3997 IST [Coverity Connect Scan] INFO: npm warn deprecated fsevents@1.2.13: Upgrade to fsevents v2 to mitigate potential security issues
2025-11-13 21:23:29.5051 IST [Coverity Connect Scan] INFO: npm warn deprecated minimatch@2.0.10: Please update to minimatch 3.0.2 or higher to avoid a RegExp DoS issue
2025-11-13 21:23:29.8770 IST [Coverity Connect Scan] INFO: npm warn deprecated core-js@1.2.7: core-js@<3.23.3 is no longer maintained and not recommended for usage due to the number of issues. Because of the V8 engine whims, feature detection in old core-js versions could cause a slowdown up to 100x even if nothing is polyfilled. Some versions have web compatibility issues. Please, upgrade your dependencies to the actual version of core-js.
2025-11-13 21:24:58.8103 IST [Coverity Connect Scan] INFO: 
2025-11-13 21:24:58.8103 IST [Coverity Connect Scan] INFO: added 737 packages, and audited 738 packages in 3m
2025-11-13 21:24:58.8103 IST [Coverity Connect Scan] INFO: 
2025-11-13 21:24:58.8103 IST [Coverity Connect Scan] INFO: 25 packages are looking for funding
2025-11-13 21:24:58.8104 IST [Coverity Connect Scan] INFO:   run `npm fund` for details
2025-11-13 21:24:58.8518 IST [Coverity Connect Scan] INFO: 
2025-11-13 21:24:58.8518 IST [Coverity Connect Scan] INFO: 49 vulnerabilities (1 low, 10 moderate, 19 high, 19 critical)
2025-11-13 21:24:58.8518 IST [Coverity Connect Scan] INFO: 
2025-11-13 21:24:58.8518 IST [Coverity Connect Scan] INFO: To address issues that do not require attention, run:
2025-11-13 21:24:58.8518 IST [Coverity Connect Scan] INFO:   npm audit fix
2025-11-13 21:24:58.8518 IST [Coverity Connect Scan] INFO: 
2025-11-13 21:24:58.8518 IST [Coverity Connect Scan] INFO: To address all issues possible (including breaking changes), run:
2025-11-13 21:24:58.8519 IST [Coverity Connect Scan] INFO:   npm audit fix --force
2025-11-13 21:24:58.8519 IST [Coverity Connect Scan] INFO: 
2025-11-13 21:24:58.8519 IST [Coverity Connect Scan] INFO: Some issues need review, and may require choosing
2025-11-13 21:24:58.8519 IST [Coverity Connect Scan] INFO: a different dependency.
2025-11-13 21:24:58.8519 IST [Coverity Connect Scan] INFO: 
2025-11-13 21:24:58.8519 IST [Coverity Connect Scan] INFO: Run `npm audit` for details.
2025-11-13 21:24:59.1191 IST [Coverity Connect Scan] INFO: Attempting to detect unconfigured compilers in build
2025-11-13 21:24:59.1261 IST [Coverity Connect Scan] INFO: |0----------25-----------50----------75---------100|
2025-11-13 21:24:59.2369 IST [Coverity Connect Scan] INFO: ****************************************************
2025-11-13 21:24:59.2621 IST [Coverity Connect Scan] WARNING: Recorded 0 C/C++ compilation units (0%) successfully. These compilation units are ready for replay
2025-11-13 21:24:59.2621 IST [Coverity Connect Scan] WARNING: Recoverable errors were encountered during 1 of these C/C++ compilation units.
2025-11-13 21:24:59.2621 IST [Coverity Connect Scan] INFO: 
2025-11-13 21:24:59.2621 IST [Coverity Connect Scan] INFO:  For more details, please look at: 
2025-11-13 21:24:59.2622 IST [Coverity Connect Scan] INFO:     /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/build-log.txt
2025-11-13 21:24:59.3358 IST [Coverity Connect Scan] INFO: Executing action Collect Build Metrics
2025-11-13 21:24:59.3361 IST [Coverity Connect Scan] INFO: Executing action Invalidate capture results
2025-11-13 21:24:59.3362 IST [Coverity Connect Scan] INFO: Executing action Update uncaptured file timestamps for project "/Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/node_modules/consolidate/Makefile"
2025-11-13 21:24:59.3364 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir list-capture-diagnostics
2025-11-13 21:25:00.4310 IST [Coverity Connect Scan] INFO: Executing action Emit files using buildless capture: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-capture-files --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ticker-mode none --append-log --capture-list-file /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/capture-file-list-3696101163 --record-with-source
2025-11-13 21:25:00.4556 IST [Coverity Connect Scan] INFO: Buildless capture started.
2025-11-13 21:25:00.4702 IST [Coverity Connect Scan] INFO: Emitting 84 Files.
2025-11-13 21:25:00.9177 IST [Coverity Connect Scan] INFO: Buildless capture completed.
2025-11-13 21:25:00.9195 IST [Coverity Connect Scan] INFO: Executing action Delete unwanted TUs: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit @@/Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/delete-unwanted-tus-action-422214411
2025-11-13 21:25:00.9391 IST [Coverity Connect Scan] INFO: Executing action Action cleanup: Unwanted TUs action cleanup
2025-11-13 21:25:00.9392 IST [Coverity Connect Scan] INFO: Executing action deleteResidualTUs /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir
2025-11-13 21:25:00.9394 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir list-capture-diagnostics
2025-11-13 21:25:00.9559 IST [Coverity Connect Scan] INFO: Executing action Invalidate capture results
2025-11-13 21:25:01.9176 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir list-capture-diagnostics
2025-11-13 21:25:02.0079 IST [Coverity Connect Scan] INFO: Capture summary:
2025-11-13 21:25:02.0079 IST [Coverity Connect Scan] INFO:     SUCCEEDED: 84
2025-11-13 21:25:02.0079 IST [Coverity Connect Scan] INFO:     INCOMPLETE: 0
2025-11-13 21:25:02.0079 IST [Coverity Connect Scan] INFO:     FAILED: 0
2025-11-13 21:25:02.0079 IST [Coverity Connect Scan] INFO:     IGNORED: 6
2025-11-13 21:25:02.0079 IST [Coverity Connect Scan] INFO:     FILES CAPTURED: 84
2025-11-13 21:25:02.0080 IST [Coverity Connect Scan] INFO:     LINES OF CODE: 32728
2025-11-13 21:25:02.0110 IST [Coverity Connect Scan] INFO: Capture phase took 2m48.308s.
2025-11-13 21:25:02.0112 IST [Coverity Connect Scan] INFO: Loading compiler config '/Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml'
2025-11-13 21:25:02.0136 IST [Coverity Connect Scan] INFO: Loading compiler config '/Users/madhusud/Jenkins_Testing/Nodes/workspace/ub_Coverity_Detailed_Sample_main@2/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml'
2025-11-13 21:25:02.0146 IST [Coverity Connect Scan] INFO: Analyzing project in the cloud using Coverity Analysis version 2025.9.0
2025-11-13 21:25:02.8126 IST [Coverity Connect Scan] INFO: Creating archive containing data to be analyzed...
2025-11-13 21:25:02.9246 IST [Coverity Connect Scan] INFO: Properties archive created.
2025-11-13 21:25:02.9247 IST [Coverity Connect Scan] INFO: Uploading data for analysis...
2025-11-13 21:25:03.6132 IST [Coverity Connect Scan] INFO: |0----------25-----------50----------75---------100|
2025-11-13 21:25:10.1507 IST [Coverity Connect Scan] INFO: ****************************************************
2025-11-13 21:25:10.1508 IST [Coverity Connect Scan] INFO: Scan created.
2025-11-13 21:25:10.1509 IST [Coverity Connect Scan] INFO: The scan ID is '204eab93-c48e-41ae-9a10-04b71492e33f'
2025-11-13 21:25:10.1512 IST [Coverity Connect Scan] INFO: Waiting for scan to complete...
2025-11-13 21:25:10.1512 IST [Coverity Connect Scan] INFO: |0----------25-----------50----------75---------100|
2025-11-13 21:26:57.7317 IST [Coverity Connect Scan] INFO: ****************************************************
2025-11-13 21:26:58.4358 IST [Coverity Connect Scan] INFO: Analysis summary after merging defects:
2025-11-13 21:26:58.4360 IST [Coverity Connect Scan] INFO:     HIGH SEVERITY:    2 issue(s)
2025-11-13 21:26:58.4360 IST [Coverity Connect Scan] INFO:     MEDIUM SEVERITY: 12 issue(s)
2025-11-13 21:26:58.4360 IST [Coverity Connect Scan] INFO:     LOW SEVERITY:    25 issue(s)
2025-11-13 21:26:58.4361 IST [Coverity Connect Scan] INFO:     AUDIT SEVERITY:   0 issue(s)
2025-11-13 21:26:58.4361 IST [Coverity Connect Scan] INFO: Results are available at https://integrations-qa.dev.cnc.duckutil.net:443/query/defects.htm?stream=detailed-example-main&outstanding=true
2025-11-13 21:26:58.4376 IST [Coverity Connect Scan] INFO: Analyze phase took 1m56.42s.
2025-11-13 21:26:58.4413 IST [Coverity Connect Scan] WARNING: !! SOURCES FOR UNSUPPORTED LANGUAGES WERE DETECTED !!
2025-11-13 21:26:58.4414 IST [Coverity Connect Scan] WARNING: 
2025-11-13 21:26:58.4416 IST [Coverity Connect Scan] WARNING: Source files for the following languages were detected, but these languages are not supported on Mac OS ARM:
2025-11-13 21:26:58.4416 IST [Coverity Connect Scan] WARNING:   * C#
2025-11-13 21:26:58.4422 IST [Coverity Connect Scan] WARNING: In order to analyze these files, please analyze the project on an operating system and architecture where they are supported.
2025-11-13 21:26:58.4423 IST [Coverity Connect Scan] INFO: Scan complete.
2025-11-13 21:26:58.4525 IST [Coverity Connect Scan] INFO: Coverity Capture completed successfully
2025-11-13 21:26:58.4643 IST [Coverity Connect Scan] INFO: Provided value for resource 'coverity.completed'
2025-11-13 21:26:58.4644 IST [Coverity Connect Scan] INFO: Provided value for resource 'coverity.idir.output'
2025-11-13 21:26:58.4649 IST [Coverity Connect Scan] INFO: Adapter finished
2025-11-13 21:26:58.5228 IST [SCM Checker] INFO: Adapter finished
2025-11-13 21:27:00.1453 IST [Coverity Connect Post Scan] INFO: Provided value for resource 'coverity.connect.resultURL'
2025-11-13 21:27:00.1455 IST [Coverity Connect Post Scan] INFO: Provided value for resource 'coverity.connect.policy.issueCount'
2025-11-13 21:27:00.1463 IST [Coverity Connect Post Scan] INFO: Adapter finished
******************************* END EXECUTION OF BRIDGE CLI *******************************
[Security Scan] INFO: Retrieving the issue count from the scan results
[Security Scan] INFO: Total issues found: 39
[Security Scan] INFO: Security Scan execution is successful
[Security Scan] INFO: Marking build status as SUCCESS is ignored since exit code is: 0
**************************** END EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Pipeline] }
[Pipeline] // dir
[Pipeline] }
[Pipeline] // script
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (Declarative: Post Actions)
[Pipeline] echo
Black Duck Logs Publisher - Starting log upload process
[Pipeline] echo
Configuration: [githubOrg:coverity-cnc-jenkins-samples, repoName:detailed-example, credentialsId:github-pat-logs-publisher, maxRetries:3, retentionCount:5, jobNamePrefixes:[MBP_Github_, MBP_, Github_, Pipeline_, Job_, Build_]]
[Pipeline] echo
Job Name: MBP_Github_Coverity_Detailed_Sample/main
[Pipeline] echo
Build Number: 2
[Pipeline] echo
GitHub Organization: coverity-cnc-jenkins-samples
[Pipeline] withCredentials
Masking supported pattern matches of $GITHUB_TOKEN
[Pipeline] {
[Pipeline] echo
Using configured repository name: detailed-example
[Pipeline] echo
Target repository: coverity-cnc-jenkins-samples/detailed-example
[Pipeline] echo
LogProcessor: captureJenkinsLogs called
```

---

*Log generated by Black Duck Logs Publisher*