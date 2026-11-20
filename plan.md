Plan 1: Quarto Report

Goal:
Create a Quarto report that brings together the course analyses: descriptive 
statistics tables of diamond size by clarity, an NCAA three-point line plot, a 
Monte Carlo estimate of the area under a curve, a calcium tidying plan with a 
GenAI comparison, a reflection, and appendices for GenAI use and code.

SG1: Set up the Quarto report and load packages
SG2: Create a section of the Diamonds statistics tables (length, width, height)
SG3: Create a section of the NCAA three-point attempts line plot
SG4: Create a section of the Monte Carlo integration figure
SG5: Document the Planning and Prompting GenAI Tools section (calcium)
SG6: Write the Reflection and create the appendices
SG7: Render my Reproducible Data Quarto Report

Needs:
Nouns: the {tidyverse}, {janitor}, {knitr} and {kableExtra} packages, Quarto 
document (.qmd), diamonds data, team_box.csv, coordinate generator function, 
chi-square density curve, calcium.csv, ChatGPT plot, generic AI plot, reflection

Verbs: install, load packages, clean, compute, summarize, format, define, 
generate, estimate, plot, tidy, compare, describe, document, write, render

Functions and Operators: library, <-, |>, +, filter_out, filter, select, group_by, 
summarise, quantile, adorn_rounding, kable, kable_styling, add_header_above, 
read.table, read_csv, is.na, mean, function, tibble, runif, dchisq, mutate, 
row_number, relocate, bind_rows, set_names, paste, round, ggplot, aes, geom_line, 
geom_point, geom_abline, stat_function, scale_color_manual, coord_cartesian, labs, 
theme_bw, theme, include_graphics

Steps

1. Create the Quarto document with a title, author, date and output format. Load 
  packages in the first chunk.
2. Diamonds tables.
      a. Use my work for my table from homework 3.4. In this assigment, I only 
          used x, or length statistics.
      b. recreate two new tables for width and height as well (y and z), by 
        changing the variable
      c.  Format each table with a caption, column names, a header above the columns, 
          and commas in the counts.
      d. Repeat for length (x), width (y) and height (z).
      e. Write a short interpretation under each table.
3. NCAA line plot.
      a. Use my work from 3.4, but with improvements. Add alt text where I forgot,
        and use relative file path. 
      b. Insert that visualization, then use my previous narrative that says how the 
        attempts changed from 2006 to 2026 and what that might mean for the Big Ten 
        Academic Alliance.
4. Monte Carlo figure.
      a. Reuse my 3.4 function that generates random x and y coordinates, but
        improve based on the feedback i got. Name all of my assignments, and 
        rename the whole function to be a verb
      b. combine the four plots using my previous code, but with updates
      c. display the four sub figures the Quarto way, upload each to ASU image 
        website and use four alt texts.
5. Planning and prompting section.
      a. write a plan to tidy the calcium data
      b. create plan informed prompt by asking ChatGPT to write my code
      c. record the generic AI prompt, and include its plot.
      d. Compare the two results.
6. Write the reflection on learning R, functions, data wrangling and visualizations.
7. Code appendix
    Appendix A: for each AI use, record the tool, the date, what was provided, 
    the exact response, and any changes made. Include the alt text for every figure.
    Appendix B: include all the code used in the report.
8. Render and check, then save as PDF
9. Coding
    Load {tidyverse}, {janitor}, {knitr} and {kableExtra} using library
    Build the diamonds statistics with filter_out, select, group_by and summarise, 
      then format them with kable
    Read team_box.csv with read.table, summarize by season, and plot with geom_line and geom_point
    Define the coordinate generator with function and runif
    Wrangle each Monte Carlo set with mutate and dchisq, and plot with stat_function
    Tidy the calcium data with select, set_names, bind_rows and relocate
    Create the calcium plot with ggplot, geom_point and geom_abline
    Render the document
    
Plan 2: 4.3 GitHub Repository Plan

Goal
Create a public GitHub repository that documents the development of HW #4.3 using 
branches, Issues, commits, and a pull request.

SG1: Set up the repository
SG2: Organize and add the project files
SG3: Maintain the repository while completing the assignment
SG4: Review and merge the completed work

Needs

Nouns: GitHub repository, GitHub Desktop, README.md, plan.md, QMD file, PDF file, main branch, development branch, Issues, commits, pull request

Verbs: create, organize, add, save, commit, push, update, check, review, merge

Guthub functions: commit, push, branch, Issue, pull request

teps

1. Create a public GitHub repository for HW #4.3.
2. Create a development branch separate from the main branch.
3. Create at least two Issues related to completing and finalizing HW #4.3.
4. Add the completed QMD and PDF files to the development branch.
5. Commit the QMD and PDF to the development branch with a clear commit message.
6. Push the changes to GitHub.
7. Add and maintain the README and this plan document in the repository.
8. Continue making meaningful commits to the development branch as changes are made.
9. Check the repository to make sure the required files are present and organized.
10. Create a pull request from the development branch to the main branch once the 
    work is complete.
11. Review the pull request and merge the development branch into main.
12. Complete a final check of the main branch to confirm that the README, plan, 
    QMD, PDF, Issues, commits, and pull request provide evidence of the completed workflow.

GitHub Workflow

1. Make or update a file in the local repository.
2. Review the changes in GitHub Desktop.
3. Commit the changes to the development branch using a clear commit message.
4. Push the development branch to GitHub.
5. Repeat this process whenever a meaningful change is made.
6. When the assignment is complete, create a pull request from the development branch to main.
7. Merge the pull request into main after reviewing the completed work.