# Theme Configuration
The following sections describe how to add other types of content, including portlets and pages, as well as how to provision that content based on service packages or perform other, more advanced configuration.

## Configurable Theme Elements
The Covisint Standard Theme has the following key attributes:
```
Key portlets optimized for the generic theme (mobile and big browser) Responsive and Adaptive behaviors
* Responsive design
* Adaptive navigation
* Gesture support for key portlets
* Includes Twitter Bootstrap and 7 page layouts optimized for bootstrap
```
```
Media queries in the bootstrap CSS are (first number indicates the min width for activation second number is the max width for activation):
* 767 min / 768 max (768)
* 991 min / 992 max (992)
* 1199 min / 1200 max (1200)
```
```
Optimized navigation
* Direct drag and drop page navigation and page name modification disabled to avoid inadvertent site map changes
* Clickable top navigation optimized for big browser and mobile
```
## Configurable page elements accessible from Manage Pages menu Configurable style
    * Configurable style sheet override
    * Configurable footer
    * Dynamic style inheritance based on Organization hierarchy             
The following settings can be configured:
* **Show Portlet Borders by Default (Default value: false)** – This setting controls whether portlets are enabled or disabled when portlets are dropped on a page.  Note that this setting only controls the default for portlets when they are initially dropped on a page and does not toggle borders off or on when enabled or disabled. Show Site Name (Default value: true) – This setting controls whether the site name is displayed in the top right section of the Masthead
 
* **Hide-asset-publisher-icons (Default value: true)** – This setting controls whether the default Liferay icons are displayed in the standard Asset Publisher Display Styles (Table, Title List, Abstract, Full Content)
* **Hide-goto-menu (Default value: false)** – This setting controls whether the Go To menu is displayed in the Dock Bar.  The Go To menu can be suppressed where users have content management rights on only one site or access to Control Panel needs to be restricted
* **Enable-theme-inheritance (Default value: false)** – This setting controls whether theme inheritance is enabled.  Theme inheritance controls whether a CSS override and custom footer content will be applied to a page or site based on a users Organization membership.  The Footer content is HTML that is embedded in the Footer of the theme.  The CSS Override has settings that will override content styling in the footer.  The business rules are provided in a separate section below.
* **Max-page-width (Default value: 1200)** – This setting controls the maximum page width of the content and navigation.  The maximum value is 1200 px.  Note that this setting can be used in conjunction with mobile device rules.  The max width for mobile-only parallel pages can be set within the standard break points for the responsive design.
* **Support IE8 Responsiveness (Default value: false)** – This setting controls whether the page will load an additional CSS file to support responsive behavior in IE8.  If IE8 is not a required browser, this setting can be used to prevent the additional CSS from being loaded, improving page performance.
* **IE8 Stylesheet (Default value: /documents/null/ie8.css)** – This setting controls the URL to the CSS file for IE8 responsive behavior.
* **Include Search (Default value: true)** – This setting controls whether the search box is displayed on a page or not.  The search box appears on the top right of the Top Hat section of the page.

## Theme Override
The following elements can be configured in the theme CSS Override.  The CSS Override is based on a structure and template.  The default values in the structure can be set using the standard functionality.  The Theme is designed to look for content based on a structure named STYLESHEET_OVERRIDE and for the Footer based on a structure named FOOTER_CONTENT.  The list of items that can be configured are outlined below and the values entered are HTML code for the various elements (Hexadecimal values for colors, em size for font sizes, and image paths for images):
* **Base Styles**
    * Background Color
    * Base Font Size
    * Dockbar Styles
    * Dockbar Background Color
    * Dockbar Link Color
    * Dockbar Link (Hover) Color
* **Top Hat Rules**
    * Top Hat Sidewall Color
    * Top Hat Background Color
    * Masthead Styles
    * Brand Logo
    * Masthead Background Image
    * Masthead Background Color
    * Masthead Sidewall Color
    * Masthead Site Name Font Size
    * Masthead Site Name Font Color
* **Navigation Styles**
    * Navigation Background Color
    * Navigation Sidewall Color
    * Navigation Link Text Color
    * Navigation Link Text (Hover) Color
    * Navigation Active Link Background Color
* **Content Area Styles**
    * Content Area Sidewall Color
    * Content Area Background Color
* **Footer Styles**
    * Footer Background Color
    * Footer Sidewall Color
    * Footer Text Color
    * Footer Link Color
    * Footer Link (Hover) Color
* **Typography Styles**
    * Content H1 Font Size
    * Content H1 Font Color
    * Content H1 Font Weight
    * Content H2 Font Size
    * Content H2 Font Color
    * Content H2 Font Weight
    * Content H3 Font Size
    * Content H3 Font Color
    * Content H3 Font Weight
    * Content H4 Font Size
    * Content H4 Font Color
    * Content H4 Font Weight

## Business Rules for Theme Override
The following business rules describe how Theme Inheritance works when enabled and disabled:
1. Base theme is the Covisint branded theme on a specific site (“Site A”)
    * Assumptions:
        1. Site A is not part of the Org Site hierarchy where the users belong
        2. A user can only belong directly to one Organization at a time
            * A users’ organization may be a member of one or more other organizations
                * This could be used to drive access to more than one or all sites in a hierarchy
                * This could be used to create a matrixed organization
            * A user will be a named, individual member of only one Organization
    * If the check box for” Enable Theme Inheritance” is checked:
        1. If there is no override web content article anywhere in the portal, theme appears as default for all users on Site A.
        2. If there is an override web content article in the web content repository for Site A and nowhere else in the portal, Site A will have the style overrides of that web content article.
iii.	If there is an override web content article in the Org Site where the user is a named, individual member of the Organization, (“Site B”) then the style overrides of the web content article in Site B will be applied to Site A when the user visits site A.
iv.	If there is not an override web content article in the Org Site where the user is a named, individual member of the Organization, (“Site B”) but there is an override web content in the hierarchy of Orgs where the user is a named individual member (“Site C”)then the style overrides of the web content article in Site C will be applied to Site A when the user visits site A.
c.	If the check box for “Enable Theme Inheritance” is NOT checked:
i.	If there is no override web content article anywhere in the portal, theme appears as default for all users on Site A.
ii.	If there is an override web content article in the web content repository for Site A and nowhere else in the portal, Site A will have the style overrides of that web content article.
iii.	If there is an override web content article in the Org Site where the user is a named, individual member of the Organization, (“Site B”) then the style overrides of the web content article in Site B will NOT be applied to Site A when the user visits site A.
iv.	If there is not an override web content article in the Org Site where the user is a named, individual member of the Organization, (“Site B”) but there is an override web content in the hierarchy of Orgs where the user is a named individual member (“Site C”)then the style overrides of the web content article in Site C will NOT be applied to Site A when the user visits site A.
d.	The check box for “Enable Theme Inheritance” is NOT checked by default.

