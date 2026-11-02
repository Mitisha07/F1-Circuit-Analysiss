# F1 Circuit Analytics Website

## Files
- `index.html` — website structure
- `style.css` — responsive dark F1-inspired design
- `app.js` — charts, map, filters, Excel import, scenario answers and story slides

## Run in VS Code
1. Extract this ZIP file.
2. Open the extracted `f1_circuit_analysis_website` folder in VS Code.
3. Install the **Live Server** extension (Extensions icon on the left, search "Live Server").
4. Right-click `index.html` and choose **Open with Live Server**.
5. Your browser will open the website.

An internet connection is required for the Chart.js, SheetJS, Leaflet, map tiles and Google Fonts CDN libraries.

## Load your Excel dataset
1. Open the website.
2. Click **Upload Excel / CSV** in the top-right.
3. Select your `.xlsx`, `.xls` or `.csv` file.
4. The website reads the first worksheet and updates the charts, map, table and scenario answers.

The first worksheet should have a header row. Column names can vary, but these are recognized:
- Circuit Name (or Circuit / Name)
- Country
- City
- Laps (or Lap Count)
- Lap Km (or Lap Distance / Circuit Length)
- Altitude M (or Altitude / Elevation)
- Direction
- Type (or Circuit Type)
- Latitude (or Lat)
- Longitude (or Lon / Long)

If latitude/longitude are missing, the map will not show markers for those records. Missing numerical values will show as blank or be excluded from the relevant calculation.

## Publish online with GitHub Pages
1. Create or sign in to a GitHub account.
2. Create a new public repository, for example `f1-circuit-analytics`.
3. Upload `index.html`, `style.css` and `app.js` to the repository root.
4. Open repository **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select branch `main` and folder `/ (root)`, then click **Save**.
7. Wait for GitHub Pages to publish. Open the website URL shown in the Pages section.

## Important notes
- The included records are demo/sample data so the site can be previewed before you upload your Excel file. Replace them by uploading your own file.
- Scenario answers are calculated from the currently filtered rows. Verify them against your source data before submitting.
- This is a static website. Uploaded Excel data is processed locally in the visitor's browser and is not automatically stored online or shared with other visitors.
- Do not describe demo values as official current-season F1 statistics.
