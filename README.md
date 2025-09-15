#  Pore Volume Calculator

This is a simple HTML + JavaScript app that helps estimate **reservoir pore volume** in sand zones using well log data.

**This project was developed as part of a coursework assignment for the "Introduction to Oil and Gas Engineering" module.**  
It implements a basic model for pore volume calculation using typical well log data.

**[Live preview (HTMLPreview)](https://htmlpreview.github.io/?https://github.com/GannaUK/log_calculator/blob/main/index.html)**

##  Features

- Manual input of log data (Depth, GR, DPHI, NPHI)
- Calculates porosity and pore volume for each 10 ft interval
- Displays total and average values
- Left panel for visual logs (image), right panel for calculations

##  Formula Used

```
Pore Volume = Area × Thickness × Porosity × 7758
```

Where:
- **Area** = 49,720 acres
- **Thickness** = 10 ft per row
- **Porosity (ϕ)** = average of DPHI and NPHI
- **7758** = conversion factor to barrels

##  How to Use

1. Open the `index.html` file in a browser.
2. Modify the log data (if needed) in the text area.
3. Click **"Calculate"**.
4. View the results in the table on the right.

##  Layout

- **Left side** – Log image (for visual reference)
- **Right side** – Data input and results

##  Example Log Format

```
Depth,GR,DPHI,NPHI
6360,28,0.23,0.25
6370,29,0.24,0.26
...
```
