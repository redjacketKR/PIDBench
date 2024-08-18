🔄 PIDBench Update Notice 🛠️
An issue has been identified and resolved regarding file path resolution when processing single files. This fix ensures all file operations now use full paths, improving the application's overall reliability.
To update your installation:

Download the new PIDBench.exe file from the [official repository](https://github.com/redjacketKR/PIDBench/releases/download/v0.9/PIDBench.exe).
Replace the existing file at C:\Program Files (x86)\redjacketRC\PIDBench\PIDBench.exe with the newly downloaded version.

This update addresses the file path resolution problem. We apologize for any inconvenience caused. Your patience and feedback are greatly appreciated, as they contribute to the ongoing improvement of the software.

Download link: [PIDBench.exe](https://github.com/redjacketKR/PIDBench/releases/download/v0.9/PIDBench.exe)
Installation path: C:\Program Files (x86)\redjacketRC\PIDBench\PIDBench.exe




# 🚀 **PIDBench User Manual (v0.9)**


<p align="center">
  <img src="https://github.com/redjacketKR/PIDBench/raw/main/redjacket-PIDBench.png" alt="PIDBench Logo" width="500"/>
  <img src="https://github.com/redjacketKR/PIDBench/blob/main/PIDBench_QgJ0GWfuky.png" alt="PIDBench Main Window" width="1200"/>
</p>

<h2 style="color: #1976D2;">1. Introduction</h2>

PIDBench is a GUI application designed for <span style="color: #0277BD;">Rotorflight Blackbox Analysis</span>. It provides tools to process and analyze <span style="color: #0277BD;">.bbl (BlackBox Log)</span> files, convert them to CSV format, and visualize step response data for roll, pitch, and yaw axes.

<h2 style="color: #1976D2;">2. Installation</h2>

- Download the `PIDBench_v0.9_setup.exe` file from the provided source.
- Run the installer and follow the on-screen instructions.
- The installer will create a program folder and shortcuts for easy access.

<h2 style="color: #1976D2;">3. Launching the Application</h2>

- After installation, launch PIDBench using the desktop shortcut or from the Start menu.
- The application will open with its main window divided into three sections:
  - <span style="color: #0277BD;">Control Frame</span> (left)
  - <span style="color: #0277BD;">Plot Frame</span> (right top)
  - <span style="color: #0277BD;">Log Frame</span> (right bottom)

<h2 style="color: #1976D2;">4. Selecting Working Directory</h2>

- Click the "<span style="color: #0277BD;">SELECT Logs folder</span>" button to choose the directory containing your .bbl files.
- The selected directory path will be displayed in the "Logs folder" text box.
- The application remembers the last used directory across sessions.

<h2 style="color: #1976D2;">5. File Management</h2>

- The listbox in the Control Frame displays .bbl files in the selected directory.
- Use the "<span style="color: #0277BD;">REFRESH</span>" button to update the file list if you add or remove files externally.
- Select one or multiple files in the listbox for processing.
- Use "<span style="color: #0277BD;">REMOVE selected</span>" to remove selected files from the list (does not delete files from disk).
- "<span style="color: #0277BD;">CLEAR</span>" button empties the entire listbox.

<h2 style="color: #1976D2;">6. Processing Files</h2>

- "<span style="color: #0277BD;">PROCESS folder</span>" button processes all .bbl files in the selected directory.
- "<span style="color: #0277BD;">PROCESS selected</span>" button processes only the files selected in the listbox.
- Processing steps:
  1. Splits multi-session .bbl files into individual sessions.
  2. Converts single flight session .bbl files into CSV format.
  3. The software moves original .bbl files to an "original_bblogs" subdirectory.

<h2 style="color: #1976D2;">7. Generating Plots</h2>

- After processing, click the "<span style="color: #0277BD;">PLOT listed</span>" button to generate step response plots.
- The application will create three subplots for Roll, Pitch, and Yaw axes.
- Each processed file will be represented by a different colored line on the plots.
- The plots show the step response over time, with reference lines at y=1 and x=20ms, 100ms.

<h2 style="color: #1976D2;">8. Analyzing Results</h2>

- The application calculates and displays peak values and delay times for each axis and each processed file.
- It also computes the area between y=1 and each curve, which can be used to compare overall performance.
- The legend for each plot is located in the lower right corner and can be used to identify which line corresponds to which file.

<h2 style="color: #1976D2;">9. Exporting Results</h2>

- Use the toolbar below the plot for various options:
  - Pan and zoom the plot for detailed inspection.
  - Save the plot as an image file (PNG, JPG, PDF, or SVG).
- The application automatically suggests a filename based on the current date and "combined step response".

<h2 style="color: #1976D2;">10. Additional Features and Support</h2>

- Access the "<span style="color: #0277BD;">About</span>" window from the Help menu for version information and third-party library details.
- A donation link is available for users who wish to support the development.
- The Log Frame at the bottom provides real-time feedback on application operations and any errors encountered.
- For uninstallation, use the "Uninstall PIDBench" shortcut in the Start menu or the Windows Control Panel.

<h2 style="color: #1976D2;">Tips for Effective Use</h2>

- Ensure your .bbl files are in the selected directory before processing.
- For best results, process files from similar flight conditions or tuning sessions together.
- Use the legend and color coding to compare performance across different configurations.
- Pay attention to the peak values and delay times to assess the responsiveness of your craft.
- The area calculation can help identify the most optimal tune among multiple files.

<h2 style="color: #1976D2;">Troubleshooting</h2>

- If files are not appearing in the listbox, use the "REFRESH" button.
- Check the Log Frame for any error messages if processing or plotting fails.
- If the application fails to start, ensure your Windows version is compatible (Windows XP and later are supported).
- For very large files or many files, allow sufficient time for processing and plotting. If .bbl files are very large and/or in a slightly different format, use external converters like blackbox splitter and decoder.exe (available on GitHub).

Remember, PIDBench is a tool to assist in your tuning process. Always combine these analytical results with real-world flight testing for the best outcomes. Filter out noise for a good and fast response.

---

<p style="color: #1976D2;">RJ thank the RF development team very much for their work.</p>

