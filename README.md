1. Created index.html file

Purpose

- This is the landing page for a receptionist/visitor-management app.
- Ithas a welcoming hero, simple navigation, check-in and check-out forms, an about section, a contact section, a static AI Assistant placeholder, testimonials, and a footer.

Header & Navigation

- Top bar with logo (placeholder image or text) and site name “SmartReception”.
- Navigation with links that jump (anchor links) to sections on the same page:
  Home (#home)
  Features (#features)
  Check In (#check-in)
  Check Out (#check-out)
  About (#about)
  Contact (#contact)

Hero (Home)

- Prominent headline: “Welcome to SmartReception”.
- Subheadline: “Fast, easy, and secure visitor management.”
- A primary button styled via CSS that links to the Check In section (#check-in).
- A hero illustration placeholder (<img> with alt text).

Features Section (#features)

- Grid or list of static feature descriptions such as:
  - Digital Check-In and Check-Out
  - Instant Host Notifications
  - Secure Visitor Logs
  - Appointment Scheduling
  - Multilingual Support
  - Touch-Free QR Check-In
  - Cloud-Based Storage
- Each feature has a heading and short descriptive paragraph.

Check-In Section (#check-in)

- Short intro text.
- Form (method="post", action="#"):
  - Full Name (text, required)
  - Contact Number (tel, required, basic pattern)
  - Company / Organization (text, optional)
  - Purpose of Visit (select: Meeting, Interview, Delivery, Maintenance, Other)
  - Host Name (text, required)
  - Date (date, required)
  - Time (time, required)
  - Terms checkbox (required): “I agree to the visitor policy.”
  - Submit button labeled “Check In”

Check-Out Section (#check-out)

- Short explanation.
- Form (method="post", action="#"):
  Full Name (text, required)
  Contact Number (tel, required)
  Time of Departure (time, required)
  Submit button labeled “Check Out”

AI Assistant Placeholder Section

- Static box with text: “Chat with our AI Receptionist (Coming Soon)”.
- A mock chat interface made of static HTML (no functionality).

Testimonials Section

- Two or three short testimonials in blockquotes with names and roles.

About Section (#about)

- Two short paragraphs describing SmartReception benefits.
- A static unordered list of advantages.

Contact Section (#contact)

- Static address block (<address>), email mailto link, and phone tel link.
- A simple FAQ using <details><summary> for 2–3 questions.

Footer

- Copyright line with the current year.
- Links to Terms and Privacy (dummy anchors).
- Social media text links

STYLING

I created an external file called styles.css

FEATURES

This project uses a custom CSS theme with consistent color variables, spacing rules, typography, and responsive layouts.
Below is an overview of how the styling is structured:

1. Global Reset & Variables

Resets all margins, paddings, and sets box-sizing: border-box.

Defines :root CSS variables for primary, secondary, light, dark colors, gradients, shadows, and border radius.

Uses a modern, clean font stack:
"Segoe UI", Tahoma, Geneva, Verdana, sans-serif.

2. Layout Structure

.container for centered content with responsive padding.

Sticky header with box shadow and transparent white background.

Main content with rounded corners, soft shadow, and alternating section backgrounds.

Responsive breakpoints:

@media (max-width: 768px) → tablet adjustments.

@media (max-width: 480px) → mobile adjustments.

3. Component Styles

Header & Navigation

Flexible layout with horizontal nav links.

Hover and focus states for better accessibility.

Hero Section

Split layout with text and image (switches to stacked on mobile).

Call-to-action button with smooth hover animations.

Features

Grid & horizontal scroll layouts for feature cards.

Hover lift effect for interactivity.

Forms

Styled inputs, selects, textareas with focus glow.

.btn-submit with smooth color transition and shadow on hover.

AI Assistant

Chat bubble styling for AI and user messages.

Scrollable message area with clean input box.

Testimonials

Quote block styling with decorative quotation marks.

About & Contact

Checklist style lists with green checkmarks.

Address cards with hover link effects.

FAQ

Collapsible <details> styling with smooth spacing.

Footer

Dark background, centered content, hover effects for links.

4. Accessibility Features

Skip Link for keyboard navigation.

High contrast for important interactive elements.

Focus states for all buttons and links.

5. Color Palette
   Variable Color
   --primary #2c6fbb
   --primary-light #4a8fd4
   --secondary #3aafa9
   --dark #2b2d42
   --light #f8f9fa
   --gray #6c757d
   --light-gray
