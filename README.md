# Shipping-service
World Express Delivery Service 
PROJECT: PROFESSIONAL INTERNATIONAL COURIER AND LOGISTICS MANAGEMENT WEBSITE

Act as a senior full-stack web developer, UI/UX designer, database architect, and cybersecurity engineer. Build a professional, production-oriented international courier and logistics website for my delivery company.

This is a serious business project. Do not create only a static landing page or a visual prototype. Build the actual functional features wherever the platform supports them. If a feature requires an external service, API key, paid subscription, domain, or additional setup, clearly identify that requirement rather than pretending it works.

1. BRANDING AND VISUAL DESIGN

Create a premium, elegant, modern international logistics website.

Design requirements:

- Primary colors: white and bright golden yellow.
- Secondary colors: dark charcoal, black, and subtle grey.
- Clean white backgrounds with tasteful yellow highlights.
- Professional typography, attractive cards, smooth animations, clear icons, and generous spacing.
- Responsive design for Android phones, iPhones, tablets, laptops, and desktops.
- A premium corporate appearance comparable to an established international courier company.
- Fast-loading pages, accessible text, intuitive navigation, and clear buttons.
- Create a customizable company logo featuring a professional shipping, parcel, globe, or delivery symbol.
- Allow the administrator to upload and replace the company logo without editing source code.
- Display the company logo consistently in the website header, customer dashboard, tracking page, email templates, receipts, invoices, and downloadable documents.

Use a temporary company name, “YOUR COURIER COMPANY,” until I replace it with my real registered business name. Do not invent company registration numbers, addresses, certifications, licenses, or other official credentials.

2. PUBLIC WEBSITE

Build the following public pages:

1. Home
2. About Us
3. Our Services
4. Domestic Shipping
5. International Shipping
6. Track a Shipment
7. Request a Shipping Quote
8. Shipping Rates and Conditions
9. Frequently Asked Questions
10. Contact Us
11. Privacy Policy
12. Terms and Conditions
13. Shipping, Damage, Loss, and Claims Policy
14. Refund and Cancellation Policy

The homepage should include:

- Company branding and a professional navigation bar.
- A prominent shipment-tracking search field.
- A “Create Shipment” button.
- A “Track Package” button.
- An international shipping destination selector.
- An overview of available delivery services.
- Customer benefits and support information.
- A contact section and footer.

Do not show fabricated testimonials, fake customer numbers, fake ratings, or unverified claims about worldwide operations.

3. CUSTOMER REGISTRATION AND AUTHENTICATION

Build a secure customer registration and login system.

Registration fields:

- Full legal name.
- Email address.
- Phone number with international country code.
- Residential or business address.
- Country and city.
- Password and password confirmation.
- Agreement to the privacy policy and terms.

Email verification:

- Generate a secure, random, time-limited, single-use OTP.
- Send the OTP to the customer's email address.
- Require successful verification before completing account activation.
- Limit verification attempts and OTP resends.
- Never store OTPs in plaintext or expose them in browser code or application logs.

Manual account approval:

- After email verification, place the customer account in “Pending Administrator Approval.”
- Notify the administrator of the pending account.
- Allow the administrator to approve, reject, suspend, or reactivate accounts.
- Notify customers by email when their account is approved or rejected.
- Prevent unapproved or suspended users from booking shipments or accessing protected features.

Account management:

- Secure login and logout.
- Forgot-password and password-reset functions.
- Change-password functionality.
- Session management and suspicious-login protections.
- Customer profile editing.
- Optional administrator-configurable additional verification.

Each customer must see only their own profile, shipments, documents, invoices, support tickets, and private notifications.

4. CUSTOMER DASHBOARD

Create a premium customer portal with a sidebar or mobile-friendly navigation.

Include:

- Dashboard overview.
- My Profile.
- Create a Shipment.
- My Shipments.
- Track a Shipment.
- Received Shipments.
- Shipping Quotes.
- Receipts and Invoices.
- Notifications.
- Support Tickets.
- Security Settings.
- Logout.

Display summary cards for:

- Pending shipments.
- Approved shipments.
- Packages received by the company.
- Packages in transit.
- Shipments undergoing clearance.
- Packages out for delivery.
- Delivered shipments.
- Shipments on hold or cancelled.

Customers should be able to filter shipments by tracking number, date, status, origin, and destination.

The “Received Shipments” section should distinguish between packages physically received by the courier company and packages delivered to the final recipient. Never mark a package as physically received or delivered without an authorized, recorded update.

5. INTERNATIONAL SHIPMENT BOOKING

Create a detailed shipment request form with separate sender and recipient sections.

Sender information

- Full name.
- Company name, if applicable.
- Email address.
- Phone number with country code.
- Street address.
- Apartment, suite, or building details.
- Country.
- State, province, or region.
- City.
- Postal or ZIP code.

Recipient information

- Full name.
- Company name, if applicable.
- Email address.
- Phone number with country code.
- Complete street address.
- Apartment, suite, or building details.
- Country.
- State, province, or region.
- City.
- Postal or ZIP code.
- Delivery instructions.

Package information

- Package description.
- Package category.
- Number of packages.
- Actual weight.
- Length, width, and height.
- Weight unit and dimension unit.
- Declared value and currency.
- Optional insurance selection.
- Fragile-item indicator.
- Special handling instructions.
- Required customs or shipping documentation.
- Requested shipping service.
- Preferred dispatch date, if available.

Personal message

Include an optional field where the sender can write a greeting, personal message, or delivery note for the recipient. Keep personal messages separate from customs declarations and operational instructions.

Allow the customer to review the complete booking before submitting it.

Country and city selection

- Provide searchable international country lists.
- Support country-dependent state, province, city, and postal-code fields.
- Use a maintained geographic database or reliable location API.
- Support international address formats and phone numbers.
- Allow the administrator to configure supported origin countries, destination countries, routes, and service restrictions.
- Display a clear message when a requested route is not supported.
- Do not claim that every destination is serviceable merely because it appears in the country selector.

6. ADMINISTRATOR APPROVAL WORKFLOW

Create a separate, private administrator portal.

Only explicitly authorized administrators may access it. Customer accounts must never receive administrator privileges through registration or ordinary profile editing.

The administrator must manually control the important operational decisions.

Include approval queues for:

- New customer registrations.
- New shipment requests.
- Shipment price quotes.
- Requested shipment changes.
- Cancellation requests.
- Address or destination changes.
- Refund requests, if payments are enabled.
- Shipment completion and delivery confirmation.

For each request, provide:

- View complete details.
- Approve.
- Reject.
- Request additional information.
- Place on hold.
- Cancel, when appropriate.
- Add an internal note.
- Add a customer-visible message.
- Record the decision and timestamp.

Require confirmation before consequential actions. Record the administrator responsible for each action.

A shipment must not be approved, cancelled, delivered, or modified solely because a customer changes a browser field or submits an untrusted request.

7. SHIPMENT MANAGEMENT AND TRACKING

Every approved shipment must have a unique, unpredictable tracking reference that cannot be easily guessed.

Example format: CARGO-2026-8F3K92.

Do not reuse tracking numbers. Prevent collisions and unauthorized access to tracking records.

Create a configurable shipment-status system with the following default stages:

1. Shipment Request Submitted.
2. Pending Administrator Approval.
3. Shipment Approved.
4. Awaiting Package Drop-off.
5. Package Received at Facility.
6. Package Inspection and Processing.
7. Documentation Processing.
8. Export Clearance in Progress.
9. Export Clearance Completed.
10. Dispatched from Origin Facility.
11. In Transit.
12. Arrived at Transit Facility.
13. Import Clearance in Progress.
14. Import Clearance Completed.
15. Final Release or Additional Inspection.
16. Arrived at Destination Facility.
17. Out for Delivery.
18. Delivery Attempted.
19. Delivered.
20. On Hold.
21. Address or Documentation Issue.
22. Clearance Exception.
23. Returned to Sender.
24. Cancelled.

Allow the administrator to add, rename, reorder, enable, or disable optional stages.

Not every shipment must pass through every stage. The administrator must select the applicable stage and record a real operational event.

Tracking updates

For every update, record:

- Shipment reference.
- Previous status.
- New status.
- Date and time.
- Recorded location.
- Public tracking description.
- Optional internal note.
- Administrator or authorized staff member responsible.
- Supporting document or proof, when applicable.

Display a professional timeline with completed stages, the current stage, timestamps, and future stages clearly distinguished.

Allow the administrator to correct mistakes, but preserve the original event in the audit history.

Do not display fabricated GPS positions, simulated physical scans, or automatic delivery confirmations. Map tracking should use verified location data or be clearly labelled as an estimated route.

8. QR CODES, BARCODES, AND TRACKING

Generate a QR code and a scannable barcode for every approved shipment.

Print both on the official shipment receipt and shipping label.

Requirements:

- The barcode must encode the shipment's tracking reference.
- The QR code should open the official tracking page using the shipment's actual tracking reference.
- Use a reliable QR-code library and barcode format, such as Code 128.
- Ensure the codes have sufficient resolution, contrast, and quiet space for scanning.
- Test the generated codes with real scanning software.
- Never use a decorative image as a substitute for a working barcode or QR code.
- Do not encode passwords, private customer information, or confidential shipment details in the QR code.

Include a manual tracking-number search for customers who cannot scan the code.

9. PROFESSIONAL SHIPPING RECEIPT AND WAYBILL

Create a premium, print-ready receipt design using the company logo and white-and-yellow corporate branding.

The receipt must look like a genuine business document, with consistent spacing, readable typography, clear section headings, and a professional layout.

Include:

Company section

- Company logo.
- Company name.
- Registered business address, once supplied.
- Official contact information.
- Customer service email.
- Website address.
- Receipt or waybill number.
- Document issue date.
- Company registration and tax details only if supplied and verified.

Sender section

- Full name.
- Email.
- Phone.
- Complete address.
- Country and city.

Recipient section

- Full name.
- Email.
- Phone.
- Complete address.
- Country and city.

Shipment section

- Unique tracking number in large, bold, readable text.
- Scannable barcode.
- Scannable QR code.
- Shipment creation date.
- Package description.
- Number of packages.
- Actual weight and dimensions.
- Origin and destination.
- Shipping service.
- Applicable customs or documentation information.
- Current shipment status.
- Estimated delivery date, only when reasonably available.
- Declared value and insurance information, if applicable.

Financial section

- Shipping charge.
- Packaging or handling charge, if applicable.
- Applicable taxes.
- Additional service charges.
- Customs duties or import charges, when applicable and properly identified.
- Late-payment charges only when authorized by the disclosed agreement and permitted by applicable law.
- Discounts, payments received, outstanding balance, and total amount due.
- Currency displayed clearly.

Do not label a quote as a paid receipt. Distinguish a quote, booking confirmation, issued invoice, payment receipt, and waybill according to their actual purpose and status.

Allow the administrator to generate, preview, print, and download receipts as PDF files. Provide the option to email the document to the sender.

Receipt notice and shipping terms

Include a concise notice such as:

“Please inspect the shipment upon receipt and report any visible damage, loss, or discrepancy promptly through our official customer service channel. Packaging, declared-value requirements, claims deadlines, compensation, exclusions, and liability for loss or damage are governed by the shipping agreement and applicable law.”

Include a payment notice such as:

“Please pay the charges stated on your official invoice by the specified due date. Any applicable late-payment fee must be disclosed in advance, authorized by the agreed terms, and permitted by applicable law.”

Allow the administrator to edit these notices and configure the actual terms before issuing documents.

Do not automatically state that customers are responsible for every damaged item. Responsibility for damage must be determined according to the applicable agreement, evidence, and law.

10. AUTOMATED EMAIL NOTIFICATIONS

Use a real transactional email service connected to the company's verified domain.

Provide configurable templates for:

- OTP verification.
- Successful email verification.
- Account approval or rejection.
- Shipment request received.
- Shipment approved or rejected.
- Tracking number issued.
- Package received at the courier facility.
- Shipment dispatched.
- Shipment in transit.
- Clearance updates.
- Shipment delayed or placed on hold.
- Additional documentation requested.
- Destination or address change approved or rejected.
- Shipment cancelled.
- Invoice issued.
- Payment received.
- Payment reminder.
- Delivery attempted.
- Shipment delivered.
- Support ticket reply.

Send notifications after the corresponding action has been successfully committed to the database.

The administrator must be able to enable or disable individual notification types and edit their templates.

Every email should contain:

- Company logo.
- Professional subject line.
- Customer's name, where appropriate.
- Shipment reference.
- Relevant status and timestamp.
- A secure link to the customer dashboard or tracking page.
- Customer support details.

Configure SPF, DKIM, and DMARC for the company domain.

Record email-provider message IDs, sending attempts, and delivery events where supported. Handle failed email deliveries with controlled retries and a visible administrative warning.

Never display an email as successfully delivered when the provider has not confirmed delivery.

11. FULL ADMINISTRATOR DASHBOARD

Create a premium private dashboard with the following modules.

Overview

- Total registered customers.
- Accounts awaiting approval.
- Total shipment requests.
- Shipments awaiting approval.
- Packages received.
- Packages in transit.
- Shipments undergoing clearance.
- Delivered and cancelled shipments.
- Outstanding invoices.
- Recent administrative activity.

Customer management

- Search and filter customers.
- Review registration details.
- Approve or reject accounts.
- Suspend and reactivate accounts.
- View individual shipment histories.
- Initiate a password reset without revealing a customer's existing password.
- Review verification status.
- Record administrative notes with appropriate privacy restrictions.

Shipment management

- Search by tracking number, customer, origin, destination, or status.
- Create shipments on behalf of customers.
- Edit shipment details with an audit record.
- Approve, reject, hold, resume, or cancel shipments.
- Assign or correct tracking references under controlled procedures.
- Change the current shipment stage.
- Add tracking events and locations.
- Upload supporting documentation.
- Generate or regenerate receipts and waybills.
- Set approved quotes and invoice amounts.
- Record payments only from verified payment evidence.
- Mark delivery complete only after an authorized confirmation.
- Record the reason for any exceptional status change.

Configurable company settings

- Company logo and branding.
- Company name and contact details.
- Supported countries and routes.
- Shipping services.
- Status stages.
- Pricing rules.
- Currency settings.
- Tax configuration.
- Invoice numbering.
- Receipt and waybill templates.
- Customer notification settings.
- Shipping policies and terms.
- Email provider settings.

Never expose email-provider API keys, payment secrets, database credentials, or other sensitive configuration in the frontend.

12. ADMINISTRATOR PRIVACY AND CYBERSECURITY

Implement strong security at the application and database levels.

- Separate administrator and customer authentication flows.
- Require multifactor authentication for administrators.
- Enforce server-side role-based access control.
- Deny access by default to protected resources.
- Apply object-level authorization to every customer, shipment, invoice, and document.
- Prevent insecure direct-object-reference vulnerabilities.
- Use secure password hashing.
- Apply rate limits to logins, OTP requests, password recovery, and public tracking searches.
- Use secure session cookies, HTTPS, CSRF protection where applicable, input validation, and output encoding.
- Use parameterized database queries or a secure ORM.
- Protect file uploads against malicious files and unauthorized access.
- Store private documents in restricted storage.
- Keep secrets in environment variables or a managed secrets service.
- Record administrator actions in append-only or tamper-evident audit logs.
- Maintain encrypted backups and test recovery procedures.
- Implement account lockout or progressive delays for repeated suspicious attempts.
- Provide a way to revoke sessions and disable compromised accounts.
- Minimize the collection of personal data and define appropriate retention periods.
- Do not log passwords, OTPs, payment secrets, or unnecessary personal information.

Only the authorized administrator should be able to access all customer and shipment records. If additional staff accounts are introduced, permissions must be limited to their assigned duties.

Do not promise absolute privacy or immunity from hacking. Document the system's security measures and limitations.

13. OPTIONAL PAYMENTS AND SHIPPING QUOTES

Prepare the architecture for future online payments, but do not activate payment collection without a configured, verified payment provider.

Allow the administrator to:

- Set or approve shipping quotes.
- Configure rate rules.
- Review charges before an invoice is issued.
- Record authorized adjustments.
- Review verified payment confirmations.
- Issue refunds through the payment provider when supported.

If payment integration is activated:

- Use the provider's secure checkout.
- Verify payment notifications server-side.
- Never trust a browser message as proof of payment.
- Never store raw card numbers or CVV codes.
- Prevent duplicate payment processing.
- Clearly identify the currency, due date, applicable fees, refund conditions, and payment status.

14. SUPPORT CENTRE

Create a customer support ticket system.

Customers can:

- Open a ticket.
- Select a topic.
- Link a ticket to a shipment.
- Submit a message.
- Attach permitted files.
- View replies and ticket status.

Administrators can:

- Review all support tickets.
- Assign priority.
- Reply to customers.
- Add private internal notes.
- Request additional information.
- Close or reopen a ticket.
- View the relevant shipment record.

Send email notifications for new replies and significant ticket-status changes.

15. DATABASE AND BACKEND

Design a normalized, secure database with appropriate relationships, constraints, indexes, and migrations.

Include entities for:

- Users.
- Customer profiles.
- Administrator roles and permissions.
- Email verification challenges.
- Shipments.
- Sender details.
- Recipient details.
- Shipment packages.
- Tracking events.
- Shipment status definitions.
- Shipment change requests.
- Quotes.
- Invoices.
- Payments.
- Receipts and waybills.
- Email notification logs.
- Support tickets and replies.
- Private document metadata.
- Audit logs.
- Company configuration.
- Supported countries, cities, routes, and services.

Enforce appropriate foreign keys and transaction boundaries. Make tracking references unique. Use safe deletion and retention policies so important financial and audit records are not accidentally erased.

Keep an immutable record of important shipment events even when editable shipment details change.

16. REQUIRED FUNCTIONAL TESTING

Before declaring the website complete, test the following:

1. A customer can register and receive a real OTP email.
2. An invalid or expired OTP cannot verify an account.
3. A verified customer remains pending until administrator approval.
4. An unapproved customer cannot create an approved shipment.
5. A customer cannot access another customer's private information by modifying a URL or request.
6. An administrator can approve, reject, edit, hold, and cancel shipments.
7. Shipment status changes appear correctly in the customer portal.
8. Configured email notifications are sent for the relevant events.
9. Tracking numbers are unique.
10. QR codes open the correct tracking page.
11. Barcodes can be scanned and return the correct tracking reference.
12. Receipts show the actual company logo, sender details, recipient details, tracking reference, charges, and applicable terms.
13. The receipt prints correctly and downloads as a readable PDF.
14. Unauthorized users cannot access the admin dashboard or private documents.
15. Failed email sends are logged and handled appropriately.
16. Payment statuses cannot be forged by a customer.
17. The interface works on mobile and desktop.
18. Database backups can be restored successfully.

Do not mark tests as passed without actually running them.

17. DELIVERY REQUIREMENTS

First, inspect the capabilities of the website-building platform and choose an implementation appropriate to the available environment.

Then:

1. Build the branded public website.
2. Implement the database and backend.
3. Implement secure authentication and OTP verification.
4. Build the customer portal.
5. Build the private administrator dashboard.
6. Implement shipment approvals and configurable tracking stages.
7. Generate working barcodes, QR codes, receipts, and PDFs.
8. Connect and test transactional email.
9. Apply access controls and security protections.
10. Test the complete booking-to-delivery workflow.
11. Provide setup instructions for the domain, hosting, database, email service, backups, and secrets.
12. Provide a list of features that work, features that still require configuration, and any features the platform cannot support.

Do not fabricate successful integrations, live shipment data, real payments, email delivery, or test results.

The final product should be a polished, extensible international courier management system with manual administrator approval at its core.

My priority is complete operational control, customer privacy, reliable shipment tracking, professional company branding, authentic documentation, and a premium customer experience.
