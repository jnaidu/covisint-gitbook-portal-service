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

## Theme