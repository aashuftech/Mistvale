# Mistvale Tea Co.

Mistvale Tea Co. is a responsive tea e-commerce website designed to provide a smooth and premium shopping experience. Users can explore different teas, search and filter products, manage their cart and wishlist, check delivery availability, and browse recently viewed products.


## Features

- Responsive tea storefront for mobile, tablet, and desktop.
- Product search, category filtering, and sorting.
- Product Quick View modal with product details.
- Shopping cart with quantity and stock limits.
- Wishlist to save favourite products.
- Recently viewed products with remove functionality.
- Cart, wishlist, and recently viewed data saved in localStorage.
- Coupon code support with discount calculations.
- Shipping fee and free-shipping threshold calculations.
- Delivery pincode checker with serviceability and error states.
- Cart drawer with quantity controls and order summary.
- FAQ accordion with single-open behavior.
- Newsletter subscription interface.
- Tea-leaf entrance animation.
- Animated hero video.
- Custom favicon and brand visuals.
- Keyboard-accessible interactions and reduced-motion support.
- SEO metadata and JSON-LD structured data.

## How product browsing works

1. Users browse the available tea products.
2. They can search by product information.
3. Category filters help narrow down the products.
4. Sorting lets users organize products by available options.
5. Quick View displays additional product information without leaving the page.
6. Wishlist and Recently Viewed help users keep track of products.

## How the cart works

1. Users add available products to the cart.
2. They can increase or decrease quantities within the allowed limits.
3. The cart checks product stock and prevents invalid quantities.
4. Users can apply eligible coupon codes.
5. Shipping fees and discounts are calculated according to the configured business rules.
6. The cart state is saved in localStorage so it can persist after a page refresh.

The cart uses the product data as its source of truth for prices and stock.

## How wishlist and recently viewed work

- Users can save products to their wishlist using the heart button.
- Wishlist items remain saved after a page refresh.
- Opening a product in Quick View adds it to Recently Viewed.
- Recently Viewed keeps up to five unique products, with the latest viewed product first.
- Users can remove products from Recently Viewed.
- Both features use localStorage to persist their state.

## How delivery checking works

1. A user enters a delivery pincode.
2. The website validates the input.
3. The configured pincode-checking logic determines the serviceability result.
4. The interface displays the result or an error state.

Actual delivery coverage depends on the configured serviceability data or API.

## Built with

- **HTML5** — structures the website content.
- **CSS3** — handles responsive layouts, styling, and animations.
- **JavaScript** — implements product browsing, cart, wishlist, and other interactions.
- **LocalStorage** — persists cart and product preference data.
- **SVG** — provides lightweight icons and visual elements.
- **WebP** — used for optimized image assets where available.
- **Vercel** — hosts the live website.

## Project structure

```text
Mistvale/
├── index.html       Main website, styles and JavaScript
├── images/          Product, hero and brand images
├── favicon/         Favicon assets
├── video/           Hero background video
├── README.md        Project documentation
└── .gitignore       Git ignore rules
```

The exact files may differ depending on the current repository.

## Run locally

You will need a modern web browser and, optionally, a local development server.

### 1. Clone the repository

```bash
git clone YOUR_MISTVALE_GITHUB_REPO_URL
cd Mistvale
```

Replace the repository URL with your actual GitHub URL.

### 2. Open the website

You can open `index.html` in your browser or use a local development server.

For example, if you have VS Code with the Live Server extension installed, right-click `index.html` and select **Open with Live Server**.

### 3. Check the assets

Make sure the `images/`, `favicon/`, and `video/` folders are present and that their filenames match the paths referenced in `index.html`.

## Deployment

The website is deployed on Vercel.

- **Live URL:** https://mistvaletea.vercel.app
- **Hosting:** Vercel
- **Build step:** Not required for the current plain HTML, CSS, and JavaScript setup.

The deployed version should be checked after updates to confirm that images, the hero video, favicon, and interactive features work correctly.

## Accessibility and performance

- Responsive layouts for different screen sizes.
- Keyboard-accessible controls and modal interactions.
- ARIA attributes for relevant interactive components.
- Reduced-motion support for users who prefer less animation.
- Lazy loading for appropriate below-the-fold images.
- Image dimensions to help reduce layout shifts.
- Lightweight inline SVG icons and CSS animations.
- SEO metadata and structured data for relevant content.

## Known limitations

- The project is a frontend storefront, not a complete production e-commerce backend.
- Cart, wishlist, and recently viewed data are stored in the browser using localStorage.
- Cart and coupon calculations run on the client and would need server-side validation in a real payment workflow.
- The pincode checker depends on the configured serviceability logic or API.
- The newsletter interface requires a backend or email service to store subscriptions and send emails.
- A production checkout would need secure payment integration, server-side order validation, and persistent order management.
- Product pack sizes and other commercial details should be verified before accepting real customer orders.

## Future improvements

- Connect products and stock to a backend database.
- Add secure user accounts and order history.
- Integrate a payment gateway and server-side order validation.
- Connect delivery checks to a real serviceability API.
- Connect the newsletter to an email service.
- Add automated tests and performance monitoring.
