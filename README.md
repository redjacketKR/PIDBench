# PIDBench User Manual (v0.9)

![PIDBench Logo](https://github.com/redjacketKR/PIDBench/raw/main/redjacket-PIDBench.png)

## 1. Introduction

PIDBench is a GUI application designed for RotorFlight Blackbox Analysis. It provides tools to process and analyze .bbl (BlackBox Log) files, convert them to CSV format, and visualize step response data for roll, pitch, and yaw axes.

## 2. Installation

- Download the `PIDBench_v0.9_setup.exe` file from the provided source.
- Run the installer and follow the on-screen instructions.
- The installer will create a program folder and shortcuts for easy access.

## 3. Launching the Application

- After installation, launch PIDBench using the desktop shortcut or from the Start menu.
- The application will open with its main window divided into three sections:
  - Control Frame (left)
  - Plot Frame (right top)
  - Log Frame (right bottom)

## 4. Selecting Working Directory

- Click the "SELECT Logs folder" button to choose the directory containing your .bbl files.
- The selected directory path will be displayed in the "Logs folder" text box.
- The application remembers the last used directory across sessions.

## 5. File Management

- The listbox in the Control Frame displays .bbl files in the selected directory.
- Use the "REFRESH" button to update the file list if you add or remove files externally.
- Select one or multiple files in the listbox for processing.
- Use "REMOVE selected" to remove selected files from the list (does not delete files from disk).
- "CLEAR" button empties the entire listbox.

## 6. Processing Files

- "PROCESS folder" button processes all .bbl files in the selected directory.
- "PROCESS selected" button processes only the files selected in the listbox.
- Processing steps:
  1. Splits multi-session .bbl files into individual sessions.
  2. Converts single flight session .bbl files into CSV format.
  3. The software moves original .bbl files to an "original_bblogs" subdirectory.

## 7. Generating Plots

- After processing, click the "PLOT listed" button to generate step response plots.
- The application will create three subplots for Roll, Pitch, and Yaw axes.
- Each processed file will be represented by a different colored line on the plots.
- The plots show the step response over time, with reference lines at y=1 and x=20ms, 100ms.

## 8. Analyzing Results

- The application calculates and displays peak values and delay times for each axis and each processed file.
- It also computes the area between y=1 and each curve, which can be used to compare overall performance.
- The legend for each plot is located in the lower right corner and can be used to identify which line corresponds to which file.

## 9. Exporting Results

- Use the toolbar below the plot for various options:
  - Pan and zoom the plot for detailed inspection.
  - Save the plot as an image file (PNG, JPG, PDF, or SVG).
- The application automatically suggests a filename based on the current date and "combined step response".

## 10. Additional Features and Support

- Access the "About" window from the Help menu for version information and third-party library details.
- A donation link is available for users who wish to support the development.
- The Log Frame at the bottom provides real-time feedback on application operations and any errors encountered.
- For uninstallation, use the "Uninstall PIDBench" shortcut in the Start menu or the Windows Control Panel.

## Tips for Effective Use

- Ensure your .bbl files are in the selected directory before processing.
- For best results, process files from similar flight conditions or tuning sessions together.
- Use the legend and color coding to compare performance across different configurations.
- Pay attention to the peak values and delay times to assess the responsiveness of your craft.
- The area calculation can help identify the most optimal tune among multiple files.

## Troubleshooting

- If files are not appearing in the listbox, use the "REFRESH" button.
- Check the Log Frame for any error messages if processing or plotting fails.
- If the application fails to start, ensure your Windows version is compatible (Windows XP and later are supported).
- For very large files or many files, allow sufficient time for processing and plotting. If .bbl files are very large and/or in a slightly different format, use external converters like blackbox splitter and decoder.exe (available on GitHub).

Remember, PIDBench is a tool to assist in your tuning process. Always combine these analytical results with real-world flight testing for the best outcomes. Filter out noise for a good and fast response.

---

RJ thank the RF development team very much for their work.



