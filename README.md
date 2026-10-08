# custom-css-framework-26

A custom CSS framework built as a team project using Sass.

## Project Progress

### Member 1 - Completed

Ufuk completed Requirements 1 and 2.

- Created the basic Sass folder structure.
- Created `_variables.scss` as a Sass partial.
- Created `main.scss`.
- Connected the variables partial using `@use`.
- Added shared Sass variables for:
  - Primary and secondary colours
  - Text and background colours
  - Border colour
  - Border width and radius
  - Font sizes
  - Font weights
  - Spacing
- Added `!default` to the variables so they can be customized later.


### Member 2 - Completed

Peter completed Requirements 3 and 5.

- Created `_theme.scss`.
- Added custom styles for standard HTML elements including:
  - Headings
  - Paragraphs
  - Links
  - Lists
  - Buttons
  - Forms
  - Inputs
  - Textareas
  - Select elements
  - Tables
  - Images
  - Blockquotes
- Used the shared Sass variables from `_variables.scss`.
- Kept colours, spacing, borders, and typography consistent across the framework.
- Connected the theme partial to `main.scss`.

### Member 3 - Completed

Mehdi completed Requirement 4.

- Created `_utilities.scss`.
- Added reusable utility classes for:
  - Text colours
  - Background colours
  - Font sizes
  - Font weights
  - Margins
  - Padding
  - Borders
  - Rounded corners
- Used the shared Sass variables to keep the utilities consistent with the framework theme.
- Connected the utilities partial to `main.scss`.

### Member 4 - Completed

Ahcene completed Requirements 6 and 7.

- Compiled the Sass framework into CSS.
- Added the compiled `css/main.css` file to the project.
- Added installation instructions to the README.
- Added usage examples for the framework and utility classes.
- Added customization instructions for Sass variables.
- Added instructions for recompiling the framework after making Sass changes.


## Current Sass Structure

```text
scss/
├── _theme.scss
├── _utilities.scss
├── _variables.scss
└── main.scss

css/
├── main.css
└── main.css.map
```

## Installation

Clone or download this repository.

To use the compiled framework, link the CSS file in the `<head>` of your HTML:

```html
<link rel="stylesheet" href="css/main.css">
```


## Usage

The framework automatically styles common HTML elements such as:

- Headings
- Paragraphs
- Links
- Lists
- Buttons
- Forms
- Inputs
- Tables
- Images
- Blockquotes

The framework also provides reusable utility classes.

### Colors

```html
<p class="text-primary">Primary text</p>
<p class="text-secondary">Secondary text</p>

<div class="bg-primary">Primary background</div>
<div class="bg-secondary">Secondary background</div>
```

### Font Sizes

```html
<p class="fs-small">Small text</p>
<p class="fs-base">Normal text</p>
<p class="fs-large">Large text</p>
```

### Font Weight

```html
<p class="fw-normal">Normal text</p>
<p class="fw-bold">Bold text</p>
```

### Margin

```html
<div class="m-small">Small margin</div>
<div class="m-medium">Medium margin</div>
<div class="m-large">Large margin</div>
```

### Padding

```html
<div class="p-small">Small padding</div>
<div class="p-medium">Medium padding</div>
<div class="p-large">Large padding</div>
```

### Borders

```html
<div class="border">Border</div>
<div class="rounded">Rounded corners</div>
```

## Customization

The framework can be customized by changing the Sass variables inside:

```text
scss/_variables.scss
```

For example:

```scss
$primary: #7c3aed !default;
$secondary: #111827 !default;
$border-radius: 8px !default;
$font-size-base: 1rem !default;
$spacing-medium: 1rem !default;
```

These variables can be changed to customize the colours, typography, spacing, and borders used throughout the framework.

After changing the Sass files, compile the framework again using:

```bash
npx sass scss/main.scss css/main.css
```

The compiled CSS file is located at:

```text
css/main.css
```