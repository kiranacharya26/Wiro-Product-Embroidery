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
