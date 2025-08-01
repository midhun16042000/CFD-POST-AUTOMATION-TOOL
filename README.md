
# CFD Post Automation Tool

A web-based utility to automate the generation of visualization scripts for ANSYS CFD-Post. This tool turns a repetitive, 30-minute manual task into a swift, 2-minute automated process.

## The Problem: Tedious & Repetitive Workflows

In CFD analysis, post-processing is a critical but often time-consuming phase. Manually performing tasks like coloring boundaries, creating planes, and setting up contour plots for every simulation is inefficient and prone to error. This manual process hinders productivity and can lead to inconsistent report visuals.

## How It Works

1.  **Paste Raw Data:** The user copies session data directly from the CFD-Post Command Editor and pastes it into the tool.
2.  **Review & Edit:** The tool intelligently parses the input to extract all Domain and Boundary names. The user can then remove items, configure plane heights, and modify visual properties.
3.  **Generate & Download Scripts:** With a single click, the tool generates clean `.cse` session files for surface coloring and velocity plots.

## Steps to Use

### Part 1: In ANSYS CFD-Post
1. Load your results file (`.dat` or `.res`).
2. In the session tree, right-click the loaded results file and select **"Edit in Command Editor"**.
3. Copy the entire content from the Command Editor window (`Ctrl+A`, `Ctrl+C`).

### Part 2: In the Automation Tool
4. Paste the copied content into the first text area of the tool and click **"Extract Names"**.
5. Review and edit the extracted lists as needed.
6. Click **"Generate Scripts"** and download both `.cse` files.

### Part 3: Back in ANSYS CFD-Post
7. Go to **Session > Play Session...** and run the first script (`...surface_colour...`).
8. Go to **Session > Play Session...** again and run the second script (`...contour_creation...`).
9. Your scene will be automatically generated.

## Technology Stack

* HTML5
* Tailwind CSS
* Vanilla JavaScript

## Impact & Results

* **Massive Time Savings:** Reduces post-processing setup time by over 90%.
* **Guaranteed Consistency:** Ensures all reports and visuals follow a standardized format.
* **Reduced Errors:** Eliminates the risk of manual mistakes during setup.
