# Dav-Gevra-2026
Creating a website and an app

PROJECT: E-ANAND MELA

DAV Public School – SECL Gevra

Complete Website + Mobile Application Development

Act as a senior full-stack developer, UI/UX designer, database architect and application security engineer.

Build a complete, production-oriented, responsive web application and installable mobile-friendly PWA named:

E-ANAND MELA – DAV Public School SECL GEVRA

A. DESIGN AND BRANDING

Create an exceptionally attractive, colourful, premium Indian school carnival experience.

Opening screen:

- Large attractive festive Anand Mela hero image.
- Main Hindi title: आनंद मेला
- Punchline: "अपनों का आंगन, घर जैसा स्वाद… आनंद मेले में हर पल खास!"
- Subtitle: "आइए, अपनेपन का स्वाद चखिए और यादों का मेला सजाइए!"
- School branding: DAV Public School – SECL Gevra.
- Prominent buttons: Explore Stalls, Order Food, E-Coupons, Games, Donate Clothes.

Design requirements:

- Premium Zomato/Swiggy-inspired visual quality, but original branding.
- Rich festive colours, orange, yellow, red, purple and teal.
- Beautiful Hindi and English typography.
- Responsive cards, gradients, illustrations, icons and smooth animations.
- Mobile-first design.
- Beautiful loading screens, empty states, notifications and confirmation dialogs.
- Do not use generic unstyled admin templates.

B. EVENT CONFIGURATION

Create 15 configurable stalls.

Stalls 1–12: Food stalls, initially supporting two food items each.

Stalls 13–15: Game Zone / Fun Corner.

Each stall:

- 3 assigned teachers.
- 4 assigned students.
- Minimum sales target: ₹5,000.
- Configurable members, inventory, pricing and expenses.
- Individual stall ledger.

Allow Admin to add, edit, delete, activate or deactivate food items and game activities.

Allow Admin to add, remove or reassign teachers and students to any stall.

C. ROLE-BASED LOGIN AND ACCESS

Create secure login and dashboards for:

1. Super Admin
2. Stall Teacher
3. Student
4. Customer
5. Cashier / Coupon Verifier
6. Delivery Partner
7. Donation Coordinator

Implement role-based access control on the backend, not just by hiding frontend buttons.

Every user should only access authorized information.

Admin must be able to create and disable accounts and reset credentials.

D. ADMIN DASHBOARD

Create a professional master dashboard displaying:

- Total stalls: 15
- Total registered teachers and students
- Total investments
- Total sales
- Total expenses
- Total gross profit
- Total net profit
- Stall-wise performance
- Target completion percentage
- Total coupons generated
- Coupons redeemed
- UPI transactions
- Cash transactions
- Remaining stock
- Pending orders
- Delivery status
- Donations collected and distributed.

Provide interactive charts, date filters, stall filters and downloadable Excel/PDF reports.

E. INVENTORY AND BUSINESS ACCOUNTING

Implement individual inventory and financial ledgers for all stalls.

Maintain:

- Opening stock
- Stock purchases
- Stock received
- Stock sold
- Damaged stock
- Remaining stock
- Item-wise selling price
- Item-wise cost price
- Purchase expenses
- Other expenses
- Total revenue
- Gross profit
- Net distributable profit.

Track investment separately for every teacher and student.

Profit-sharing formula:

Member profit share = (Member's eligible investment / Total eligible investment) × Distributable net profit.

Do not automatically distribute profit before all expenses, liabilities and adjustments have been entered.

Maintain complete transaction history and audit logs.

Prevent unauthorized editing or deletion of completed financial transactions. Use reversal and adjustment entries instead.

F. E-COUPON AND UNIQUE QR TOKEN ENGINE

Create ₹20 denomination digital coupons.

Requirements:

- Generate cryptographically secure unique coupon identifiers.
- Generate individual QR codes.
- Each coupon can be redeemed exactly once.
- Implement atomic server-side redemption.
- Prevent replay, duplicate redemption and concurrent double-spending.
- Record coupon issue, purchase, verification, redemption and cancellation.
- Show duplicate scan warning.
- Generate printable and digital receipts.
- Allow bulk coupon generation.
- Provide Admin reporting and reconciliation.

Coupon verification must happen through an authenticated server API. Never trust QR contents alone.

G. CUSTOMER ORDERING SYSTEM

Create attractive food menus with:

- Stall name
- Food image
- Item name
- Description
- Price
- Availability
- Add to cart
- Quantity selection
- Order summary
- Receipt generation.

Allow customers to pay using:

1. UPI payment gateway.
2. Cash payment with authorized confirmation.

Implement proper order IDs and payment reconciliation.

H. STALL MANAGEMENT PANELS

Teacher panel:

- Stall overview
- Sales dashboard
- Inventory
- Purchase entries
- Expenses
- Investment ledger
- Team members
- Customer orders
- Coupon verification
- Financial reports.

Student panel:

- Own inventory
- Personal stock contribution
- Item-wise sales
- Remaining stock
- Investment
- Calculated profit share
- Transaction history.

I. ANAND MELA FOOD EXPRESS

Create a separate public-facing food delivery module.

Functions:

- List approved unsold food items.
- Update available quantities.
- Customer location/address.
- Delivery fee fixed at ₹30.
- UPI and Cash on Delivery.
- Order acceptance.
- Food preparation status.
- Delivery partner assignment.
- GPS-based location tracking with consent.
- Estimated preparation and delivery times.
- Order completion and delivery confirmation.

Only authorized staff can list unsold food.

Implement stock reservation to prevent two customers from ordering the same remaining item.

Do not expose customer addresses or delivery partner location publicly.

J. PROMOTION AND ADVERTISEMENT

Build promotional tools before the event:

- Public event landing page.
- Shareable menu links.
- WhatsApp sharing.
- Downloadable promotional posters.
- QR code for website access.
- Stall introductions.
- Event countdown.
- Food previews.
- Delivery service announcement.
- School-approved promotional content.

K. ANAND VASTRA SEVA – DONATION MODULE

Create a separate social donation management system.

Allow parents and students to register donations of clean, washed and usable clothes.

Capture:

- Donor details or anonymous donation.
- Clothing category.
- Quantity.
- Collection status.
- Quality inspection.
- Packaging status.
- Receiving acknowledgement.
- Recipient institution.
- Distribution date.
- Distribution proof.
- Total collection and distribution reports.

Include categories for old-age homes, orphanages, blind schools, schools for deaf and speech-impaired children, poor families, women's shelters, homeless people, tribal communities, special schools and other eligible institutions.

Maintain privacy and obtain consent before publishing donor or beneficiary photographs.

L. DATABASE AND TECHNOLOGY

Use a maintainable modern architecture.

Preferred stack:

- Frontend: Next.js / React with TypeScript.
- Styling: Tailwind CSS.
- Backend: Next.js API or equivalent secure backend.
- Database: PostgreSQL.
- Authentication: Secure role-based authentication.
- ORM: Prisma.
- QR generation: Secure QR library.
- Charts: Recharts.
- PWA: Installable mobile-friendly interface.
- Storage: Secure cloud file storage.

Use a relational database with proper foreign keys, indexes, constraints and transaction handling.

Suggested entities:
Users, Roles, Stalls, StallMembers, FoodItems, Inventory, Investments, Expenses, Orders, OrderItems, Payments, Coupons, CouponRedemptions, ProfitDistributions, DeliveryPartners, Deliveries, Donations, Institutions, AuditLogs.

M. SECURITY AND RELIABILITY

- Secure password hashing.
- Server-side authorization.
- Input validation.
- Rate limiting.
- CSRF protection where applicable.
- Secure payment verification and webhooks.
- Database backups.
- Audit logging.
- Idempotent payment and coupon operations.
- No exposure of secret keys.
- No hardcoded admin credentials.
- Safe error handling.
- Database recovery procedures.

Never store UPI PINs, card PINs or banking passwords.

N. DEVELOPMENT PHASES

Phase 1: Build attractive public homepage and 15-stall interface.

Phase 2: Admin dashboard, login and role management.

Phase 3: Inventory, investments and financial accounting.

Phase 4: QR coupon generation and redemption.

Phase 5: Teacher and student panels.

Phase 6: Customer ordering and payment gateway.

Phase 7: Food Express and delivery tracking.

Phase 8: Donation management.

Phase 9: Testing, security review, deployment and PWA installation.

O. IMPORTANT DEVELOPMENT INSTRUCTIONS

Do not build merely a static UI prototype.

Build working forms, functional buttons, database-backed dashboards, real calculations, secure APIs and proper validations.

Do not use fake payment success or fake GPS tracking.

If payment gateway credentials or external API keys are unavailable, create a clearly labelled sandbox/demo integration and document the exact production setup requirements.

Keep all stall names, food items, members, prices, targets and event settings editable through Admin.

Seed the application with 15 sample stalls and clearly labelled demonstration data.

Write automated tests for coupon duplication, stock reservation, payment verification, profit calculations and role permissions.

First inspect the existing repository, if one exists. Preserve working code and avoid unnecessary rewrites.

Start by preparing the project architecture and database schema, then implement the application in phases. Keep the application runnable at every phase and provide setup and deployment documentation.

FINAL OBJECTIVE: Deliver a beautiful, secure, fully functional E-ANAND MELA digital ecosystem for DAV Public School SECL Gevra, accessible through both mobile and desktop browsers.
