Issue after updating Elementor and/or Elementor Pro
After updating Elementor, the updated version may conflict with your current setup. Depending on what changes are not appearing, try the below troubleshooting steps.

Issue	Solution
Files or Data Files issues	1. Go to WP Admin > Elementor > Tools.
2. Click Regenerate Files & Data.
Cache and optimization issues	1. Clear optimizations and cache third-party plugins before updating. Ensure that they are disabled when you update.
2. Ensure that you do not have server caching enabled. You may need to consult your current hosting provider for additional assistance.
Issue with Elementor features	1. Deactivate Elementor features to eliminate issues with experimental features, mainly performance features such as Inline Font Icons and Improved CSS Loading.
2. Deactivate features by going to WP Admin > Elementor > Settings > Features.
3rd party plugin conflicts	Disable all plugins except Elementor and Elementor Pro on your staging site to eliminate any possible conflicts with third-party plugins.
WordPress Themes conflict	Switch your theme to any default WordPress theme or the Elementor Hello theme.
Issues with CSS Print method	1. Deactivate and clear optimizations and cache before updating. Ensure that they are disabled when you update.
2. Ensure that you do not have server caching enabled. You may need to consult your current hosting provider for additional assistance.
Cache and Optimization issues
Cache or optimizations can prevent your changes from appearing online.
Do one or more of the following to troubleshoot the issue:

Disable any third-party WordPress optimization or cache plugins.
Temporarily clear/disable any server-level caching. You may need to consult your hosting provider for help with this.
Clear your browser cache or test the page using incognito mode.
Issues with Features or Experiments
An issue with a feature or experiment can prevent your changes from appearing online.

Do one or more of the following to troubleshoot the issue:

Deactivate Elementor features to eliminate issues with experimental features, mainly performance features such as Inline Font Icons and Improved CSS Loading. You can deactivate features by going to WP Admin > Elementor > Settings > Features. See this article for more information: Elementor features.
Disable any third-party WordPress optimization or cache plugins.
Temporarily clear/disable any server-level caching. If you need help with this, consult your hosting provider.
Clear your browser cache or test the page using incognito mode.
Incorrect Server/WordPress configuration
Server or WordPress configurations may affect how stylesheets are generated, preventing your changes from appearing online.

Do one or more of the following to troubleshoot the issue:

If you recently added SSL or made other changes in your domain or file directory, ensure these changes are aligned. Go to Settings > General on the WordPress dashboard and check that both the WordPress Address (URL) and Site Address (URL) are the same and that both are either http:// or https://.
Permalinks can affect your layout or stylesheet. Go to WP Admin>Settings>Permalinks and set permalinks to Plain. 
Check your Custom Server Configuration/Optimization.
Check your .htaccess custom code/configuration.
Issues with CSS Print method
The CSS print method can affect your stylesheet.

To troubleshoot the issue:

In the WP Admin, go to Elementor>Settings>Performance and check the CSS Print Method.
If it is set to External File, set it to Internal File. If it is set to Internal File, set to External File.
Test to see if this resolves the issue.
Unclosed HTML tags, CSS or custom codes
If you added custom code or CSS to Elementor widgets, Global Settings or Theme and did not close the HTML tags, this can prevent your changes from appearing online.

To troubleshoot the issue:

Check any custom code or CSS added on to global settings and verify that the code works, checking for any unclosed, or improperly closed, tags.
If you added any inline styling to widgets (such as the Heading, Text Editor or HTML widgets), check them for unclosed, or improperly closed tags.
Check your pages for custom CSS. An easy way to check is to open the Navigator and look for any highlighted elements. These highlights indicate that the element contains custom CSS, motion effects or absolute positioning.
