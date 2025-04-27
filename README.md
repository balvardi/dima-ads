---

# Dima Ads

![License](https://img.shields.io/badge/license-GPLv2-blue.svg) ![Version](https://img.shields.io/badge/version-1.5-green.svg)

A secure and user-friendly WordPress plugin that allows users to submit advertisements with categories, contact information, images, and descriptions. The plugin uses Bootstrap for styling and provides a seamless experience for both administrators and users.

## Features

- **User-Friendly Advertisement Submission**: Users can submit advertisements with a title, description, contact information, and an image URL.
- **Categories Support**: Administrators can create and manage categories for better organization of advertisements.
- **Admin Approval System**: All submitted advertisements are pending by default and require admin approval before being displayed publicly.
- **Public Display**: Approved advertisements can be displayed on any page or post using a shortcode (`[display_ads]`).
- **User-Specific Ad Lists**: Logged-in users can view their submitted advertisements in the WordPress dashboard.
- **Bootstrap Styling**: Forms and tables are styled using Bootstrap for a clean and modern look.
- **Security**: Includes nonce verification and input sanitization to prevent security vulnerabilities.

---

## Installation

### 1. Manual Installation
1. Download the plugin ZIP file from the [GitHub repository](https://github.com/your-repo/dima-ads).
2. Go to your WordPress admin dashboard.
3. Navigate to **Plugins > Add New**.
4. Click on **Upload Plugin** and upload the ZIP file.
5. Activate the plugin through the **Plugins** menu.

### 2. Via GitHub
1. Clone the repository into your WordPress plugins directory:
   ```bash
   git clone https://github.com/your-repo/dima-ads.git wp-content/plugins/dima-ads
   ```
2. Activate the plugin through the **Plugins** menu in WordPress.

---

## Usage

### 1. Admin Dashboard Pages
After activating the plugin, the following pages will be available in the WordPress admin dashboard:

- **Categories**: Manage advertisement categories (add/delete).
- **All Ads**: View and manage all submitted advertisements (approve/reject).
- **My Ads**: Logged-in users can view their submitted advertisements.
- **Submit Ad**: Logged-in users can submit new advertisements.

### 2. Displaying Advertisements on the Frontend
To display approved advertisements on your website:
1. Create a new page or edit an existing one.
2. Use the `[display_ads]` shortcode to list advertisements. For example:
   - Display all ads:
     ```plaintext
     [display_ads]
     ```
   - Display ads from a specific category:
     ```plaintext
     [display_ads category="cars"]
     ```
   - Limit the number of displayed ads:
     ```plaintext
     [display_ads limit="5"]
     ```

### 3. Customizing Styles
You can customize the appearance of advertisements by adding custom CSS to your theme's `style.css` file. Refer to the **Styling** section below for sample styles.

---

## Shortcode Parameters

The `[display_ads]` shortcode supports the following parameters:

| Parameter | Description                          | Example                      |
|-----------|--------------------------------------|------------------------------|
| `category`| Filter ads by a specific category   | `[display_ads category="cars"]` |
| `limit`   | Limit the number of displayed ads   | `[display_ads limit="5"]`    |

---

## Styling

To enhance the appearance of advertisements, you can use the following CSS styles. Add them to your theme's `style.css` file:

```css
.dima-ads-list {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    margin: 20px 0;
}

.dima-ad-item {
    border: 1px solid #ddd;
    padding: 15px;
    border-radius: 8px;
    width: calc(33.33% - 20px);
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.dima-ad-item:hover {
    transform: translateY(-5px);
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
}

.dima-ad-image {
    max-width: 100%;
    height: auto;
    border-radius: 8px;
    margin-bottom: 10px;
}

.dima-ad-title {
    font-size: 18px;
    margin: 10px 0;
    color: #333;
}

.dima-ad-description {
    font-size: 14px;
    color: #666;
    margin-bottom: 10px;
}

.dima-ad-contact {
    font-size: 14px;
    color: #0073aa;
}

.dima-ad-category {
    font-size: 12px;
    color: #999;
}
```

---

## Screenshots

1. **Admin Categories Page**:
   ![Categories Page](https://via.placeholder.com/800x400?text=Categories+Page)

2. **Submit Advertisement Form**:
   ![Submit Ad Form](https://via.placeholder.com/800x400?text=Submit+Ad+Form)

3. **Public Display of Advertisements**:
   ![Public Ads](https://via.placeholder.com/800x400?text=Public+Ads)

---

## Contributing

Contributions are welcome! If you'd like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a pull request.

---

## Support

If you encounter any issues or have questions, feel free to open an issue on the [GitHub repository](https://github.com/your-repo/dima-ads/issues).

---

## License

This plugin is released under the [GPLv2 license](https://www.gnu.org/licenses/gpl-2.0.html).

---

## Credits

- Developed by [R.Balvardi](https://github.com/balvardi)
- Inspired by the need for a simple and secure advertisement management system.

---

## Changelog

### Version 1.5
- Added public display of advertisements using `[display_ads]` shortcode.
- Improved styling with Bootstrap integration.
- Added support for filtering ads by category and limiting the number of displayed ads.

### Version 1.4
- Added fields for contact information and image URL in the submission form.
- Enhanced admin dashboard with all advertisements list and approval/rejection options.

### Version 1.3
- Initial release with basic functionality for submitting and managing advertisements.

---

Thank you for using **Dima Ads**! 😊
