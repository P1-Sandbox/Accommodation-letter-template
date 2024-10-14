# Accommodation Letter Template

This repository contains a template for generating academic accommodation letters used by the California Community Colleges Disability Services. The template integrates with **QuickBase**, allowing dynamic retrieval and display of student accommodations from QuickBase tables. This helps ensure compliance with Section 504 of the Rehabilitation Act and the Americans with Disabilities Act (ADA) by outlining the accommodations authorized for students.

![CCC Logo](https://amacsam.quickbase.com/up/bnuuc9j4q/g/rb/eg/va/1200px-California_Community_Colleges_System_logo.svg.png)

## Table of Contents

- [Overview](#overview)
- [Usage](#usage)
- [File Structure](#file-structure)
- [Customization](#customization)
- [License](#license)

## Overview

The `Accommodation Notification` template is used to notify instructors of a student's authorized accommodations. These accommodations help reduce the impact of a student's disability in an academic setting. All information regarding a student's disability is confidential, and the template is designed to provide instructors with the necessary details without disclosing the specifics of the disability.

This template works with **QuickBase** by fetching accommodation data from a specific QuickBase table. The dynamic data is displayed within the template using an API call.

## Usage

This template uses HTML, CSS, and JavaScript to generate and display accommodations in a user-friendly format. The template includes:
- Integration with **QuickBase** through the `API_GenResultsTable`, which retrieves student accommodations based on their **Student ID**.
- Functionality to finalize the letter by selecting accommodations and removing unchecked options.
- The option to hide additional comments if they are not filled out.

### Example of Key Fields:
- **Student ID**: 123456
- **Student Name**: John Doe
- **Authorized Accommodations**: Displayed in the dynamically generated table.

### Instructions for Use:
1. Replace placeholders such as `~Student ID~`, `~Name~`, and `~Additional Comments (text)~` with actual values.
2. Ensure that the script connects to your QuickBase database by specifying the correct **accommodationTable** and field IDs.
3. Use the "Finish" button to finalize the accommodation selections.
4. The finalized letter can then be shared with the instructor.

## File Structure

- `CCC Accommodation Letter.html`: The main template file containing the structure for the accommodation notification letter.
- Inline CSS for styling the template, including headers, tables, and other layout elements.
- JavaScript that interacts with **QuickBase** using `API_GenResultsTable` to dynamically load the student’s accommodations into the HTML table.

## Customization

You can customize the following elements to meet your specific needs:
- **Student Information**: Modify the JavaScript to input specific student IDs or names and ensure the QuickBase integration works with your database.
- **Accommodations Table**: Accommodations are fetched from a QuickBase table and displayed in the letter. You can adjust the logic to suit your own database structure or modify the table's content and style.
- **Additional Comments Section**: You can hide this section based on the presence of comments using the JavaScript provided.

## License

This project is licensed under the MIT License. You are free to use, modify, and distribute this template for educational and administrative purposes.
