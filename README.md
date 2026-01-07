➕ Accordion Activity - Plus and Ticks

A streamlined, interactive accordion component designed for structured information delivery. This tool features a "one-at-a-time" expansion logic, high-contrast brand styling, and custom decorative list elements.

🚀 Live Demo

Explore the Accordion Activity Component Here

✨ Project Overview

The Accordion Activity component is optimized for readability and focus. It uses a "Plus" (+) icon system that rotates during interaction and a unique "Tick" (✓) list style to present key points clearly within expanded sections.

Key Features

Mutual Exclusion Logic: Expanding one section automatically collapses all other open sections, ensuring the user's focus remains on a single topic.

Animated State Changes: * Panel Reveal: Utilizes a slideIn keyframe animation for a smooth downward entrance.

Icon Rotation: The plus (+) icon rotates 45 degrees when active, providing a subtle visual cue for the "Close" state.

Custom Brand Iconography: Replaces standard bullet points with Teal-colored checkmarks (✓) using CSS ::before pseudo-elements.

Sub-Category Organization: Supports labeled sub-categories within sections to handle complex or multi-part content.

Responsive Container: The activity-card is capped at 850px for optimal line length and readability across desktop and tablet devices.

🛠️ Technical Implementation

Interaction Logic: A single JavaScript function toggleSection(header) manages the state of the DOM. It queries all active sections to reset them before applying the .active class to the clicked element.

CSS Architecture:

Transitions: Smooth transitions for background colors and icon transforms.

Flexbox Headers: Uses justify-content: space-between to keep titles and toggle icons perfectly aligned regardless of content width.

Typography: Leverages the Inter font family for a modern, professional aesthetic.

📂 Design Tokens

Midnight Blue (#1f2a52): Primary background for headers and main titles.

Teal (#00bec7): Interaction highlight color (hover/active states) and checkmark icons.

Light Aqua (#d2f0f0): Used for subtle borders and sub-category underlines.

Slate Grey (#abb5bf): Tertiary color used for shadows and softer UI borders.

📖 Usage Instructions

To add new sections to the accordion, follow this HTML structure inside the .main-content div:

<!-- New Section Header -->
<div class="section-header" onclick="toggleSection(this)">
    Section Title Here
    <span class="toggle-icon">+</span>
</div>
<!-- New Section Content -->
<div class="section-content">
    <span class="sub-category">Optional Subtitle</span>
    <ul>
        <li><strong>Bold Point:</strong> Regular description text.</li>
    </ul>
</div>


📄 License

MIT License - Developed as part of the accounts-eles UI component library.
