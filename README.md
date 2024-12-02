# Base Style Guidelines

## Introduction

This document outlines the foundational guidelines for styling a web application. It serves as a technical guide, detailing how styling should be implemented consistently. While not exhaustive, it provides a solid starting point for development. These guidelines prioritize uniform styling and usage, without prescribing specific components to include.

## Good to Know

- **Consistency is key**: Adhering to these guidelines ensures a cohesive and maintainable codebase.
- **Semantic and accessible HTML**: Use semantic elements as the foundation for styling to enhance accessibility.
- **Avoid hardcoding values**: Leverage design tokens and variables to maintain flexibility and scalability.

## Colors

At the start of a project, define a comprehensive color palette. For this guideline, colors are derived from an alerting system that includes the following types:  

- **`success`**: Indicates successful actions or confirmations.  
- **`info`**: Provides contextual information.  
- **`warning`**: Warns users of potential issues.  
- **`error`**: Alerts users to errors or critical issues.  
- **`default`**: Represents neutral actions or states.  

These alert types form the foundation of the color palette and are applied to buttons, links, backgrounds, text, and other UI elements. Consistent use of these colors across the application ensures a unified and predictable user experience.

## Sizes

All sizes are calculated relative to the base font size. The defined size categories are:  
- **`smaller`**  
- **`small`**  
- **`default`**  
- **`big`**  
- **`bigger`**  

These sizes are applied universally across the application. Key starting points include `font-size` and `line-height`, which serve as the basis for calculating all other dimensions. Use relative units such as `em`, `rem`, or percentages for scalability and responsiveness.

## Interactions

Interactive elements should support the following states:  
- **`hover`**: When a user hovers over an element.  
- **`focus`**: When an element is selected or in focus.  
- **`active`**: When an element is being interacted with.  
- **`readonly`**: When an element is not editable.  
- **`required`**: When an element is mandatory.  
- **`disabled`**: When an element is not available for interaction or selection.  

### Usage in Interactions

#### Colors  
- **`success`**: Used for positive actions or confirmations.  
- **`default`**: Used for neutral actions like resets or cancellations.  
- **`info`, `warning`, `error`**: Used for context-specific messages or actions.  

#### States  
Ensure interactions are applied consistently across the application. For instance, a `hover` state should be present on all interactive elements, not just buttons. Certain states, such as `disabled`, may omit unnecessary interactions like `hover`.

## How to Use

### Elements Styled as Buttons

Not all HTML elements behave consistently out of the box. For example, `button` and `a` elements often require additional styling to align their appearance and behavior.  

**Guidelines for button like elements:**  
- Add consistent **padding**, **margin**, **border size**, and **border radius**.  
- Define **background color**, **text color**, **border color**, and **shadow**.  
- Ensure all states are supported: `hover`, `focus`, `active`, `disabled`, `readonly`.  
