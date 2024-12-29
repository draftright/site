---
layout: post
title: "Bootstrap Layout and Grid System  - Part 2"
subtitle: Day 2
categories: Learning
author: "Dilip Rout"
meta: ""
tags: bootstrap learning
top: 
excerpt_image: https://getbootstrap.com/docs/5.3/assets/img/bootstrap-icons.png
---
![banner](https://getbootstrap.com/docs/5.3/assets/img/bootstrap-icons.png)


**Objective:** Dive deeper into the responsive grid system and layout utilities.

- **Tasks:**
  - Learn about:
    - Container types (.container, .container-fluid, .container-xxl).
    - Rows and columns in the grid system.
    - Breakpoints (sm, md, lg, xl, xxl).
  - Build sample layouts:
    - Create a responsive 3-column layout.
    - Adjust column spans for different screen sizes.
  - Explore spacing utilities:
    - Margins and paddings (.m-, .p-, .g-).

Here’s a detailed **Day 2: Bootstrap Layout and Grid System** course. Today, you’ll dive deeper into creating responsive layouts using Bootstrap's powerful grid system and layout utilities.

**Objective**

- Understand how container types, rows, columns, and breakpoints work in the Bootstrap grid system.
- Build responsive layouts with column spans and explore spacing utilities like margins, paddings, and gutters.

**1\. Understanding Container Types**

In Bootstrap, containers are fundamental for structuring your layout. They act as wrappers for your content.

**A. Types of Containers**

1. **.container**
    - Provides a fixed-width container based on the screen size.
    - The width automatically adjusts at different breakpoints.
2. **.container-fluid**
    - Provides a full-width container that spans the entire width of the viewport, regardless of screen size.
3. **.container-xxl**
    - A hybrid container that behaves like .container but extends to an extra-large breakpoint (xxl) for high-resolution screens.

**B. Example Code**

html

&lt;div class="container"&gt;

&lt;p&gt;This is a fixed-width container.&lt;/p&gt;

&lt;/div&gt;

&lt;div class="container-fluid bg-light"&gt;

&lt;p&gt;This is a full-width container.&lt;/p&gt;

&lt;/div&gt;

&lt;div class="container-xxl bg-secondary text-white"&gt;

&lt;p&gt;This is a container optimized for extra-large screens.&lt;/p&gt;

&lt;/div&gt;

**2\. Rows and Columns in the Grid System**

The grid system allows you to create layouts with a 12-column system.

**A. Basic Grid Syntax**

1. **.row**
    - Use the .row class to group your columns.
2. **.col-\***
    - Specify how many columns an element spans with .col-\* classes (e.g., .col-4, .col-6).
    - The total column span in a row must add up to 12 for a full-width layout.

**B. Example Code**

A simple layout with three equal-width columns:

html

&lt;div class="container"&gt;

&lt;div class="row"&gt;

&lt;div class="col"&gt;Column 1&lt;/div&gt;

&lt;div class="col"&gt;Column 2&lt;/div&gt;

&lt;div class="col"&gt;Column 3&lt;/div&gt;

&lt;/div&gt;

&lt;/div&gt;

**3\. Breakpoints**

Breakpoints define how your layout responds to different screen sizes.

**A. Available Breakpoints**

- sm (small): ≥576px
- md (medium): ≥768px
- lg (large): ≥992px
- xl (extra large): ≥1200px
- xxl (extra extra large): ≥1400px

**B. Customizing Column Spans for Breakpoints**

Specify different column spans for different breakpoints using classes like .col-sm-\*, .col-md-\*, etc.

Example:

html

&lt;div class="container"&gt;

&lt;div class="row"&gt;

&lt;div class="col-12 col-md-6 col-lg-4"&gt;Column 1&lt;/div&gt;

&lt;div class="col-12 col-md-6 col-lg-4"&gt;Column 2&lt;/div&gt;

&lt;div class="col-12 col-lg-4"&gt;Column 3&lt;/div&gt;

&lt;/div&gt;

&lt;/div&gt;

**Explanation**:

- On small screens (<768px): All columns take up the full width (col-12).
- On medium screens (≥768px): Each column spans half the width (col-md-6).
- On large screens (≥992px): Columns span one-third of the width (col-lg-4).

**4\. Building Sample Layouts**

**A. Responsive 3-Column Layout**

Create a layout where the columns adjust responsively:

html

&lt;div class="container"&gt;

&lt;div class="row"&gt;

&lt;div class="col-12 col-md-4"&gt;Column 1&lt;/div&gt;

&lt;div class="col-12 col-md-4"&gt;Column 2&lt;/div&gt;

&lt;div class="col-12 col-md-4"&gt;Column 3&lt;/div&gt;

&lt;/div&gt;

&lt;/div&gt;

**B. Nested Columns**

Nest rows and columns to create complex layouts.

html

&lt;div class="container"&gt;

&lt;div class="row"&gt;

&lt;div class="col-6"&gt;

&lt;div class="row"&gt;

&lt;div class="col"&gt;Nested Column 1&lt;/div&gt;

&lt;div class="col"&gt;Nested Column 2&lt;/div&gt;

&lt;/div&gt;

&lt;/div&gt;

&lt;div class="col-6"&gt;Column 2&lt;/div&gt;

&lt;/div&gt;

&lt;/div&gt;

**5\. Spacing Utilities**

Bootstrap includes utility classes for managing spacing (margins, padding, and gutters).

**A. Margins and Padding**

- Margins (.m-\*) control the space **outside** an element.
- Padding (.p-\*) controls the space **inside** an element.
- Add values: 0 (none), 1 (0.25rem), 2 (0.5rem), 3 (1rem), 4 (1.5rem), 5 (3rem), and auto.

Example:

html

&lt;div class="container"&gt;

&lt;div class="row"&gt;

&lt;div class="col p-3 m-2 bg-primary text-white"&gt;Column 1&lt;/div&gt;

&lt;div class="col p-3 m-2 bg-success text-white"&gt;Column 2&lt;/div&gt;

&lt;/div&gt;

&lt;/div&gt;

**B. Gutters**

Gutters are the spaces between columns.

- By default, Bootstrap adds gutters between columns in a row.
- You can adjust or remove gutters using .g-\* classes.

Example:

html

&lt;div class="container"&gt;

&lt;div class="row g-3"&gt;

&lt;div class="col"&gt;Column 1&lt;/div&gt;

&lt;div class="col"&gt;Column 2&lt;/div&gt;

&lt;/div&gt;

&lt;/div&gt;

**C. Combining Spacing Utilities**

Combine margin and padding utilities for advanced control.

Example:

html

&lt;div class="container"&gt;

&lt;div class="row"&gt;

&lt;div class="col p-5 m-4 bg-warning text-dark"&gt;Column with padding and margin&lt;/div&gt;

&lt;/div&gt;

&lt;/div&gt;

**6\. Summary and Practice**

**What You Learned**

- The different types of containers (.container, .container-fluid, .container-xxl).
- How rows and columns work in Bootstrap's grid system.
- How to use breakpoints (sm, md, lg, etc.) for responsive designs.
- The use of spacing utilities for margins, paddings, and gutters.

**Practice Tasks**

1. Create a layout with:
    - A fixed-width container containing a header, main content, and footer.
    - The main content should have two columns: one taking up 8 units and the other 4 units.
    - Adjust the layout so that both columns take up 12 units on small screens.
2. Experiment with margins, paddings, and gutters to fine-tune your layouts.

Let me know if you’d like additional clarification or assistance! Ready for Day 3? 😊

Bottom of Form