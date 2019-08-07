# AEM
AEM Authentication Support
https://helpx.adobe.com/experience-manager/kt/platform-repository/using/authentication-support-article-understand.html
Basic
TokenBased
Form Based
http://localhost:4502/system/console/configMgr/org.apache.sling.engine.impl.auth.SlingAuthenticator

Publish Server
https://docs.adobe.com/docs/en/aem/6-1/administer/security/encapsulated-token.html
AEM uses the Token Authentication Handler to authenticate each request. However, in order to serve authentication requests the Token Authentication Handler requires access to the repository for every request. This happens because cookies are used to maintain the authentication state. Logically, the state needs to be persisted in the repository in order to validate subsequent requests. In effect, this means that the authentication mechanism is stateful.
