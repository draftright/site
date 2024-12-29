---
layout: post
title: "Bootstrap Customization with Sass - Part 5"
subtitle: Day 5
categories: Learning
author: "Dilip Rout"
meta: ""
tags: bootstrap learning
top: 
excerpt_image: https://getbootstrap.com/docs/5.3/assets/img/bootstrap-icons.png
---
![banner](https://getbootstrap.com/docs/5.3/assets/img/bootstrap-icons.png)


**Objective**

- Learn to customize Bootstrap using Sass.
- Modify key variables like colors, breakpoints, and spacing.
- Compile a custom CSS file from your Sass changes to create a custom Bootstrap theme.

**1\. Install Sass**

**A. Verify Node.js and npm**

Make sure you have Node.js and npm installed, as Sass uses npm for installation.

bash

node -v

npm -v

If not installed, download from [Node.js](https://nodejs.org/).

**B. Install Sass**

Install Sass globally using npm:

bash

npm install -g sass

Or, for a project-specific installation:

bash

npm install sass --save-dev

Verify installation:

bash

sass --version

**2\. Bootstrap Source Files**

**A. Download Bootstrap Source**

Download the Bootstrap source files, which include the Sass files, from [Bootstrap’s GitHub](https://github.com/twbs/bootstrap) or via npm:

bash

npm install bootstrap

**B. Bootstrap Sass File Structure**

In the scss directory, you’ll find:

- \_variables.scss: Contains all the customizable default variables.
- \_mixins.scss: Contains reusable styles.
- bootstrap.scss: The main file that imports all other Sass partials.

**3\. Modify Default Variables**

Bootstrap variables are defined in \_variables.scss. You can override them by creating your own \_custom.scss file before importing Bootstrap.

**A. Customizing Colors**

Example: Changing the primary color.

scss

// \_custom.scss

$primary: #ff6347; // Custom primary color

@import "bootstrap/scss/bootstrap"; // Import Bootstrap after overriding variables

Compile your Sass to CSS:

bash

sass \_custom.scss custom.css

**B. Customizing Breakpoints**

Modify breakpoints to suit your design:

scss

$grid-breakpoints: (

xs: 0,

sm: 480px,

md: 768px,

lg: 1024px,

xl: 1280px

);

@import "bootstrap/scss/bootstrap";

**C. Customizing Spacing**

Bootstrap uses $spacer for spacing utilities. Customize it to modify all spacing values.

scss

$spacer: 2rem; // Default is 1rem

@import "bootstrap/scss/bootstrap";

**4\. Build a Custom Bootstrap Theme**

**A. Setting Up Your Project Structure**

1. Create the following folders:

bash

/project

/scss

\_custom.scss

/css

custom.css

1. Place your \_custom.scss and Bootstrap files in the /scss folder.

**B. Compiling Sass**

Use Sass to compile your custom theme:

bash

sass scss/\_custom.scss css/custom.css

**C. Integrating the Custom Theme**

Link your custom CSS file in your HTML:

html

&lt;link rel="stylesheet" href="css/custom.css"&gt;

**5\. Advanced Sass Features**

**A. Using Mixins**

Mixins allow you to reuse common patterns. Bootstrap provides several useful mixins.  
Example: Using the breakpoint mixin:

scss

@include media-breakpoint-up(md) {

body {

background-color: lightblue;

}

}

**B. Extending Styles**

Use Sass's @extend feature to inherit styles:

scss

.button {

@extend .btn-primary;

background-color: #333;

}

**6\. Practice: Build a Custom Theme**

1. **Customize Default Styles**:
    - Change the primary and secondary colors.
    - Modify the button sizes and border radius.
2. **Create a Custom Navbar**:
    - Update the navbar background and font colors.
3. **Compile and Test**:
    - Compile your custom Sass into CSS and link it to a sample HTML file.

**7\. Summary and Next Steps**

**What You Learned**

- Installed Sass and Bootstrap source files.
- Overrode Bootstrap’s default variables.
- Created and compiled a custom theme.

**Next Steps**

- Experiment with more variables in \_variables.scss.
- Explore Bootstrap’s mixins and utility generators.
- Build a complete project with your custom Bootstrap theme.

Let me know if you’d like help setting up your project or troubleshooting Sass compilation! 😊
