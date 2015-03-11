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

