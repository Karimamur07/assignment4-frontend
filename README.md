Karima Mursalimova
IT-2502

Part 1. Basic HTML Forms

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

Task 4. Registration Form

