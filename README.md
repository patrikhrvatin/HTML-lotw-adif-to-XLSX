# WAJA LoTW Log Processor

A simple, client-side web tool to process your **LoTW (Logbook of the World) ADIF** files and generate a detailed **WAJA (Worked All Japan Award)** status report in Excel format.

## Features

* **No Server-Side Processing:** Your log files are processed entirely in your web browser. Your data never leaves your computer.
* **Automatic Statistics:** Generates a "Statistics" tab showing your progress (e.g., 22/47) for each band (160m - 6m).
* **Missing Prefectures List:** Automatically lists the exact names of the prefectures you are still missing for each band.
* **Band-Specific Reports:** Creates individual tabs for each band (160m to 6m) with a complete list of all 47 Japanese prefectures.
* **Easy to Use:** Just select your ADIF file and download the Excel report.

## How to use

1. Download the `japan_map_prefectures_xls6.html or english version japan_map_prefectures_xls7.html` file from this repository.
2. Open it in any modern web browser (Chrome, Firefox, Edge, etc.).
3. Click the **"Choose File"** button and select your `lotwreport.adi` file.
4. Click **"Download Excel with Statistics"** to generate and save your report.
5. Copy/paste all generated data in the Original XLS file from JARL site sample-form -2tabs.xls
## Requirements

* None. This tool uses the [SheetJS (xlsx)](https://sheetjs.com/) library via CDN, so it works offline as long as the page is already loaded.

## Technical Details

* **Language:** HTML5, JavaScript.
* **Parser:** Uses Regular Expressions to parse ADIF data, specifically targeting the `<STATE>` tag to identify Japanese prefectures (1-47).
* **Filtering:** Automatically filters your log for `DXCC: 339` (Japan).

## License

Feel free to use, modify, and share this tool for your personal amateur radio needs. 73!

---

