# Targeting Content
This section describes the different ways to introduce a piece of web content into an environment, based on the business rules and the model that is configured in the POC. There are several ways to deliver content:
1. Publish content on a single page that is displayed to all users
2. Publish content on a page that is displayed to users of just one customer
3. Publish content on a page that is displayed to users based on context
4. Publish content on a page based on personalization or preference
5. Publish content that can appear on one page, then downstream content managers can choose to display the content in a site or modify the content before it is displayed
6. Content is secured so that only one or more groups or roles can see the content

## Publish content on a single page that is displayed to all users
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

## Publish content on a page that is displayed to users of just one customer
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

## Publish content on a page that is displayed to users based on context
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
d.	Categories are applied to the Web Content Article
e.	Asset Publisher is configured to display Web Content Articles:
i.	Scope includes site or repository where the Web Content is located
ii.	Categories are configured on the Asset Publisher to include the Web Content Article in the display criteria 
iii.	The article is displayed in an Asset publisher portlet on any site as long as it is scoped and configured to display content from the site where the content is stored and based on categorization


## Publish content on a page based on personalization or preference

## Publish content that can appear on one page, then downstream content managers can choose to display the content in a site or modify the content before it is displayed

## Content is secured so that only one or more groups or roles can see the content
