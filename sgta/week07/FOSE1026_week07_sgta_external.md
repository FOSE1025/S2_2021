# Week 7 SGTA (External offering)

## Activity 1 - Importing CSV data to Excel Online (5 minutes + 5 minutes discussion)

The following URL points to a list of CSV files (Comma-Separated Value). We will use some of them in the lectures:

* https://people.sc.fsu.edu/~jburkardt/data/csv/csv.html

Download the file "homes.csv" and open it using **Excel Online** (not the desktop app). Remember the process, as described in week 6 video 1 and in the lecture:

1. Upload the CSV file to OneDrive.
2. Double-click on the file. This will open Excel Online.
3. Enable editing and follow the prompts. This will save the file to the Excel format (.xlsx).

## Activity 2 - Writing Instructions (15 minutes + 10 minutes discussion)

Below is a list of Excel tasks that you have learnt so far. The list is not exhaustive:

  1. Week 3: Filter data.
  2. Week 3: Sort data.
  3. Week 4: Validate data.
  4. Week 4: Look up at data using VLOOKUP.
  5. Week 5: Plot data.

Choose one of these tasks and write specific instructions that would help someone else complete the task.

Now, exchange your instructions with those of your peer (use the iLearn discussion forum for this) and assess how good they are for reproducibility. Are the instructions clear enough to help you complete the task?

## OPTIONAL Activity 3 - Git and Github (10 minutes + 5 minutes discussion)

This activity is optional for those who have completed activities 1 and 2.

The lectures have mentioned git and github. These two are related but different technologies to manage software repositories and help collaboration. Answer the following questions by searching the web or based on your own experience:

1. What is the difference between git and github?
2. You can use git outside of github. Give an example of how you could do this.
3. While it could be possible to use github without using git, in practice, normally you would not want to do it. Explain why.

## Activity 4 - Upload files to MATLAB Drive (10 minutes + 10 minutes discussion)

The following links lead to MATLAB Online. Use them to start MATLAB Online:

* Information about MATLAB licenses for Macquarie University students: https://au.mathworks.com/academia/tah-portal/macquarie-university-916052.html
* Access MATLAB Online: https://matlab.mathworks.com/

Download all the CSV files from this folder:

* [MonthlySalesFiles](MonthlySalesFiles) 

and save them in a MATLAB Drive folder named `MonthlySalesFiles`.

To upload the CSV files into MATLAB Drive, try the following two options and discuss the advantages and inconveniences of each:

1. Create the folder by interacting with MATLAB Online at https://matlab.mathworks.com.
    1. Create the folder `MonthlySalesFiles` by using the "New" option.
    2. Double-click on the folder to make it active.
    3. Upload the files to MATLAB Drive by using the "upload" option (or clicking and dragging them).
    If the files do not appear in your folder `MonthlySalesFiles`, click and drag them to the right folder.

2. Create the folder by interacting with MATLAB Drive https://drive.matlab.com/:
    1. Create a folder `MonthlySalesFiles` by using the "New Folder" option.
    2. Double-click on the folder to make it active.
    3. Upload the files by using the "Upload" option.
    If the files do not appear in your folder `MATLAB Workshop`, click and drag them to the right folder.

## Activity 5 - Generate a Live Script (15 minutes + 10 minutes discussion)

Generate a Live Script that imports the sales data from January by following these steps:

1. Double-click on the CSV file that has the January sales data. The "Import Data" wizard will open.

2. Inspect the options of the "Import Data" wizard and change these options so that:

    1. The name of the variable is `sales_jan`.
    2. The type of the column `OrderDate` is `Datetime`.
    3. The type of the columns `Category` and `PaymentType` is `Categorical`.
    4. The type of all other non-numerical columns is `Text`.
    5. The type of all numerical columns is `Number`.

3. Select `Generate Live Script` under the option `Import Selection`.

4. Save the generated live script as a file with name `import_jan_data.mlx`.

5. Run the generated live script and check that the workspace has a variable with name `sales_jan` and the contents of the variable is correct.


## OPTIONAL Activity 6 - Modify the script so that it imports all sales data (15 minutes)

1. Examine the script `import_jan_data.mlx` from activity 2. Do you understand it? Discuss with your peers the meaning or possible meaning of each line of code from the script.

2. Make a copy of the script and rename the copy to `import_all_data.mlx`. Edit the script so that it now imports all three CSV files (January, February, March). After running the script, the workspace should have three variables `sales_jan`, `sales_feb`, `sales_mar`, so that each variable contains the data of one CSV file. (*hint: You only need to copy and edit the line that says `sales_jan = readtable(...)` so that there are three lines, one per each table.*)

# Participation tasks

1. Submit your assessment of your peer's instructions from Activity 2.
2. Download and submit the script `import_jan_data.mlx` that you created in Activity 5.
