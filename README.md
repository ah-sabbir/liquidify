# liquidify - One handed shopify business solutions

This is a flexible Shopify theme that's meant to be reused and customized. Reusable components exist within sections, snippets, and templates for assurance that all features are available across the entire theme.

## Features

- **Responsive Design**: The theme is responsive and adapts itself to various screen sizes.
- **Dynamic Product Grid**: Highlights the products on the homepage dynamically.
- **Reusable Snippets**: Pockets of code, such as the price of the product, have been reused in numerous templates.
- **Easy Navigation**: Automatically generated navigation menus based on Shopify's link lists.
- **Customizable Sections**: This can easily be done using the Shopify theme editor.

## Folder Structure

```bash
my-universal-theme/  
├── assets/  
│   └── theme.css               # Main stylesheet for the theme  
├── config/  
│   ├── settings_schema.json     # Schema for theme setting  
│   └── settings_data.json       # Default configuration for the theme  
├── layout/  
│   └── theme.liquid             # The main layout file for the theme  
├── sections/  
│   ├── header.liquid            # Header section  
│   ├── footer.liquid            # Footer section  
│   └── product-grid.liquid      # Product grid section on homepage  
└── snippets/  
    ├── product-price.liquid     # Snippet to show product price  
    └── navigation.liquid        # Dynamic navigation menu snippet  
├── templates/  
│   ├── index.liquid             # Homepage template  
│   ├── product.liquid           # Product detail page template  
│   ├── collection.liquid        # Collection page template  
│   └── page.liquid              # Template of a custom page  
└── config/  
    └── settings_data.json       # Data of settings used for theme customizing  
```

# Installation

Install the theme in your Shopify store with the following steps:

1. **Clone or download** this repository to your computer.
2. **Compress the Folder**: Make sure all theme files and folders are compressed inside one single `.zip` file (e.g., `my-universal-theme.zip`).
3. **Upload the theme to Shopify**:
   - Log in to your Shopify admin.
   - Go to **Online Store > Themes**.
   - Click **Upload Theme**, then select the `.zip` file you just created.
4. **Publish Theme**: Upon uploading, you can preview the theme and publish it as your live theme.

# Customization

- **Edit Theme Settings**: You can adjust several settings from the Shopify theme editor (e.g., title for the product grid). These settings are defined in `config/settings_schema.json` and stored in `config/settings_data.json`.
- **Adjust Styles**: The CSS for the theme resides in `assets/theme.css`. You can override the store's styling by editing this file.
- **Add/Edit Sections**: Sections such as header, footer, and product-grid can be updated from the `sections/` folder. You can create additional sections by following the same structure.
- **Navigate**: The main navigation is dynamically pulled using the `snippets/navigation.liquid` file, which gets data from your Shopify link lists. To edit the navigation, go to **Online Store > Navigation** in your Shopify admin and click **Edit** by the Main Menu.

# Available Templates

- **index.liquid**: Homepage template containing a dynamic product grid.
- **product.liquid**: Product detail page template.
- **collection.liquid**: Collection page template.
- **page.liquid**: Template for custom pages such as "About Us" or "Contact Us."

# Adding New Sections and Snippets

- **Sections**: To create a new section, add a `.liquid` file inside the `sections/` folder and reference it in your template or the theme editor.
- **Snippets**: Provide reusable components by creating `.liquid` files in the `snippets/` directory. Reference snippets using `{% render 'snippet-name' %}` from your templates.

# How to Use Product Grid

Add the Product Grid section from the theme editor to the homepage. You can change the section title and adjust the number of products displayed by editing `sections/product-grid.liquid`.

# Support

If you have any problems or need assistance, you can contact the theme developer [Sabbir Ahmmed](mailto:<imsabbir.dev@outlook.com>?subject=<subject>&body=<body>) or refer to the [Shopify Theme Development Documentation](https://shopify.dev/themes).
