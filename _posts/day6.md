Day 6

# Day 5: Customization with Sass

**Objective:** Customize Bootstrap using Sass.

- **Tasks:**
  - Install Sass (if not already installed).
  - Learn how to modify Bootstrap's default variables:
    - Colors.
    - Breakpoints.
    - Spacing.
  - Build a custom Bootstrap theme:
    - Override the default styles.
    - Compile your Sass changes into a custom CSS file.


# Day 6: JavaScript Components

**Objective:** Understand and implement Bootstrap’s JavaScript components.

- **Tasks:**
  - Learn to use:
    - Dropdowns.
    - Collapsibles.
    - Modals.
    - Tooltips and popovers.
  - Practice initializing these components using:
    - Data attributes.
    - JavaScript methods.
  - Integrate third-party libraries if needed (e.g., jQuery).

**Day 6: JavaScript Components**

Today’s focus is on understanding and implementing Bootstrap’s JavaScript-powered components. These dynamic components enhance interactivity and user experience on your web pages.

**Objective**

- Learn to use Bootstrap’s JavaScript components such as dropdowns, modals, collapsibles, tooltips, and popovers.
- Practice initializing these components using data attributes and JavaScript methods.
- Optionally, explore integrating third-party libraries like jQuery if needed.

**1\. Setup**

**A. Include Bootstrap JavaScript**

Ensure Bootstrap’s JavaScript is included in your project.

- Use Bootstrap’s official CDN:

html

&lt;script src="<https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/js/bootstrap.bundle.min.js"&gt;&lt;/script>&gt;

- Alternatively, download and link bootstrap.bundle.min.js.

**B. Optional: Add jQuery**

If your project relies on jQuery, include it as well:

html

&lt;script src="<https://code.jquery.com/jquery-3.6.4.min.js"&gt;&lt;/script>&gt;

**2\. Dropdowns**

**A. Using Data Attributes**

Example:

html

&lt;div class="dropdown"&gt;

&lt;button class="btn btn-secondary dropdown-toggle" type="button" id="dropdownMenuButton" data-bs-toggle="dropdown" aria-expanded="false"&gt;

Dropdown button

&lt;/button&gt;

&lt;ul class="dropdown-menu" aria-labelledby="dropdownMenuButton"&gt;

&lt;li&gt;&lt;a class="dropdown-item" href="#"&gt;Action&lt;/a&gt;&lt;/li&gt;

&lt;li&gt;&lt;a class="dropdown-item" href="#"&gt;Another action&lt;/a&gt;&lt;/li&gt;

&lt;li&gt;&lt;a class="dropdown-item" href="#"&gt;Something else here&lt;/a&gt;&lt;/li&gt;

&lt;/ul&gt;

&lt;/div&gt;

**B. Using JavaScript**

Initialize the dropdown using JavaScript:

html

&lt;script&gt;

const dropdownTrigger = document.getElementById('dropdownMenuButton');

const dropdown = new bootstrap.Dropdown(dropdownTrigger);

&lt;/script&gt;

**3\. Collapsibles**

**A. Using Data Attributes**

Example:

html

&lt;p&gt;

&lt;a class="btn btn-primary" data-bs-toggle="collapse" href="#collapseExample" role="button" aria-expanded="false" aria-controls="collapseExample"&gt;

Toggle Content

&lt;/a&gt;

&lt;/p&gt;

&lt;div class="collapse" id="collapseExample"&gt;

&lt;div class="card card-body"&gt;

This is collapsible content!

&lt;/div&gt;

&lt;/div&gt;

**B. Using JavaScript**

Initialize and toggle a collapse programmatically:

html

&lt;script&gt;

const collapseElement = document.getElementById('collapseExample');

const collapse = new bootstrap.Collapse(collapseElement);

&lt;/script&gt;

**4\. Modals**

**A. Using Data Attributes**

Example:

html

&lt;button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModal"&gt;

Launch Modal

&lt;/button&gt;

&lt;div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true"&gt;

&lt;div class="modal-dialog"&gt;

&lt;div class="modal-content"&gt;

&lt;div class="modal-header"&gt;

&lt;h5 class="modal-title" id="exampleModalLabel"&gt;Modal title&lt;/h5&gt;

&lt;button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"&gt;&lt;/button&gt;

&lt;/div&gt;

&lt;div class="modal-body"&gt;

Modal content goes here!

&lt;/div&gt;

&lt;div class="modal-footer"&gt;

&lt;button type="button" class="btn btn-secondary" data-bs-dismiss="modal"&gt;Close&lt;/button&gt;

&lt;button type="button" class="btn btn-primary"&gt;Save changes&lt;/button&gt;

&lt;/div&gt;

&lt;/div&gt;

&lt;/div&gt;

&lt;/div&gt;

**B. Using JavaScript**

Control modals dynamically:

html

&lt;script&gt;

const modalElement = document.getElementById('exampleModal');

const modal = new bootstrap.Modal(modalElement);

modal.show(); // To open the modal

&lt;/script&gt;

**5\. Tooltips and Popovers**

**A. Tooltips**

Add tooltips to elements using data-bs-toggle="tooltip".  
Example:

html

&lt;button type="button" class="btn btn-secondary" data-bs-toggle="tooltip" data-bs-placement="top" title="Tooltip text"&gt;

Hover me

&lt;/button&gt;

&lt;script&gt;

const tooltipTriggerList = \[\].slice.call(document.querySelectorAll('\[data-bs-toggle="tooltip"\]'));

const tooltipList = tooltipTriggerList.map(function (tooltipTriggerEl) {

return new bootstrap.Tooltip(tooltipTriggerEl);

});

&lt;/script&gt;

**B. Popovers**

Add popovers to elements using data-bs-toggle="popover".  
Example:

html

&lt;button type="button" class="btn btn-secondary" data-bs-toggle="popover" data-bs-content="Popover text"&gt;

Click me

&lt;/button&gt;

&lt;script&gt;

const popoverTriggerList = \[\].slice.call(document.querySelectorAll('\[data-bs-toggle="popover"\]'));

const popoverList = popoverTriggerList.map(function (popoverTriggerEl) {

return new bootstrap.Popover(popoverTriggerEl);

});

&lt;/script&gt;

**6\. Practice Tasks**

**A. Dropdowns**

Create a dropdown menu with links for “Home,” “About,” and “Contact.”

**B. Collapsibles**

Create an accordion with three sections that can be collapsed and expanded.

**C. Modals**

Build a modal with a form containing Name and Email fields.

**D. Tooltips and Popovers**

Add tooltips to buttons and popovers to icons in a navigation bar.

**7\. Summary and Next Steps**

**What You Learned**

- Implemented dropdowns, collapsibles, modals, tooltips, and popovers.
- Used both data attributes and JavaScript to initialize and control components.

**Next Steps**

- Experiment with customizing component behavior using JavaScript options and methods.
- Combine multiple components to create a dynamic user interface.

Let me know if you’d like detailed code for the practice tasks or help integrating these components into a larger project! 😊
