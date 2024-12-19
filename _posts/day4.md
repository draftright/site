Day 4

# Day 4: Forms and Tables

**Objective:** Learn to create responsive forms and tables.

- **Tasks:**
  - Explore form controls:
    - Input fields, checkboxes, radios, and dropdowns.
    - Validation states and feedback messages.
  - Build a form with a grid layout.
  - Style tables:
    - Basic table styles (.table, .table-striped, .table-bordered).
    - Responsive tables using .table-responsive.

**Day 4: Forms and Input Components**

Today’s focus is on understanding and building responsive, styled forms using Bootstrap. Forms are essential in web applications, and Bootstrap provides tools to create and customize them easily.

**Objective**

- Learn to create accessible and visually appealing forms using Bootstrap.
- Use Bootstrap utilities to style forms effectively.

**1\. Form Basics**

**A. Creating a Simple Form**

Bootstrap uses the &lt;form&gt; element with classes to style form inputs, labels, and buttons.  
Example:

html

&lt;form&gt;

&lt;div class="mb-3"&gt;

&lt;label for="exampleInputEmail1" class="form-label"&gt;Email address&lt;/label&gt;

&lt;input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp"&gt;

&lt;div id="emailHelp" class="form-text"&gt;We'll never share your email with anyone else.&lt;/div&gt;

&lt;/div&gt;

&lt;div class="mb-3"&gt;

&lt;label for="exampleInputPassword1" class="form-label"&gt;Password&lt;/label&gt;

&lt;input type="password" class="form-control" id="exampleInputPassword1"&gt;

&lt;/div&gt;

&lt;button type="submit" class="btn btn-primary"&gt;Submit&lt;/button&gt;

&lt;/form&gt;

**B. Inline Forms**

Use .form-inline to create compact, inline forms.  
Example:

html

&lt;form class="d-flex"&gt;

&lt;input class="form-control me-2" type="search" placeholder="Search" aria-label="Search"&gt;

&lt;button class="btn btn-outline-success" type="submit"&gt;Search&lt;/button&gt;

&lt;/form&gt;

**2\. Input Types and States**

**A. Different Input Types**

Bootstrap supports a variety of input types such as text, email, password, number, etc.  
Example:

html

&lt;div class="mb-3"&gt;

&lt;label for="inputText" class="form-label"&gt;Text Input&lt;/label&gt;

&lt;input type="text" class="form-control" id="inputText"&gt;

&lt;/div&gt;

&lt;div class="mb-3"&gt;

&lt;label for="inputDate" class="form-label"&gt;Date Input&lt;/label&gt;

&lt;input type="date" class="form-control" id="inputDate"&gt;

&lt;/div&gt;

&lt;div class="mb-3"&gt;

&lt;label for="inputFile" class="form-label"&gt;File Input&lt;/label&gt;

&lt;input type="file" class="form-control" id="inputFile"&gt;

&lt;/div&gt;

**B. Disabled and Read-Only Inputs**

- **Disabled**: Add disabled attribute or .disabled class.
- **Read-Only**: Use readonly attribute.  
    Example:

html

&lt;input type="text" class="form-control" value="Read-only" readonly&gt;

&lt;input type="text" class="form-control" value="Disabled Input" disabled&gt;

**3\. Form Layouts**

**A. Stacked (Default) Layout**

Form elements stack vertically by default.

**B. Horizontal Forms**

Add .row and column classes to create a horizontal layout.  
Example:

html

&lt;form&gt;

&lt;div class="row mb-3"&gt;

&lt;label for="inputName" class="col-sm-2 col-form-label"&gt;Name&lt;/label&gt;

&lt;div class="col-sm-10"&gt;

&lt;input type="text" class="form-control" id="inputName"&gt;

&lt;/div&gt;

&lt;/div&gt;

&lt;div class="row mb-3"&gt;

&lt;label for="inputEmail" class="col-sm-2 col-form-label"&gt;Email&lt;/label&gt;

&lt;div class="col-sm-10"&gt;

&lt;input type="email" class="form-control" id="inputEmail"&gt;

&lt;/div&gt;

&lt;/div&gt;

&lt;button type="submit" class="btn btn-primary"&gt;Submit&lt;/button&gt;

&lt;/form&gt;

**4\. Form Controls**

**A. Checkboxes and Radios**

Bootstrap provides styled checkboxes and radio buttons.  
Example:

html

&lt;div class="form-check"&gt;

&lt;input class="form-check-input" type="checkbox" value="" id="flexCheckDefault"&gt;

&lt;label class="form-check-label" for="flexCheckDefault"&gt;Default checkbox&lt;/label&gt;

&lt;/div&gt;

&lt;div class="form-check"&gt;

&lt;input class="form-check-input" type="radio" name="flexRadioDefault" id="flexRadio1"&gt;

&lt;label class="form-check-label" for="flexRadio1"&gt;Radio 1&lt;/label&gt;

&lt;/div&gt;

&lt;div class="form-check"&gt;

&lt;input class="form-check-input" type="radio" name="flexRadioDefault" id="flexRadio2"&gt;

&lt;label class="form-check-label" for="flexRadio2"&gt;Radio 2&lt;/label&gt;

&lt;/div&gt;

**B. Switches**

Switches are styled checkboxes.  
Example:

html

&lt;div class="form-check form-switch"&gt;

&lt;input class="form-check-input" type="checkbox" id="flexSwitchCheckDefault"&gt;

&lt;label class="form-check-label" for="flexSwitchCheckDefault"&gt;Default switch checkbox&lt;/label&gt;

&lt;/div&gt;

**C. Input Groups**

Input groups add icons, text, or buttons next to inputs.  
Example:

html

&lt;div class="input-group mb-3"&gt;

&lt;span class="input-group-text"&gt;@&lt;/span&gt;

&lt;input type="text" class="form-control" placeholder="Username"&gt;

&lt;/div&gt;

&lt;div class="input-group"&gt;

&lt;input type="text" class="form-control" placeholder="Recipient's username"&gt;

&lt;button class="btn btn-primary" type="button"&gt;Send&lt;/button&gt;

&lt;/div&gt;

**5\. Validation and Feedback**

Bootstrap supports form validation with feedback messages.

Example:

html

&lt;form class="needs-validation" novalidate&gt;

&lt;div class="mb-3"&gt;

&lt;label for="validationCustom01" class="form-label"&gt;First name&lt;/label&gt;

&lt;input type="text" class="form-control" id="validationCustom01" required&gt;

&lt;div class="valid-feedback"&gt;Looks good!&lt;/div&gt;

&lt;div class="invalid-feedback"&gt;Please provide a valid first name.&lt;/div&gt;

&lt;/div&gt;

&lt;button class="btn btn-primary" type="submit"&gt;Submit&lt;/button&gt;

&lt;/form&gt;

**Tip:** Add was-validated class to the form after submission for validation styling.

**6\. Utility Classes for Forms**

- **Spacing:** Use .mb-3, .mt-4, etc., to manage margins.
- **Alignment:** Use .text-center or .align-items-center for aligning form elements.
- **Responsive Design:** Use grid breakpoints to customize form layouts for different screen sizes.

**7\. Summary and Practice**

**What You Learned**

- Created basic and advanced form layouts.
- Styled inputs, checkboxes, radios, switches, and input groups.
- Implemented validation and feedback mechanisms.

**Practice Tasks**

1. Create a contact form with the following:
    - Name, Email, and Message fields.
    - A checkbox for "Subscribe to Newsletter."
    - A "Submit" button.
2. Build a login form with the following:
    - Email and Password inputs.
    - A "Remember Me" checkbox.
    - A "Forgot Password?" link.
3. Experiment with horizontal and inline form layouts.

Let me know if you need assistance with the practice tasks or more examples! 😊
