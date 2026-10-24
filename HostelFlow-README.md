# HostelFlow | Hostel Allotment System

A responsive, presentation-ready hostel allotment website based on the Python project idea. Built with plain HTML, CSS and JavaScript, so there is no build step or package installation.

## Features
- Dashboard with hostel blocks, room counts, allotments and occupancy
- Student allotment form with fresher/non-fresher classification
- Matches gender, student category, room capacity and AC/NAC preference
- Inventory is decremented after a successful allotment
- Duplicate registration-number protection
- Searchable student records
- Hostel block management
- Export data as JSON and student records as CSV
- Responsive layout for desktop, tablet and mobile
- Browser local storage, so demo data remains after refresh on the same browser

## Run it locally
1. Download or clone this repository.
2. Open `index.html` in a modern browser.
3. Explore the sample data, try a new allotment, or add a block under **Manage inventory**.

No Python, Node.js, or other installation is required.

## Publish with GitHub Pages
1. Sign in to GitHub and create a **new public repository**, for example `hostel-allotment-system`.
2. Extract this project ZIP on your computer.
3. Upload `index.html` and `README.md` to the **root** of that repository. (Do not upload only the ZIP file.)
4. Open the repository's **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select branch `main` and folder `/(root)`, then click **Save**.
7. Wait a minute or two and refresh the Pages screen. GitHub will show the published website URL, usually:
   `https://YOUR-USERNAME.github.io/hostel-allotment-system/`
8. Open that URL and test the form. You can present that link to your class.

If the page does not appear, confirm `index.html` is in the repository root and that Pages is enabled for the correct branch.

## Suggested presentation demo
1. Show the dashboard and explain the room inventory.
2. Open **Allot a hostel**.
3. Enter a student name, a registration number beginning with the current year (e.g. `26BEE0193` for academic year 2026), gender, academic year, room capacity and AC/NAC preference.
4. Submit and show the successful allotment result.
5. Open **Hostel blocks** to show inventory counts.
6. Open **Student records** to show the new record.
7. Use **Manage inventory** to export JSON/CSV.

## Important limitations
- This is a **front-end school presentation demo**, not a production hostel-management system.
- Records are stored in the current browser's `localStorage`. They are not shared between computers or users, and clearing browser storage removes them.
- The default data is illustrative sample data.
- Room inventory is modeled as **number of rooms** per capacity and type. When a room is allotted, one room of that configuration is removed from available inventory. This is more consistent than treating a room count as a count of individual beds.
- The fresher rule assumes the first two digits of the registration number are the admission year, matching the logic in the supplied Python code.
- Do not put real student personal information into a public demo. For a real deployment, add authentication, a server/database, input validation and appropriate privacy controls.
