Dima Ads 

   
   

    

Dima Ads  is a secure and user-friendly WordPress plugin designed to allow users to submit advertisements for admin approval. It provides a simple interface for users to submit their ads and an admin dashboard to manage and approve/reject submissions. 

Developed by Rouhollah Balvardi  under the Dima  brand, this plugin ensures security, flexibility, and ease of use. 
Features 

    User-Friendly Submission Form : Users can easily submit advertisements via a shortcode.
    Admin Approval System : Admins can approve or reject submitted ads from the WordPress dashboard.
    Ad Limit Per User : Each user can submit a limited number of ads (default is 3).
    Security Measures : Includes CSRF protection, SQL injection prevention, and XSS protection.
    Bootstrap Styling : Clean and responsive UI using Bootstrap.
    Translation Ready : Supports localization with proper text domains.
     

Installation 
Manual Installation 

    Download the latest release of Dima Ads from the GitHub repository .
    Upload the dima-ads folder to the /wp-content/plugins/ directory of your WordPress installation.
    Activate the plugin through the 'Plugins' menu in WordPress.
    Use the [submit_advertisement] shortcode in any post or page to display the ad submission form.
     

Usage 
Submitting Ads 

    Users can submit ads by visiting a page or post where the [submit_advertisement] shortcode is used.
    Each user can submit up to 3 ads  by default.
     

Managing Ads 

    Admins can manage ads from the Dima Ads  menu in the WordPress dashboard.
    Ads can be approved or rejected from the admin panel.
     

Screenshots 

    Ad Submission Form 

   

Admin Dashboard 

       
     

Security 

This plugin implements several security measures to ensure safe usage: 

    CSRF Protection : Uses WordPress nonces to prevent cross-site request forgery attacks.
    SQL Injection Prevention : Uses $wpdb->prepare for all database queries.
    XSS Protection : Sanitizes all user inputs and escapes outputs.
     

Contributing 

Contributions are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request. 

    Fork the repository.
    Create your feature branch (git checkout -b feature/YourFeatureName).
    Commit your changes (git commit -m 'Add some feature').
    Push to the branch (git push origin feature/YourFeatureName).
    Open a pull request.
     

Support 

For support or inquiries, please contact us: 

    Developer : Rouhollah Balvardi
    Email : your-email@example.com 
    Website : dimagroup.ir 
     

License 

This plugin is released under the GNU General Public License v2 (or later) . 
Credits 

    Author : Rouhollah Balvardi 
    Brand : Dima Group 
    Inspiration : Built with love for WordPress developers and users.
     

Changelog 
Version 1.0 

    Initial release.
    Added ad submission form with user limits.
    Added admin dashboard for managing ads.
    Implemented security measures (CSRF, XSS, SQL Injection).
     
