# Food Recipe – React Application (Corrected)

## Run the project
1. Extract this ZIP.
2. Open the `FoodRecipe-React-Fixed` folder in VS Code.
3. Open Terminal in the same folder (the folder containing `package.json`).
4. Run:
   ```bash
   npm install
   npm run dev
   ```
5. Open the Local URL printed by Vite (usually `http://localhost:5173`).

Do not open the project using Live Server. It is a Vite + React application.

## Main pages
- `/` – Public Home page (opens first; does not force login)
- `/login` – User login
- `/signup` – User registration
- `/recipes` – Recipe listing
- `/cuisines` – Cuisine listing
- `/admin/login` and `/admin/signup` – Chef/Admin access
- `/super-admin/login` – Super Admin access
- `/super-admin/dashboard` – Super Admin control panel

## Super Admin demo login
Email: `manikantamani8034@kluniversity.in`
Password: `superadmin123`

## Account behavior
- User signup stores each account in `users`; after signup, the app opens the login page with the new email prefilled.
- Admin signup stores each admin in `admins`.
- Super Admin can view and delete registered users and admins.
- Deleting an account also removes its active session and login history in this browser.
- User, Admin and Super Admin sessions have separate keys.

## Important limitation
This version uses browser Local Storage, so accounts and dashboard data are available only in the same browser profile on the same device. It is a front-end demonstration, not secure multi-device authentication. Passwords are not automatically displayed or prefilled on the login page for security; only the email is remembered.
