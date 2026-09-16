# Google Groups Alumni Email Matcher v1.6

A browser-based tool that compares a Google Groups listing against an Alumni file and creates a formatted Excel workbook.

## Main features

- Matches the Google Groups `Email address` against content in both Alumni `email` and `AdditionalEmail`.
- Adds First Name and Last Name to the Google Groups output.
- Sorts records by Last Name and then First Name.
- Highlights unmatched records yellow and ambiguous matches red.
- Creates separate worksheets for unmatched, ambiguous, Alumni not in Google Groups, Birth Date records, Date of Death records, and a summary.
- Processes all selected files locally in the browser. The app does not upload the source files.

## Publish with GitHub Pages

1. Create a new GitHub repository, or open an existing repository intended for this app.
2. Upload `index.html`, `.nojekyll`, and this `README.md` file to the root of the repository.
3. Open the repository's **Settings**.
4. Select **Pages** from the left menu.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select the `main` branch and the `/ (root)` folder, then click **Save**.
7. GitHub will display the public website address after deployment finishes.

For a user named `munnster44` and a repository named `google-groups-alumni-email-matcher`, the expected address would be:

`https://munnster44.github.io/google-groups-alumni-email-matcher/`

## Using the app

1. Open the published GitHub Pages address.
2. Select the Google Groups Excel or CSV file.
3. Select the Alumni Excel or CSV file.
4. Select the correct worksheet for each workbook if necessary.
5. Click **Match Email Addresses**.
6. Review the summary and preview.
7. Click **Export Excel Workbook**.

## Required columns

Google Groups file:

- `Email address`

Alumni file:

- `FirstName`
- `LastName`
- `email`
- `AdditionalEmail`

The optional `Birth Date` and `Date of Death` columns are used to create their respective output worksheets.

## Internet connection

The published app uses SheetJS and ExcelJS from jsDelivr to read and create Excel workbooks. An internet connection is required when opening the app so those libraries can load.

## Copyright

© 2026 Glen Carruthers

