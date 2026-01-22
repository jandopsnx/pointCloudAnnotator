# Classifications Example

This example demonstrates Potree's classification visualization features for point clouds, allowing users to switch between different classification schemes (e.g., default, tree-based, or random colors). It also includes interactive annotation tools for marking points in 3D space.

## About — Technical choices

This example uses semantic HTML and vanilla JavaScript for structure and interactivity, and Potree (built on Three.js) for WebGL point-cloud rendering. Annotations persist client-side via `localStorage`; jQuery is used only sparingly for small UI enhancements. The goal is a lightweight, easy-to-embed example with minimal external dependencies.

## Features

- **Classification Schemes**: Buttons to apply different color schemes to point classifications.
- **Annotations**: Click on the point cloud to add annotations with text descriptions. Annotations can be saved, loaded, exported, or imported via JSON files.
- **Persistence**: Annotations are stored in localStorage for session persistence.

## How to Run

1. **Prerequisites**:
   - Install [Node.js](https://nodejs.org/) (version 14 or higher recommended).
   - Clone or download the Potree repository.

2. **Setup**:
   - Navigate to the Potree root directory in your terminal.
   - Run `npm install` to install dependencies and build the project.

3. **Start the Server**:
   - Run `npm start` to build Potree, watch for source changes, and start a local web server at `http://localhost:1234`.

4. **Access the Example**:
   - Open your web browser and go to `http://localhost:1234/examples/classifications.html`.
   - The page will load a sample point cloud from an external source (PG&E dataset hosted on Open Topography).

5. **Usage**:
   - Use the buttons at the bottom to change classification schemes.
   - Click on the point cloud to create annotations. Enter text in the popup and save.
   - Use "Save Annotations" to persist to localStorage, "Load Annotations" to restore, or "Export/Import" for file-based persistence.

## Notes

- The point cloud data is loaded from `http://5.9.65.151/mschuetz/potree/resources/pointclouds/opentopography/CA13_1.4/cloud.js`. Ensure internet access for loading.
- Annotations are saved locally in the browser; clearing localStorage will remove them.
- For production deployment, upload the Potree folder to a web server (no Node.js required on the server).

## Troubleshooting

- If the page doesn't load, ensure the build completed successfully and the server is running.
- For CORS issues with external resources, run a local server as described.
- If annotations don't save, check browser console for errors (debug logs have been removed for cleanliness).</content>
<parameter name="filePath">e:\Development\poTree\potree\examples\README_classifications.md
