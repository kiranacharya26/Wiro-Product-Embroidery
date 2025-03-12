Files used -: 
cart-drawer.liquid
main-product.liquid


Documentation :

Tech stack:
Front-End
JavaScript
Liquid
AJAX
HTML5
Tailwind CSS
Shopify platform
Shopify cart API
Backend
Shopify metafields
Shopify admin API

Managing metafields: Useful for offering product customisation features ex: embroidery

Product metafields:
Metafields are stored under product and used in liquid templates using ex:product.metafields.custom, where we can add properties like fonts, colors and pricing.
We can fetch them product.metafields.custom.embroidery_image.
Display and update metafields
embroidery :- these metafields are displayed dynamically based on availability. Ex font color selection options are shown dynamically.
Adding to cart: when a product is added to cart, the selected options values are sent as properties in form. These data will be stored in a cart.
Customise metafields 
Using shopify we can create metafields in the shopify admin panel.
 Clients can add multiple custom properties.

Cart drawer: 

Cart drawer: a sliding panel which contains items added to cart
Cart drawer can be opened and closed using js by toggling
This cart drawer dynamically shows items added to cart including price and also we can from here navigate to the checkout page.
Provide overlay when the cart drawer is open, so the attention will be on the cart and not the background.
Cart data
/cart.js fetches the cart data, which includes items, properties, price etc.
The cart total will be updated dynamically and when embroidery  options are added, that price will also be added to total.
Using JS for cart drawer
Cart drawer slides from right to left and an overlay is shown.
addtoCart function responsible for submitting products to cart and also checks for existing products to prevent duplication.
Cart options
Checkout button redirects to checkout page
Using a clear cart clears all the products in the cart at once, not needed but useful.

PDP: 

Metafields integration: handles customisation for product, provides custom feature for users.
Embroidery Enabled-used to provide options  which are available for the product.
Embroidery Image-stores image which can be displayed with the options
Character Limit-specifies max number of characters that can be added for embroidery.
Embroidery Fonts & Colors-provide options for font and color selection.
Form elements for options: 
Embroidery Text Input-customer can add text for embroidery and character limit will be set using metafield.
Font select-list of fonts which will be rendered using metafield id.
Color select-list of colors for embroidery text
Price-prices for specific color options will be different and using metafield we can achieve this.
Main image and thumbnail
The PDP provides a carousel of product images. The main image switches when a thumbnail is clicked or when the "previous" or "next" buttons are used. Using JS we can achieve this functionality.
Handling product submission
form-submits the product ID along with any customized properties (like embroidery text, color, and font) to the cart.
Price adjust- script adjusts the price dynamically to include any additional embroidery charges and adds them to form data.
Additional:
Use AJAX- 
Using AJAX to interact with cart allows users to add, update and remove items from cart without reloading the page.







	




