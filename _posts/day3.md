Day 3

# Day 3: Components

**Objective:** Get familiar with Bootstrap's components.

- **Tasks:**
  - Practice using common components:
    - Buttons (.btn, .btn-primary, etc.).
    - Navigation bar (&lt;nav&gt;, .navbar).
    - Cards and carousels.
    - Modals.
  - Customize components using utility classes.

Here’s a detailed **Day 3: Bootstrap Components** course. Today, you'll explore the versatile pre-built components in Bootstrap and learn how to customize them using utility classes.

**Objective**

- Understand and practice using Bootstrap's common components.
- Customize components using Bootstrap utility classes to adapt them to different use cases.

**1\. Buttons**

Bootstrap provides a wide range of pre-styled buttons with various colors, sizes, and states.

**A. Button Basics**

Buttons are styled using the .btn class and color modifier classes.

Example:

html

&lt;button class="btn btn-primary"&gt;Primary Button&lt;/button&gt;

&lt;button class="btn btn-secondary"&gt;Secondary Button&lt;/button&gt;

&lt;button class="btn btn-success"&gt;Success Button&lt;/button&gt;

&lt;button class="btn btn-danger"&gt;Danger Button&lt;/button&gt;

&lt;button class="btn btn-warning"&gt;Warning Button&lt;/button&gt;

&lt;button class="btn btn-info"&gt;Info Button&lt;/button&gt;

&lt;button class="btn btn-light"&gt;Light Button&lt;/button&gt;

&lt;button class="btn btn-dark"&gt;Dark Button&lt;/button&gt;

**B. Button Sizes**

Use .btn-sm for small buttons and .btn-lg for large buttons.

Example:

html

&lt;button class="btn btn-primary btn-sm"&gt;Small Button&lt;/button&gt;

&lt;button class="btn btn-primary"&gt;Default Button&lt;/button&gt;

&lt;button class="btn btn-primary btn-lg"&gt;Large Button&lt;/button&gt;

**C. Button States**

- Disabled buttons: Add the disabled attribute or .disabled class.
- Active buttons: Add the .active class.

Example:

html

&lt;button class="btn btn-primary active"&gt;Active Button&lt;/button&gt;

&lt;button class="btn btn-secondary disabled" disabled&gt;Disabled Button&lt;/button&gt;

**2\. Navigation Bar**

The Navbar is a responsive header component used for navigation.

**A. Basic Navbar**

Create a simple navigation bar with links:

html

&lt;nav class="navbar navbar-expand-lg navbar-light bg-light"&gt;

&lt;a class="navbar-brand" href="#"&gt;Brand&lt;/a&gt;

&lt;button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"&gt;

&lt;span class="navbar-toggler-icon"&gt;&lt;/span&gt;

&lt;/button&gt;

&lt;div class="collapse navbar-collapse" id="navbarNav"&gt;

&lt;ul class="navbar-nav"&gt;

&lt;li class="nav-item"&gt;&lt;a class="nav-link active" href="#"&gt;Home&lt;/a&gt;&lt;/li&gt;

&lt;li class="nav-item"&gt;&lt;a class="nav-link" href="#"&gt;About&lt;/a&gt;&lt;/li&gt;

&lt;li class="nav-item"&gt;&lt;a class="nav-link" href="#"&gt;Contact&lt;/a&gt;&lt;/li&gt;

&lt;/ul&gt;

&lt;/div&gt;

&lt;/nav&gt;

**B. Customizing Navbars**

Use utility classes to change background color, text color, or alignment.

html

&lt;nav class="navbar navbar-dark bg-dark"&gt;

&lt;a class="navbar-brand" href="#"&gt;Dark Navbar&lt;/a&gt;

&lt;/nav&gt;

**3\. Cards**

Cards are flexible and extensible content containers.

**A. Basic Card**

Create a card with a title, text, and button.

html

&lt;div class="card" style="width: 18rem;"&gt;

&lt;img src="<https://via.placeholder.com/150>" class="card-img-top" alt="Placeholder"&gt;

&lt;div class="card-body"&gt;

&lt;h5 class="card-title"&gt;Card Title&lt;/h5&gt;

&lt;p class="card-text"&gt;This is some example text inside a card.&lt;/p&gt;

&lt;a href="#" class="btn btn-primary"&gt;Learn More&lt;/a&gt;

&lt;/div&gt;

&lt;/div&gt;

**B. Grouped Cards**

Cards can be grouped together using .card-group.

html

&lt;div class="card-group"&gt;

&lt;div class="card"&gt;

&lt;img src="<https://via.placeholder.com/150>" class="card-img-top" alt="Placeholder"&gt;

&lt;div class="card-body"&gt;

&lt;h5 class="card-title"&gt;Card 1&lt;/h5&gt;

&lt;p class="card-text"&gt;Some quick example text.&lt;/p&gt;

&lt;/div&gt;

&lt;/div&gt;

&lt;div class="card"&gt;

&lt;img src="<https://via.placeholder.com/150>" class="card-img-top" alt="Placeholder"&gt;

&lt;div class="card-body"&gt;

&lt;h5 class="card-title"&gt;Card 2&lt;/h5&gt;

&lt;p class="card-text"&gt;Some quick example text.&lt;/p&gt;

&lt;/div&gt;

&lt;/div&gt;

&lt;/div&gt;

**4\. Carousels**

Carousels are image sliders used for showcasing content.

**A. Basic Carousel**

html

&lt;div id="carouselExampleIndicators" class="carousel slide" data-bs-ride="carousel"&gt;

&lt;div class="carousel-indicators"&gt;

&lt;button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active"&gt;&lt;/button&gt;

&lt;button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1"&gt;&lt;/button&gt;

&lt;button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2"&gt;&lt;/button&gt;

&lt;/div&gt;

&lt;div class="carousel-inner"&gt;

&lt;div class="carousel-item active"&gt;

&lt;img src="<https://via.placeholder.com/800x400>" class="d-block w-100" alt="Slide 1"&gt;

&lt;/div&gt;

&lt;div class="carousel-item"&gt;

&lt;img src="<https://via.placeholder.com/800x400>" class="d-block w-100" alt="Slide 2"&gt;

&lt;/div&gt;

&lt;div class="carousel-item"&gt;

&lt;img src="<https://via.placeholder.com/800x400>" class="d-block w-100" alt="Slide 3"&gt;

&lt;/div&gt;

&lt;/div&gt;

&lt;button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev"&gt;

&lt;span class="carousel-control-prev-icon" aria-hidden="true"&gt;&lt;/span&gt;

&lt;/button&gt;

&lt;button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next"&gt;

&lt;span class="carousel-control-next-icon" aria-hidden="true"&gt;&lt;/span&gt;

&lt;/button&gt;

&lt;/div&gt;

**5\. Modals**

Modals are dialog boxes or overlays.

**A. Basic Modal**

html

&lt;!-- Trigger Button --&gt;

&lt;button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModal"&gt;

Launch Modal

&lt;/button&gt;

&lt;!-- Modal --&gt;

&lt;div class="modal fade" id="exampleModal" tabindex="-1"&gt;

&lt;div class="modal-dialog"&gt;

&lt;div class="modal-content"&gt;

&lt;div class="modal-header"&gt;

&lt;h5 class="modal-title"&gt;Modal Title&lt;/h5&gt;

&lt;button type="button" class="btn-close" data-bs-dismiss="modal"&gt;&lt;/button&gt;

&lt;/div&gt;

&lt;div class="modal-body"&gt;

This is a modal body.

&lt;/div&gt;

&lt;div class="modal-footer"&gt;

&lt;button type="button" class="btn btn-secondary" data-bs-dismiss="modal"&gt;Close&lt;/button&gt;

&lt;button type="button" class="btn btn-primary"&gt;Save Changes&lt;/button&gt;

&lt;/div&gt;

&lt;/div&gt;

&lt;/div&gt;

&lt;/div&gt;

**6\. Customizing Components with Utility Classes**

Bootstrap utility classes allow you to modify components without writing custom CSS.

**Examples**

- Change a button's color: class="btn btn-success"
- Add margin to a card: class="card m-4"
- Change padding inside a modal: class="modal-body p-5"

**7\. Summary and Practice**

**What You Learned**

- Basics of Bootstrap components like buttons, navbars, cards, carousels, and modals.
- How to customize components with utility classes.

**Practice Tasks**

1. Create a navigation bar with a brand logo, links, and a toggle menu for smaller screens.
2. Build a card deck showcasing three products with titles, descriptions, and "Buy Now" buttons.
3. Add a carousel to your webpage with at least three images.
4. Add a modal that displays when a button is clicked.

Let me know if you'd like more examples or assistance! 😊
