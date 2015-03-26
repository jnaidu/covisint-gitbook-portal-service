# Glossary of Terms
1. **Virtual Portal**: A virtual portal is the default for new customer tenancies.  A virtual portal is a separate virtual host and separate java process running virtually in one, multitenant portal instance.
2. **Portlet**: A portlet is a java application running in a portal instance and may be dropped on one or more pages.  See above for the default set of portlets included in a standard portal deployment.
3. **Module Communication Framework**: A framework for exposing functionality from connected applications, data sources or devices through the Portal content management system (CMS) as a published standard set of JavaScript functions and APIs.
4. **Module**: A Module is a self-contained java application component deployed in the portal as a portlet.  A module is integrated with any API-enabled application, data source, or device via any available protocol (SOAP services, REST services, Remote Procedure Call, database connectivity, sockets, etc.).
    * Each Module exposes functionality of the connected application, data source or device through the Portal content management system (CMS) as a published standard set of JavaScript functions.  
    * The modules de-couple the presentation layer from the business logic and integration layers.  By enabling a mock JSON object as a placeholder, user interface (UI) and back-end services development take place in parallel, significantly reducing time to delivery over traditional development
    * With only basic JavaScript skills, almost any user can visualize those application functions as HTML5 applications, right from the CMS. A catalog of functions and objects, along with how to use them are displayed to the user through console.
5. **Content Delivery Network**: An optional add-on to improve page performance by enabling distributed caching over 125,000 global points of presence and proprietary routing algorithms.  Additional options for CDN enhancements exist beyond the items listed in the standard pricing.  Contact a solution architect for additional details.
6. **Content Management System** - A Content Management System (CMS) is a computer program that allows publishing, editing and modifying content as well as maintenance from a central interface. 
7. **Site** – A site is the basic unit for content management and collaboration.  
    * Site Types – Sites can be:
        1. Open – Users can join or leave sites without any approval required
        2. Restricted – Users request access to sites and access is granted by a Site administrator
        3. Private – Users can access Private Sites by invitation only
    * Site Content – Each site has an independent set of content
        1. Web Content
        2. Documents and Media
        3. Blog
        4. Wiki
        5. Forum
        6. Knowledge Base
        7. Local taxonomy
        8. Site Pages
    * Site Roles – Each Site has an independent set of users that can be granted granular access to Site content
        1. Site Administrator – Site administrator is a standard role across all sites that has omni-administrative privileges for a Site, including content administration, page and site administration, and user access administration
        2. Site Member – Site member is a standard role across all sites with basic access to authenticated site content and collaboration functionality
        3. Site Teams – Site Teams are ad hoc roles that can be created on an individual site
8. **Global Site** – A collection of assets that can be leveraged across all sites in a portal.  Global assets are subject to their own workflow. The Global taxonomy is used to drive personalization across the portal.
9. **User Site** – Each User may be provisioned with a User Site that can be exposed as part of the Portal.  User Sites include all of the capabilities of a standard Site
10.	**Page** – An unlimited number of web pages can be created the portal
    * Page Types
        1. Public Pages – Public pages can be exposed to unauthenticated users (Guest) or authenticated users; Users without any role on a site can still see public pages
        2. Private Pages – Private pages can only be seen by users with at least one Site role
    * User Pages – Users can enable private pages and public pages as part of their profile that can include all of the Social Network portlets
    * Site Pages – Each Site has its own set of pages, public and private.  Pages can be individually styled with one of the available page layouts, a unique theme, css, and JavaScript.   
    * Page Layout – A predefined page format that governs the orientation of portlets on a page.  Page Templates can be used to control which sections of a page can be customized by end users
11. **Theme** – Each Covisint portal includes 1 standard theme. Customers can customize the look and feel of the theme according to Covisint’s published Style Guide.  The default Covisint theme has preconfigured responsive and adaptive behaviors to function on a wide array of devices and form factors.
12. **Application** – A piece of software designed to help the user to perform specific tasks, typically deployed in the portal as a portlet or exposed through the CMS as JavaScript via the Module Communication Framework.
13.	**Control Panel** – The core set of functions to set up and manage the virtual portal environment are fully controlled from the UX/UI
14.	**Group** – A Group is used to aggregate a bundle of Regular Roles, Site Roles, or Team Roles in the Portal.  Each CIS Service Package is tied to a Group in Portal.  
15.	**Roles** – Roles are sets of privileges in Portal.  There are three types of Role in Portal
16.	**Search** – Search is Covisint’s implementation of enterprise search in the portal. Covisint’s search is highly differentiated with features such as auto-complete search terms, multi-language support, faceted search, configurable scope and interaction with asset publisher.
17.	**Guided / Queryless Search** – This is a set of functionality that allows the site to respond to a user and provide information back to the user based on a combination of user profile attributes and context. 
18.	**Entity** – Either identity provider (IDP) or service provider (SP).
19.	**Identity** – Collect of information describing a user, person, or machine.
20.	**Service Provider (SP)** – An entity that provides services to principals or other system entities in a federation. Covisint maintains a list of supported catalog applications that defines whether an application is Catalog or Non-catalog.  Standard SPs must support one of the following protocols when CIS acts as an IDP in the federation:
    * SAML 1.1
    * SAML 2.x
    * OAuth 2.0
    * OpenID 2.0
    * OpenID Connect 1.0
    * WS-Federation (Passive profile)
21. **Identity Provider (IDP)** – An entity that creates, maintains, and manages identity information for principals and provides principal authentication to other service providers within a federation, such as with web browser profiles. CIS supports the following standard protocols when acting as an IDP:
    * SAML 1.1
    * SAML 2.x
    * OAuth 2.0
    * OpenID 2.0
    * WS-Federation
    * Facebook Connect
22. **Relying Party (RP)** – Def 1: Synonym for service provider. Def 2: The peer in an IDP / SP exchange, such that, the relying party of the IDP is the SP and vice-versa.
23.	**Service** – Any web-based content that needs to be protected.
24. **Application** – Synonym for service or SP.
25. **Just in Time** – Any process that occurred at the moment that a decision was needed.
26.	**Ahead of Time** – A process that pre-computes a decision prior to its usage.
27.	**Single Sign-on** – The act of using an IDP to create a session at an SP.
28. **Federation** – Describes the technologies, standards and use-cases that serve to enable the portability of identity information across otherwise autonomous security domains.
29. **Synchronization** – Process of reconciling user records between two or more systems.
30.	**Authorization** – Act of determining whether a user should be able to perform an action within a service or application.
31. **Authentication** – The act of providing access to applications or services based upon a credential(s) or attribute(s) of the user.
    * Claims-based – in SharePoint, SAML attributes are referred to as Claims; SharePoint / Microsoft expect the User Identifier to be in one of the Attributes / Claims – and not in the Subject Name Identifier
32.	**Account** – The set of information that defines a registered User in CIS.
33.	**Security Token** - The programmatic “blob” used to authenticate an identity to a resource.  Supported Security Tokens are:
    * Kerberos Ticket
    * SAML Assertion
    * PKI Certificate
    * One-time Password (OTP)
    * Biometric
    * Session Cookie
    * Physical Token
34. **Assertion** – SAML's security token.
35.	**Attribute** – Defined as a specification that is a component of an identity.
36.	**Name Identifier** – The place in a SAML message that carries the unique identifier of a person.
37.	**Registry** – The data store of all users, groups, permissions and services.
38. **LDAP Directory** – Lightweight Directory Access Protocol, defined as an application protocol for accessing and maintaining distributed directory information services over an Internet Protocol (IP) network.  CIS supports LDAPv3 directory service services.
39. **Active Directory** – Microsoft’s directory service for MS Windows domain networks.
40.	**ADFS** – Active Directory Federation Services. Microsoft's AD-based implementation of SAML and WS-Federation.
41. **Authentication Protocols** – Network protocol used to perform sign on to an IDP or SP.  CIS supported protocols include:
    * SAML 1.1, 2.x
    * OpenID 2.0
    * OAuth 2.0
    * WS-Federation
    * Kerberos
    * Facebook Connect
42. **SaaS** – Software as a Service, a Cloud-based application or service that serves in a multi-tenant architecture.
43.	**Covisint Terms**
    * Realm – The collection of all orgs, users and services used by a distinct group of customers.
    * Org – A top-level organization roughly equivalent to a company.
    * Sub Org / Division – A unit representing a division within an organization, for example, a department within a company.
    * Context – A set of configuration information based on the current request, for example, a request coming into customer.covisint.com would receive a set of configuration parameters pointing to their logo, style sheet, etc.
    * Group – Collection of users.
    * Role – A collection of privileges.
    * User – A registered user in a CIS tenancy.
    * Service Package – A collection of services or SPs.
    * Service - A service or application.
    * Privilege – The grantable right to perform an action within a service.
    * Tenancy – The logical portion of the Covisint Cloud infrastructure devoted to a customer.			
44. **IDBridge** – An IDBridge is a component of CIS that is downloaded by the tenant and configured against their enterprise MS Active Directory (AD) or LDAPv3 directory service.  It is a virtual machine image that resides in the customers network de-militarized zone (DMZ) to synchronize their users from MS Active Directory or LDAPv3 directory service.    A single IDBridge can only be linked to one Organization or Department.  Multiple IDBridges can be linked to one Organization or Department.  One IDBridge can connect to one LDAPv3 directory service or AD User Registry.  This allows users to authenticate with their enterprise user credentials and supports desktop single sign-on to the CIS and any of the tenant’s Service Providers. 
    * IDBridge Custom Connector: Covisint offers additional custom connectors for the IDBridge.  The target application must have existing access to the user store via web services or a Java API and the connector will be developed in Java to run on Covisint's IDBridge.
45.	**Provisioning** - CIS is capable of provisioning users into SP or applications either through Just In Time (JIT) or Ahead Of Time (AOT). 
    * Service Provisioning Markup Language (SPML): The destination application must support SPML, messaging transport over HTTP, and accept one of the existing product container options (Ex. BOD)
    * Other Provisioning: Other provisioning methods are available as part of professional services engagements.
46.	**Theme** - Custom look and feel is developed according to the standard theme specifications and involves basic changes to the color scheme and placement of the customer logo.  No modifications to the application functionality or screens may be made.
47.	**Transaction-based Pricing**: Although standard pricing and editions are defined on a per-user or per-month basis, we are also able to offer our products on a consumption model.  Customers can purchase blocks of transactions by Authentication, Outbound SSO (federations), or API calls.  Typically these transactions are purchased for use over a period of time (e.g. authentications per month).  Transaction-based pricing is an alternative to the per-user fee structure; however minimum subscription levels and other line item pricing fees apply to both models.
    * Authentication: A single transaction is defined as the action performed by the system to determine the identity of a User by collecting User credentials, validating the correct entry of User credentials against the User registry, and producing a success or failure response.  User credentials required for authentication include at a minimum, but are not limited to, User Name and Password.
    * Outbound SSO: An Outbound SSO is a secure method of transferring authentication state and optionally user attributes from one Endpoint to another to achieve single sign-on across domains.  When a user is authenticated once and a session already exists, subsequent Outbound SSO connections represent only one transaction. When a user is first authenticated then transferred to the SP, a customer is using two transactions to complete the Outbound SSO (The Broker Edition uses this model for calculating transactions).  
    * SP Initiated SSO: In an SP initiated SSO transaction, a user starts at the SP and the SP issues an authentication request to Covisint.  In this case, the authentication represents two transactions: the authentication with Covisint and the subsequent authentication into the SP.
    * API Transaction: An API Transaction is defined as a single request to and response from one of the published Covisint APIs. 
