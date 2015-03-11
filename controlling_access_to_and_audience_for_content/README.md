# Controlling Access to and Audience for Content
This section describes how to provision a page or portlet with a Service Package or other role.

## Mapping a Role to a Service Package
There are four types of Role:
1. Regular Role – A Regular Role has the same set of privileges across the entire portal, including all sites and organizations.  Giving a privilege to a regular role has the broadest impact
2. Organizational Role – An Organizational Role will give a user a set of privileges in any Organization where the user has that role. An Organizational Role can also be mapped to a Site Role; Note that Organizational Roles cannot be mapped to Service Packages; Organizational Roles can only be granted to Organization Members on specific Organizations
3. Site Role – A Site Role will give a user a set of privileges in any Site where the user has that role
4. Team Role – A Team Role will give a user a set of privileges in the Site where the user has that role; A Team Role is a role specific to only one Site

## To map a role to a service package, follow these steps:
1. Log on to the portal as Portal administrator
2. Navigate to the control Panel
3. Under the Portal section, click on Roles
4. Find the role to which you want to map the service package
    1. Adding and configuring new roles is an advanced task and is not covered in this section
    2. You can add a new role solely for the purpose of mapping a service package to a Role easily
    3. Granting additional Portal privileges to the role is more complicated
    4. To add a Role for mapping to a Service Package, Click Add, then select the type of role you want
    5. Type a name, title and description, then click Save
5. Click the Actions button next to the Role and select Assign Members
6. Click User Groups
7. Click available
8. Check the box next to the User Group that corresponds to the Service Package you want to map to the Role
9. Click Update Associations

On any asset (portlet, page, or piece of content, etc.)  the role will now be available and mapped to the service package when you modify the Permissions for the asset.  For all assets, when editing the asset, you will see a permissions button prominently located.  Some asset types have a shortcut for permissions when the asset is created, then provides access to the complete set of permissions when the asset is edited.  The items in the shortcut menu is configurable or the full menu can be added in both locations.  On portlets, permissions are located on the Portlet Configuration menu, which can be easily accessed when edit controls are enabled.  On a Portlet, click the wrench icon and select Configuration.

## Targeting Content
This section describes the different ways to introduce a piece of web content into an environment. There are several ways to deliver content:
1. Publish content on a single page that is displayed to all users
2. Publish content on a page that is displayed to users of just one customer
3. Publish content on a page that is displayed to users based on context
4. Publish content on a page based on personalization or preference
5. Publish content that can appear on one page, then downstream content managers can choose to display the content in a site or modify the content before it is displayed
6. Content is secured so that only one or more groups or roles can see the content

### Publish content on a single page that is displayed to all users
    * This is the most simple way to publish content.
    * Ease of Publishing: Simple
    * Ease of Administration: Simple
1. Content managers can publish content that is immediately available to all users.
2. A web content article can be created in a location where all users have access to the content 
    1. Global content repository
    2. Site to which all users have access
3. The content is permissioned to a role shared by all users
    1. Power User
    2. User
    3. Guest
4. The article is displayed either in:
    1. Web content display portlet on the Site where the content is stored or on the page where the content is to be displayed
    2. Global content can be displayed on any page
    3. Asset publisher portlet on any site as long as it is scoped to display content from the site where the content is stored

### Publish content on a page that is displayed to users of just one customer
    * This is also a simple way to publish content.
    * Ease of Publishing: Simple
    * Ease of Administration: Simple
1. Content managers can publish content that is immediately available to all members of one particular site
2. A web content article can be created in a specific site 
    1. Site to which all the members have access
    2. Content can be syndicated to another site
        * Only members of the site where the content is published will see it
3. The content is permissioned to a role shared by the site members
    1. Site Member
        * Membership driven by Service Package
4. The article is displayed either in:
    1. Web content display portlet on the Site where the content is stored
        * Global content can be displayed on any page
    2. Asset publisher portlet on any site as long as it is scoped to display content from the site where the content is stored

### Publish content on a page that is displayed to users based on context
    * This is also a simple way to publish content.
    * Ease of Publishing: Simple
    * Ease of Administration: Simple
1. Content managers can publish content that is displayed in a particular context
2. A web content article can be created in a location where users can access it 
    1. Global content repository
    2. Site to which the target users have access
        * Content can be syndicated to another site
3. The content is permissioned appropriately
    1. Site Member/Role
        * Membership driven by Service Package
    2. Guest
4. Categories are applied to the Web Content Article
5. Asset Publisher is configured to display Web Content Articles:
    1. Scope includes site or repository where the Web Content is located
    2. Categories are configured on the Asset Publisher to include the Web Content Article in the display criteria 
    3. The article is displayed in an Asset publisher portlet on any site as long as it is scoped and configured to display content from the site where the content is stored and based on categorization

### Publish content on a page based on personalization or preference
    * This is also a simple way to publish content.
    * Ease of Publishing: Simple
    * Ease of Administration: Medium
1. We do not have the function to apply categories to users in bulk in the POC
    1. Categories can be applied to individual users
2. Content managers can publish content that is displayed in a particular context
3. A web content article can be created in a location where users can access it 
    1. Global content repository
    2. Site to which the target users have access
        * Content can be syndicated to another site
4. The content is permissioned appropriately
    1. Site Member/Role
        * Membership driven by Service Package
    2. Guest
5. Categories are applied to the Web Content Article
6. Asset Publisher is configured to display Web Content Articles:
    1. Scope includes site or repository where the Web Content is located
    2. Categories are configured on the Asset Publisher to include the Web Content Article in the display criteria 
    3. Personalization settings can be configured on the Asset Publisher
        * By selecting a Global vocabulary in Personalization
        * Asset Publisher looks at the categories on the user viewing the page from the selected vocabulary
        * Asset Publisher then displays other assets that have the same categories applied to them as to the user
    4. The article is displayed in an Asset publisher portlet on any site as long as it is scoped and configured to display content from the site where the content is stored and based on categorization


### Publish content that can appear on one page, then downstream content managers can choose to display the content in a site or modify the content before it is displayed
    * This is also a simple way to publish content.
    * Ease of Publishing: Simple
    * Ease of Administration: Medium
1. In this example, the publishing model is the same as number 4 above, with one additional set of steps.
2. When the content is published by the main content manager, a secondary content manager can be notified of the piece of content either by subscribing to a Category or maintaining an asset publisher visible to the content manager to show the new content as it is published.
3. The secondary content manager can syndicate the content by applying new categories to a piece of content 
    1. The new categories drive which asset publishes on which pages will display the content and to whom
4. Categories can be permissioned differently for different roles
    1. Categories can be configured so that different users in different roles can:
        * View the categories
        * Apply the categories
            * Apply the categories to particular asset types (i.e. documents vs. web content)
5. Note that a content manager can create a copy of an article, at which point the normal content creation process applies.

### Content is secured so that only one or more groups or roles can see the content
1. When a piece of content is published, a content manager can also select which roles have the View permission to a piece of content
2. The view permission determines whether a piece of content can be seen at all, despite whether the user can see the page or context around where the piece of content is displayed
3. Even though an Asset Publisher portlet may be configured to display a piece of content, a user must first have access to the content in order to be able to see it
4. In the POC, content is permissioned by role, by permission
    * The interface may require additional changes to operate at the scale of tens of thousands of roles

