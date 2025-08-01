# CFD Post Automation Tool

A web-based utility to automate the generation of visualization scripts for ANSYS CFD-Post. This tool turns a repetitive, 30-minute manual task into a swift, 2-minute automated process.



## Key Links

**[View Source Code (`index.html`)](https://github.com/midhun16042000/CFD-POST-AUTOMATION-TOOL/blob/main/index.html)**


## The Problem: Tedious & Repetitive Workflows

In CFD analysis, post-processing is a critical but often time-consuming phase. Manually performing tasks like coloring boundaries, creating planes, and setting up contour plots for every simulation is inefficient and prone to error. This manual process hinders productivity and can lead to inconsistent report visuals.

## How It Works

1.  **Paste Raw Data:** The user copies session data directly from the CFD-Post Command Editor and pastes it into the tool.
2.  **Review & Edit:** The tool intelligently parses the input to extract all Domain and Boundary names. The user can then remove items, configure plane heights, and modify visual properties.
3.  **Generate & Download Scripts:** With a single click, the tool generates clean `.cse` session files for surface coloring and velocity plots.

## Technology Stack

* HTML5
* Tailwind CSS
* Vanilla JavaScript

## Impact & Results

* **Massive Time Savings:** Reduces post-processing setup time by over 90%.
* **Guaranteed Consistency:** Ensures all reports and visuals follow a standardized format.
* **Reduced Errors:** Eliminates the risk of manual mistakes during setup.
