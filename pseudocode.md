## Part 5 – Advanced Practice: Issues & Pseudocode (≈1–1.5 hrs)
1. In GitHub Desktop, create another branch called `analysis-draft`.  
2. Create a new file called `pseudocode.md`.  
3. Write **pseudo-code** (descriptive steps, not actual code) for analyzing a dataset:  
   - Step 1: Load the dataset  
   - Step 2: Clean the data (explain how)  
   - Step 3: Calculate summary statistics  
   - Step 4: Create a visualization  
   - Step 5: Interpret results  
4. Commit and push this file to `analysis-draft`.  
5. On GitHub.com, open a new **Issue** titled *Draft pseudocode for analysis*.  
6. Open a Pull Request to merge `analysis-draft` → `main`.  
   - In the PR description, type `Closes #<issue-number>` to link it to the Issue.  
7. Merge the PR into `main`.  

### Step 1: Load the Dataset

    1. read data <- read in data from csv or whichever source
    
    2. initial brief summary <- initial summary of data to ensure that everything imported as expected, column/row names are correct
    
    3. nrows / ncols <- check to ensure that not only is the formatting correct, the amount of data we'd expect is present
    
### Step 2: Clean the Data

    1. NAs <- check for NAs throughout dataset, decide best way to handle them (remove columns/rows, impute means, etc.)
    
    2. Create calculated variables <- if necessary, add columns/rows to the dataset with calculated figures based on the type of analysis being done. Either transformations of one variable or combined with others.
    
    3. Anonymize <- Also if necessary based on the sensitivity of data, exchange potentially revealing data for anonymized names, IDs, income brackets, regions, etc. 
    
### Calculate Summary Statistics

    1. Determine typical summary statistics for continuous variables - mean, median, standard deviation, quartiles
    
    2. Create frequency/proportion tables for categorical variables
    
    3. For suspected interactions, covariance/correlation matrices, 
    
### Create a Visualization

    1. Based on the nature of the question being asked and the data present, create relevant plots to visualize distribution/interactions 
    
    2. Test assumptions of whichever figures are being visualized, create additional relevant visualizations to ensure that assumptions are satisfied. 
    
### Interpret results

    1. Refer back to question being asked, determine whether visualizations and summary statistics support a specific answer or require further investigation. 
    