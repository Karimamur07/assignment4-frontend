Karima Mursalimova
IT-2502

Part 1. Basic HTML Forms

Task 0. Simple Contact Form

A basic contact form built with plain HTML. It contains the following fields:

- **Name** — text input
- **Email** — email input
- **Message** — textarea
- **Submit** — submit button

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

