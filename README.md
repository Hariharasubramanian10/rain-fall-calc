# Rainfall Analysis Project

## Overview

This project is a C program designed to analyze and calculate yearly and monthly average rainfall data over a specified number of years. The user inputs rainfall data for each month over several years, and the program provides a summary, including yearly rainfall totals and average rainfall for each month.

## Features

- **User-Specified Data Range**: The program allows the user to define the range of years for which the rainfall data will be analyzed.
- **Yearly Rainfall Calculation**: For each year within the specified range, the program calculates the total rainfall and displays it.
- **Monthly Average Calculation**: The program computes and displays the average rainfall for each month over the entire data range.
- **Yearly Average**: The program calculates the average yearly rainfall.

## How to Run the Program

1. **Compile the Program**:
   - Use any C compiler to compile the code. For example:
     ```bash
     gcc rainfall_analysis.c -o rainfall_analysis
     ```

2. **Run the Executable**:
   - After compiling, run the program:
     ```bash
     ./rainfall_analysis
     ```

3. **Input Data**:
   - The program will prompt you to enter the number of years of data you want to analyze.
   - You will then input the start and end years (e.g., 2010-2015).
   - Finally, you will be asked to enter the rainfall data for each month of each year.

4. **View Results**:
   - The program will output the total rainfall for each year, the average rainfall for each month across all years, and the overall yearly average.

## Example Output

```
How many years of data you want to enter: 3
Data from which year to which year: 2010 - 2012
Enter data of every month:
1. 3.4
2. 2.8
...

YEAR       RAINFALL (INCHES)
2010              32.5
2011              28.9
2012              35.2

The yearly average is: 32.20 inches.

MONTHLY AVERAGES

 JAN  FEB  MAR  APR  MAY  JUN  JUL  AUG  SEP  OCT  NOV  DEC
3.0  2.5  3.1  2.7  2.8  3.4  3.0  2.9  2.7  3.0  3.3  2.8 
```

## Code Explanation

- **Variables**:
  - `YEARS`, `months`, `no_of_years`, `year`: Control the loops and manage the data input.
  - `sum`, `avg`, `total`: Used to store and calculate rainfall sums and averages.
  - `year1`, `year2`: Store the start and end years for analysis.

- **Data Storage**:
  - A 2D array `yearrain[no_of_years][MONTHS]` stores the rainfall data for each year and month.

- **Loops**:
  - Outer loop iterates over the years, and the inner loop iterates over the months, collecting and processing data.

- **Output**:
  - The program outputs the total rainfall for each year and calculates the average monthly and yearly rainfall.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

You can copy and paste this directly into your GitHub repository's README file!
