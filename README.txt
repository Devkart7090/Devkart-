DevKart Launch Candidate v2
===========================

This package is the cleaned-up static/demo release of the DevKart store and admin panel.

STORE
- Responsive mobile + desktop layout.
- Product search and category filtering.
- Product detail page with 4-image gallery.
- Login/signup demo, profile, addresses, wishlist and orders.
- Cash on Delivery checkout.
- PIN-code lookup using India Post API when available.
- Stock limits are enforced in cart and Buy Now.
- Stock is reduced when a COD order is placed.
- Order records store product name/price snapshots so deleting a product does not erase order item names.
- Empty/out-of-stock states are handled.
- Added WhatsApp support shortcut using the configured DevKart support number.
- Removed placeholder/fake review-count and rating claims; reviews should be added only from real customer feedback.
- Basic SEO description, theme color, robots metadata and lazy-loaded product images.

ADMIN CONTROL PANEL
- Open admin.html on the same domain/browser as index.html.
- Demo login: admin / admin123.
- Add/edit/delete products, price, MRP, stock, image and description.
- Manage order status: Confirmed, Packed, Shipped, Out for Delivery, Delivered, Cancelled.
- Customer list.
- Dashboard sales excludes cancelled orders.
- Export orders to CSV.
- Backup browser data to JSON.
- Product changes sync between store/admin tabs in the same browser using localStorage/storage events.

IMPORTANT PRODUCTION LIMITATION
- This is still a static GitHub Pages demo. Data is stored in browser localStorage.
- The admin username/password is NOT secure and must not be used as a production authentication system.
- A real launch needs an online backend/database (for example Supabase/Firebase), secure admin authentication, server-side order creation, inventory locking, backups, and server-side customer data storage.
- Payment gateway, real SMS OTP, shipping/courier integration and automated transactional notifications are not included.

GITHUB PAGES
Upload all files from this folder to the repository root. Keep index.html, admin.html, images and _redirects in the root.

Recommended next production modules:
1. Supabase/Firebase database
2. Secure admin login + roles
3. Server-side products, customers, orders and stock
4. Razorpay/Cashfree/other payment gateway if online payments are needed
5. WhatsApp/SMS/email order notifications
6. Shipping/courier integration and tracking
7. GST invoice generation and downloadable invoices
8. Privacy Policy, Terms, Refund/Cancellation and Shipping Policy pages
9. Analytics, backups and error monitoring
10. Custom domain + HTTPS (GitHub Pages already provides HTTPS for the standard Pages domain)
