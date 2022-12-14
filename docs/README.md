# Store Theme Shopstar

shopstar-vtexio is a clone of the shopstar store made with Vtex IO.

[https://shopstar.pe](https://shopstar.pe) was the shop chosen to realize the clone of this project, bearing in mind a design responsive that is to say the different dimensions of the screens, so much in mobile as in desktop.

## Image Gallery 

### Desktop Version

**Home Page**

![Preview](../assets/img/readme-image__home-desktop.png)

**Seccion Footer**

![Preview](../assets/img/readme-image__footer-desktop.png)

**Search Result Page**

![Preview](../assets/img/readme-image__search-results.png)

**Detail Product Page**

![Preview](../assets/img/readme-image__product-detail-desktop.png)
![Preview](../assets/img/readme-image__product-review-desktop.png)

**Custom Page About Us**

![Preview](../assets/img/readme-image__custom-page-about-us.png)

**Custom Page Terms and Conditions**

![Preview](../assets/img/readme-image__custom-page-terms-conditions.png)

**Custom Page Returns and Exchanges**

![Preview](../assets/img/readme-image__custom-page-returns-exchangess.png)
### Versión Mobile

**Home Page**

![Preview](../assets/img/readme-image__home-mobile.png)

**Seccion Footer**

![Preview](../assets/img/readme-image__footer-mobile.png)

**Detail Product Page**

![Preview](../assets/img/readme-image__product-detail-mobile.png)

### Custom Components

**Custom Countdown**

![Preview](../assets/img/readme-image__custom-component-countdown.png)

**Categories Diagramation**

![Preview](../assets/img/readme-image__custom-categories-diagramation.png)

**Custom Login**

![Preview](../assets/img/readme-image__custom-component-login.png)
![Preview](../assets/img/readme-image__custom-component-login-modal.png)

## Configuration

### Step 1 - Basic Configuration

Go to the VTEX IO [basic configuration guide](https://vtex.io/docs/getting-started/build-stores-with-store-framework/1) and follow the steps below.

At the end of the setup, you should have the VTEX command line interface (Toolbelt) installed along with a developer workspace in which you can work.

### Step 2 - Cloning the repository

Perform the [clone](https://github.com/cristhian-fernandez/shopstar-vtexio) of this repository in your local files in order to start working on it effectively. 

Then, access the repository directory using your terminal.

### Step 3 - Edit the Manifest.json

Enter the `manifest.json`n file and replace the values of `vendor`(name of the account you are working on) and `name`(name you want for your theme). For example: 

```json
{
   "vendor": "itgloberspartnercl",
   "name": "shopstar-vtexio"
}
```
### Step 4 - Install necessary apps

To use the Store Framework and work on your given store theme, it is necessary to have `vtex.store-sitemap` and `vtex.store` installed.

You can run the `vtex list` command and check if those applications are already installed, otherwise, if they are not, run the command: `vtex install vtex.store-sitemap vtex.store -f` to install them respectively.

### Step 5 - Uninstall the default store-theme

By running `vtex list`, you can check if any themes are installed.

It is common to have a `vtex.store-theme` already installed when you start the front-end development process of the store.

Therefore, if you find it in the application list, copy its name and use it together with the `vtex uninstall` command. For example:

```json
vtex uninstall vtex.store-theme
```

### Step 6 - Check the required dependencies and builders

Once this section of the `manifest.json` has been modified, you must check that the repository contains the following dependencies and the necessary builders:

### Builders 

```
{
    "styles": "2.x",
    "store": "0.x",
    "docs": "0.x",
    "assets": "0.x"
}
```

###  Dependencies

```
{
    "vtex.store": "2.x",
    "vtex.store-header": "2.x",
    "vtex.product-summary": "2.x",
    "vtex.store-footer": "2.x",
    "vtex.store-components": "3.x",
    "vtex.styleguide": "9.x",
    "vtex.slider": "0.x",
    "vtex.carousel": "2.x",
    "vtex.shelf": "1.x",
    "vtex.menu": "2.x",
    "vtex.minicart": "2.x",
    "vtex.product-details": "1.x",
    "vtex.product-kit": "1.x",
    "vtex.search-result": "3.x",
    "vtex.login": "2.x",
    "vtex.my-account": "1.x",
    "vtex.flex-layout": "0.x",
    "vtex.rich-text": "0.x",
    "vtex.store-drawer": "0.x",
    "vtex.locale-switcher": "0.x",
    "vtex.product-quantity": "1.x",
    "vtex.product-identifier": "0.x",
    "vtex.product-specification-badges": "0.x",
    "vtex.product-review-interfaces": "1.x",
    "vtex.telemarketing": "2.x",
    "vtex.order-placed": "2.x",
    "vtex.stack-layout": "0.x",
    "vtex.tab-layout": "0.x",
    "vtex.responsive-layout": "0.x",
    "vtex.slider-layout": "0.x",
    "vtex.iframe": "0.x",
    "vtex.breadcrumb": "1.x",
    "vtex.sticky-layout": "0.x",
    "vtex.add-to-cart-button": "0.x",
    "vtex.store-link": "0.x",
    "vtex.store-icons": "0.x",
    "vtex.store-image": "0.x",
    "vtex.modal-layout": "0.x",
    "vtex.overlay-layout": "0.x",
    "vtex.search": "2.x",
    "vtex.product-list": "0.x",
    "vtex.checkout-summary": "0.x",
    "vtex.disclosure-layout": "1.x",
    "vtex.product-price": "1.x",
    "vtex.category-menu": "2.x",
    "vtex.product-availability": "0.x",
    "vtex.shop-review-interfaces": "0.x"
}
```
### PeerDependencies

```
{
  "vtex.mega-menu": "2.x"
}
```

### Custom Apps

```
{
    "itgloberspartnercl.countdown": "0.x",
    "itgloberspartnercl.custom-login": "0.x",
    "itgloberspartnercl.categories-diagramation": "0.x"
}
```

### Step 7 - Run a store preview

After performing the above steps, it is time to upload the changes you made to your local files by running the `vtex link` command. 

If the process is successful you should see the following message in your terminal: `App linked successfully`. Next, run the `vtex browse` command to open a browser window with your linked store.

This will allow you to see the changes applied in real time, through your account and workspace.

## Contributors
1. Cristhian Javier Fernández Cumbia