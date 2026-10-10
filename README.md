Karima Mursalimova
IT-2502

Part 1. Basic HTML Forms

The website for this assignment: https://karimamur07.github.io/assignment4-frontend/

Task 0. Simple Contact Form

A basic contact form built with plain HTML. It contains the following fields:

- Name — text input
- Email — email input
- Message — textarea
- Submit — submit button

Every field has a proper `<label>` element linked to its input via the `for` and `id` attributes, which improves accessibility and allows focusing the input by clicking on the label.

<img width="632" height="469" alt="image" src="https://github.com/user-attachments/assets/9d4a7112-07d3-4f7f-9300-c88d6d2be70a" />

<img width="433" height="268" alt="image" src="https://github.com/user-attachments/assets/d9d5a51e-4707-40a0-a992-9383a33d66aa" />

Task 1. Form with HTML5 Validation

The same contact form, enhanced with built-in HTML5 validation attributes:

- `required` — all fields must be filled in
- `type="email"` — the browser validates the email format automatically
- `minlength` / `maxlength` — length restrictions for text inputs and textarea
- `placeholder` — hint text shown inside empty fields


<img width="476" height="387" alt="image" src="https://github.com/user-attachments/assets/88995df3-f3ad-4835-ab9a-c01d2101d8c1" />

<img width="688" height="298" alt="image" src="https://github.com/user-attachments/assets/4a4cbada-e8d4-4c67-bf53-fda6b18e7353" />

<img width="548" height="241" alt="image" src="https://github.com/user-attachments/assets/e84ad47a-ce2c-49ff-b2a9-91a89f4b048e" />

Browser shows "Please fill out this field" when submitting an empty form.

<img width="543" height="241" alt="image" src="https://github.com/user-attachments/assets/9a68e12e-aec3-49e8-9885-56c435263d81" />

Browser shows an error when the email does not contain an "@" symbol.

<img width="703" height="228" alt="image" src="https://github.com/user-attachments/assets/dbf78f70-1a72-478d-8908-e3b99d83ddf5" />

Browser shows an error when the text is shorter than the `minlength` value.

<img width="566" height="270" alt="image" src="https://github.com/user-attachments/assets/cb220a31-1280-4f65-a5e4-f67216ee0137" />

Part 2. Bootstrap Forms

The website for this assignment: https://karimamur07.github.io/assignment4-frontend/bootstrap-form.html

Task 2. Bootstrap Form Styling

The contact form recreated using **Bootstrap 5.3** classes:

- Bootstrap Grid (`container`, `row`, `col-md-6`, `col-12`) makes the layout responsive
- `card` component groups the form into a clean white panel with a shadow
- `form-label`, `form-control`, `form-text` — Bootstrap styling for inputs and helper text
- `btn btn-primary` — Bootstrap button style
- Placeholders and **helper text** (`form-text`) are added to guide the user

On desktop, Name and Email are displayed side by side; on mobile, they stack vertically — this proves the form is responsive.

Desktop view

<img width="894" height="519" alt="image" src="https://github.com/user-attachments/assets/aafce7f5-2bc3-4ea8-8a3e-cd6097c313a6" />

Mobile (responsive) view

<img width="333" height="610" alt="image" src="https://github.com/user-attachments/assets/831ff506-9feb-466f-aac4-62a4405c00a3" />

Task 3. Bootstrap Validation Styles

The same Bootstrap form, now with client-side validation feedback:

- `needs-validation` + `novalidate` on the `<form>` — disables native browser validation and hands it over to Bootstrap
- `valid-feedback` and `invalid-feedback` blocks under each input
- `was-validated` class is added by JavaScript after the first submit attempt
- HTML5 validation attributes (`required`, `minlength`, `maxlength`) define the rules
- A small JavaScript snippet (based on the official Bootstrap docs) checks `form.checkValidity()` and prevents submission if the form is invalid

<img width="666" height="509" alt="image" src="https://github.com/user-attachments/assets/be4e29dc-aa5c-4844-9d17-0b9134958272" />

<img width="685" height="452" alt="image" src="https://github.com/user-attachments/assets/fdfefe13-9698-4523-be1a-f67df2f3d71e" />

<img width="719" height="377" alt="image" src="https://github.com/user-attachments/assets/b5842b59-e142-49dd-8fc2-f93b577e10b9" />

<img width="681" height="319" alt="image" src="https://github.com/user-attachments/assets/6017a29f-2705-4837-8602-5c8ec92e263f" />

<img width="579" height="349" alt="image" src="https://github.com/user-attachments/assets/4ee710ec-fccf-4bd7-b4e7-f3ff606e86a6" />

Invalid state

After submitting an empty form, all fields turn red and show error messages.

<img width="1060" height="532" alt="image" src="https://github.com/user-attachments/assets/701d274d-27c7-40e0-b76b-85acafbd1c19" />

Valid state

When all fields are filled correctly, fields turn green and show "Looks good!".

<img width="993" height="558" alt="image" src="https://github.com/user-attachments/assets/1fd50b71-3683-4200-8fdd-1a4d1e552d2c" />

Invalid email

Submitting an invalid email shows the email-specific error message.

<img width="448" height="118" alt="image" src="https://github.com/user-attachments/assets/8721cf2f-128c-4b4c-8a20-0a92c3b43c76" />


Part 3. Advanced Form Project

The website for this assignment: https://karimamur07.github.io/assignment4-frontend/registration.html

Task 4. Registration Form

A full registration form built with Bootstrap 5.3, featuring all required field types:

- First Name / Last Name — side by side (`col-md-6`), required with min/max length
- mail — full width, `type="email"` with required validation
- Password / Confirm Password — side by side, `minlength="6"`, with a custom JavaScript check that ensures both passwords match
- Gender — radio buttons (only one can be selected)
- Hobbies — checkboxes (multiple, optional)
- Country — select dropdown with a placeholder option
- Submit / Reset buttons

Features

- Bootstrap Grid (`container`, `row`, `col-md-6`, `col-12`) makes the layout fully responsive
- HTML5 validation (`required`, `minlength`, `maxlength`, `type="email"`)
- Bootstrap feedback (`valid-feedback` / `invalid-feedback`) with `was-validated` class
- Custom JavaScript for:
  - Checking that the two passwords match (`setCustomValidity`)
  - Enforcing that at least one gender radio is selected
  - Manually showing feedback for the radio group (Bootstrap doesn't support radio groups out of the box)
  - Resetting all custom validation state when the Reset button is clicked

<img width="776" height="599" alt="image" src="https://github.com/user-attachments/assets/858a2c05-2b3e-428b-8697-21179684bee8" />

<img width="819" height="499" alt="image" src="https://github.com/user-attachments/assets/ea1e7c06-3c57-43dc-9002-a669773a8911" />

<img width="833" height="519" alt="image" src="https://github.com/user-attachments/assets/cd7e8317-9e73-4fce-839d-28da31af353d" />

<img width="822" height="512" alt="image" src="https://github.com/user-attachments/assets/873c1684-faef-42cf-ba5d-193f97623d15" />

<img width="816" height="490" alt="image" src="https://github.com/user-attachments/assets/7559b007-5edc-469e-9445-bcfe9b95a347" />

<img width="846" height="503" alt="image" src="https://github.com/user-attachments/assets/ec56cbf0-bf62-4293-a309-11e6c6bb301a" />

<img width="811" height="510" alt="image" src="https://github.com/user-attachments/assets/0081c405-0432-4496-b6fd-bfb6ad8c9595" />

<img width="857" height="531" alt="image" src="https://github.com/user-attachments/assets/52cc10c6-ad14-48cb-ad15-ac3c0591e4cb" />

<img width="726" height="360" alt="image" src="https://github.com/user-attachments/assets/efb2a7f1-35cd-4529-8bf5-c80b872fc110" />

<img width="711" height="453" alt="image" src="https://github.com/user-attachments/assets/20bcf6ec-96f8-45c8-a8f9-9ca33894792d" />

<img width="762" height="424" alt="image" src="https://github.com/user-attachments/assets/c26d8bbc-207c-482e-a498-6a51c383391f" />

<img width="757" height="494" alt="image" src="https://github.com/user-attachments/assets/55b8c199-9f5d-48b3-a57e-d02e1bff331a" />

Invalid state (empty form)

<img width="852" height="644" alt="image" src="https://github.com/user-attachments/assets/1579276a-f25d-40c1-99dd-9cc1b006f492" />

Password mismatch

<img width="679" height="106" alt="image" src="https://github.com/user-attachments/assets/c74a4dfd-e400-46fd-9fdf-48d3626a684a" />

Valid state (successful submission)

<img width="761" height="633" alt="image" src="https://github.com/user-attachments/assets/61212c80-0e79-441d-8d2a-953c4c4abc43" />

Mobile view

<img width="333" height="588" alt="image" src="https://github.com/user-attachments/assets/c7af45bc-034c-49d4-9d1d-1bb6492322a3" />


Summary

In this assignment, I built a set of HTML forms progressively, from basic HTML to a fully validated Bootstrap registration form.

- Task 0 — Created a simple contact form with Name, Email, Message, and a Submit button. Each input is properly linked to its `<label>` via the `for`/`id` attributes.
- Task 1 — Added built-in HTML5 validation attributes (`required`, `minlength`, `maxlength`, `placeholder`) and tested the browser's native validation with empty fields, an invalid email, and text that was too short.
- Task 2 — Recreated the contact form with Bootstrap 5.3 using the grid system (`container`, `row`, `col-md-6`), form classes (`form-control`, `form-label`, `form-text`), and a `card` wrapper, making the layout fully responsive.
- Task 3 — Added Bootstrap's client-side validation using `needs-validation`, `novalidate`, `valid-feedback`, and `invalid-feedback`, plus a small JavaScript snippet that applies the `was-validated` class on submit.
- Task 4 — Built a complete registration form with First/Last Name, Email, Password + Confirm Password, Gender (radio), Hobbies (checkboxes), Country (select), and Submit/Reset buttons. Combined Bootstrap Grid, HTML5 validation, and custom JavaScript to check that passwords match and that a gender is selected.

Throughout the assignment, I practiced semantic HTML, responsive layout with Bootstrap, and both native and custom client-side validation. Each task was tested in the browser with valid and invalid data, and the results are documented with screenshots in this README.
