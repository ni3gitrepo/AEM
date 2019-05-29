
final Logger logger = LoggerFactory.getLogger("libs.granite.ui.components.shell.propertiespage");
logger.debug("Render starts");

## AEM

java -Xmx512m -agentlib:jdwp=transport=dt_socket,address=30303,server=y,suspend=n -jar cq5-author-p4502.jar

AEM Timeline Activity Stream 

Timeline data comes from 

/var/audit/com.day.cq.dam/content/dam
https://helpx.adobe.com/experience-manager/6-3/assets/using/activity-stream.html

enable - Day CQ DAM Event Recorder
Enable - set isEnabled.name = true in DAM Asset Home Page Feature Flag
https://helpx.adobe.com/experience-manager/6-4/assets/using/assets-home-page.html
https://helpx.adobe.com/experience-manager/6-4/sites/authoring/using/user-properties.html

dam ASSET expiration date

./jcr:content/metadata/prism:expirationDate



====================
## windows powershell

get-help cmdlets or cmdlets -?(get-help get-content) or (get-content - ?)

get-command -verb get

get-help get-service – examples

get-content alieas gc/cat/type

get-content error.log -tail 100

PS C:\> Get-Content error.log -first 15 | Out-Gridview

PS C:\> Get-Content .\IISwebsite.log | ? {($_ | Select-String “HttpError”)}

PS C:\> Get-Content .\IISwebsite.log | ? {($_ | Select-String “HttpError”)} | Out-file 'path\file.log'

Get-Content -Path "C:\scripts\test.txt" -Wait

Get-Content ./log.log -Wait -Tail 10

Get-Content error.log | ? {($_ | Select-String “Exception”)}
gc error.log | ? {($_ | sls "replication")}

clear-content error.log (delete all data)

GriedView
gc error.log -tail 50 | ogv
=======================================================
## HTL cheatsheet

========================================================

./jcr:content/metadata/predictedTags
/conf/global/settings/dam/adminui-extension/metadataschema/common-metadata

##Splunk
=============== S P L U N K Search -===========================splunk
index="*" host="xaclddamauth1p.healthehost.com" "laadn@aetna.com"

index="*" host="aemdamauth1d.healthehostt.com" "laadn@aetna.com"

index="*" host="xaclddamauth1d.healthehostt.com" source="/aem/author/crx-quickstart/logs/error.log"

##Node.js
================== Node.js ==========================================
npm install http-server -g
cd MyApp

$ http-server
$ npm install -g light-server 
$ light-server

## VSCODE
JQUERY INSTALLATION
npm install tsd -g
npm install typings --global
typings install dt~jquery --global
<reference path="../typings/globals/jquery/index.d.ts" />


dam/gui/coral/components/admin/schemaforms/formbuilder/sectionfield
============================================= Chrome Dev Tools
##Chrome Dev Tools
Shift + Enter => allow you to write multi line text in console
Logpoint ???
Live Expression ??
chrome debug extension

======================== CHS Mareting Dam

check points for spot name in dialog
	1. Spot service configuration - endpoint, secret key etc
	2. Proxy configuration aem server proxy.aetna.com, 9119
	3. email configuration for logged in user
