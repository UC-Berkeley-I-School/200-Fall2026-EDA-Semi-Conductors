# W200: Project 2 - Exploratory Data Analysis

Welcome to your final project for W200! This is your opportunity to apply the Python, NumPy, and pandas skills you've learned throughout the semester to explore a dataset that genuinely interests you. You'll work in a team to find a dataset, ask interesting questions about it, and present your findings.

## Learning Outcomes

* Manage a team-based coding workflow using Git and GitHub, including setting up a private repository, collaborating on Python source files and notebooks, and resolving merge conflicts.
* Identify a suitable real-world dataset and formulate specific, answerable guiding questions to scope an analysis project.
* Utilize Python, NumPy, and pandas to ingest raw data, handling specific real-world issues such as missing values, inconsistent data types, and outliers, while documenting all cleaning decisions.
* Generate annotated visualizations using a Python plotting library that directly support the project's guiding questions.
* Compose a reproducible report that integrates written analysis and supporting visualizations into a cohesive narrative suitable for a technical stakeholder.


## Key Deadlines

* **Week 10:** Each student proposes a dataset in the [Project 2 Sign-up Sheet][signup] by **11:59 PM Pacific Time the day before class**.
* **Week 11:** By **11:59 PM Pacific Time the day before class**:
    * Form your team, add it to the sign-up sheet, and create your team's GitHub repository.
    * Submit your formal **Project Proposal** to your team's GitHub repository, email the link to your section instructor (CC-ing the rest of your team), and submit it to Gradescope.
* **Week 14 (During Class):** Your team will give a **10-minute presentation**.
* **Week 14 (After Class):** By **11:59 PM Pacific Time the day after class**:
    * Upload a PDF of your presentation slides to GitHub.
    * Submit your **Final Report** (PDF) to GitHub and Gradescope.


## Project Breakdown

This project has five main components: data sourcing, team formation and repo setup, the proposal, an in-class presentation, and a final report.

### Part 0: Dataset Sourcing

This part is done individually, before teams are formed. After Week 9, find a dataset on the internet that you're interested in. The dataset should be public (no private data sources, even if you work at or own the company).
* Make sure it has **at least 100 rows and at least 4 analyzable columns per team member**. Analyzable columns hold values you can study, not identifiers or record-keeping fields such as IDs, names, URLs, or "last updated" timestamps.
* You may combine multiple datasets, which can help a larger team reach the column minimum.
* Do not use synthetic / simulated datasets (these are especially common on Kaggle).

Here are some great places to start your search:
* [Awesome Public Datasets](https://github.com/caesar0301/awesome-public-datasets)
* [Data is Plural](https://www.data-is-plural.com/)
* [Data.gov](https://data.gov/)
* [Google Dataset Search](https://datasetsearch.research.google.com/)
* [Hugging Face](https://huggingface.co/datasets)
* [Kaggle](https://www.kaggle.com/datasets)
* [KDnuggets](https://www.kdnuggets.com/datasets/index.html)
* [Open Data Inception](https://opendatainception.io/)
* [Opendatasoft](https://data.opendatasoft.com/explore/dataset/open-data-sources%40public/table/?sort=code_en)
* [r/datasets](https://www.reddit.com/r/datasets)
* [... and more](https://www.google.com/)

Propose your dataset in the [Project 2 Sign-up Sheet][signup]. Classmates can browse the proposed datasets to find teammates with similar interests.


### Part 1: Team & GitHub Setup (5% of Grade)

1. **Form a Team:** Your team must include a minimum of 2 and a maximum of 4 students, and all teammates must come from the same section. Add your team members to the [Project 2 Sign-up Sheet][signup]. We recommend making a private Slack channel for yourselves to facilitate communication (do not add the instructors).

2. **Choose Your Team's Dataset:** Pick one of the datasets your teammates proposed in Part 0 (or a combination of them). If you aren't sure whether a dataset is suitable, email it to your section instructor for feedback before writing your proposal.

3. **Create a GitHub Repository:**
    * Set up a new repository in the `UC-Berkeley-I-School` organization.
    * Make sure your repository is private.
    * Name it using this format: `200-[SEMESTER][YEAR]-EDA-[TEAMNAME]`. For example: `200-FA26-EDA-Climate-Change`.
        * Use SP, SU, and FA for semester.
        * Use the last two digits of the year (e.g., 26 for 2026).
        * Your team name can be anything you want, but it should be descriptive of your project.
    * Give your teammates **Write** access and the W200 instructors **Read** access (Settings > Collaborators and teams).


### Part 2: The Proposal (10% of Grade)

This is a 1-2 page PDF document where you outline your project plan.

**Your proposal must include:**

* The names of all team members.
* The full name of and link to your team's GitHub repository.
* Your planned mode of communication and any regular meeting times from now until Week 14.
* A description of the primary dataset you plan to analyze, including a link to it.
* A list of the variables (columns) you find most interesting and what you hope to learn from them.
* 2-4 guiding questions your analysis will try to answer. These should be specific and answerable with your dataset; you may refine them as your analysis progresses.
* Information on any supplemental datasets you might use to enrich your analysis.
* A timeline of milestones that you collectively agree to adhere to from now until the submission of the final report.

### Part 3: The In-Class Presentation (20% of Grade)

During our final class, your team will present your findings in PowerPoint / slides format for **10 minutes**, followed by a 5-minute Q&A. Every team member should present part of the talk.

**Your presentation should:**

* Clearly state the main questions your analysis sought to answer.
* Walk the audience through your data exploration and cleaning process.
* Explain any assumptions you made.
* Tell a compelling story with your data, using key charts and graphs to guide your narrative.

You don't need to show your code, but you might get follow-up questions about how you treated your data.

### Part 4: The Final Report (65% of Grade)

This is the main deliverable: a polished technical write-up, submitted as a PDF, that details your exploratory data analysis. The report should not include code; it should contain your written analysis along with supporting figures and tables. The goal is to tell a clear and compelling story about your findings. There are no required section headers, as each EDA will be different. We've included a sample structure to get you started in [Example Project Structure](#example-project-structure) below. **We expect at least 400 words per student in the group, but no more than 3,000 words total.**

**Keys to a Great Report:**
* **Tell a Story:** Your analysis should be a written argument. Guide the reader through your process and what the data reveals.
* **Explain Your Figures:** Every single plot or graph should be explained. If a visualization isn't important enough to write about, don't include it. You may use any Python plotting library (e.g., matplotlib, seaborn, plotly), as long as the figures are generated by code in your repository.
* **Document Everything:** Clearly state if you remove data points, transform variables (e.g., taking a logarithm), or have to handle suspicious values. A simple sentence is often enough.
* **Stick to Descriptive Statistics:** Your analysis should focus on summarizing the data you have. Avoid making broad claims about a larger population. **Do not use words like "significant,"** which imply statistical testing we haven't covered.
* **Ensure Your Methods Are Sound:** The way you calculated your results should be clear from your writing and reproducible from the code in your GitHub repository. Do not go on fishing expeditions or otherwise manipulate your data to get the results you want.

Your report should not be a comprehensive compilation of everything your team tried. It should be a thoughtful selection of text and figures that tell the story you want it to. A helpful rule of thumb is to pretend a VP of Engineering will be reading your report: they won't read your code, but they should be able to understand how you arrived at each result. The code that produces every figure and number in your report should be in your GitHub repository.

### Submission

All files for Project 2 should be uploaded to GitHub.

1. Proposal
    * Upload a PDF of your proposal to GitHub with the text `proposal_` prepended, email the link to your section instructor (CC-ing the rest of your team), and submit the PDF to Gradescope. 1 submission per team.
2. Presentation
    * Upload a PDF of your presentation slides to GitHub with the text `presentation_` prepended.
3. Final Report (.pdf)
    * A single readable PDF report of the exploratory data analysis (no code) should be uploaded to GitHub and Gradescope with the text `report_` prepended. 1 submission per team.
4. Additional files
    * A `README.md` file should be included in your repository with a brief description of your project, your directory structure, the dataset(s) you used, and instructions for how to run your code.   
    * If each of your data files is under 50 MB, upload them to GitHub under a `data/` directory. Otherwise, don't commit them (GitHub rejects files over 100 MB); instead, include a link to the data and instructions or a script for downloading it in your repository's README.
    * All code, including the notebook(s) that produce the figures and numbers in your report and any individual / prototyping notebooks, should also be uploaded to GitHub under `src/`.
    * You may package reusable functions in .py files uploaded to GitHub, also under `src/`. If you do, make sure to include a README with instructions for how to import and use them.

For Gradescope submissions, one teammate submits and adds the rest of the team to the group submission.

Please ensure that your GitHub repository is up to date in addition to your Gradescope submissions.


## Collaboration Tips

Collaborating on a Jupyter Notebook with GitHub can be tricky because notebooks are complex JSON files, making merge conflicts difficult to resolve. The best approach is to communicate frequently and establish a clear workflow.


### GitHub Workflow

The fundamental workflow for team collaboration on GitHub is: **pull, edit, commit, push**.

1. **Pull Before You Work:** Always run `git pull` before you start making any changes. This fetches the latest version of the project from the repository, ensuring you're not working on an outdated copy.
2. **Communicate Your Work:** Let your teammates know which part of the notebook you are editing. The simplest way to avoid conflicts is to not have two people edit the same notebook at the same time.
3. **Commit and Push Often:** Make small, frequent commits with clear messages. Instead of working for hours and making one large push, push your changes after completing a small task. This keeps the project updated and makes it easier to track changes.

### Avoiding Merge Conflicts

Merge conflicts are the biggest challenge. They happen when two people change the same lines in a file. With notebooks, even running a cell can change the underlying JSON, leading to a conflict.

* **Work in Separate Notebooks:** One effective strategy is for each team member to work on a separate notebook for their part of the analysis. At the end, you can combine the finalized code into a main analysis notebook that produces the figures for your report.
* **Clear Output Before Committing:** Notebook output (like plots and tables) adds a lot of data to the JSON file. It's a good practice to clear all cell outputs before you commit and push your changes (JupyterLab: `Edit > Clear Outputs of All Cells`; VS Code: `Clear All Outputs` in the notebook toolbar; Colab: `Edit > Clear all outputs`). This reduces the file size and the likelihood of conflicts. Before exporting figures for your report, restart the kernel and re-run the notebook from top to bottom so every figure reflects the final code.

### Resolving Merge Conflicts

If a conflict does happen, `git pull` will tell you which files are affected.

* **For `.py` and `.md` files:** Open the file, find the sections between `<<<<<<<`, `=======`, and `>>>>>>>`, edit them to keep the correct version, delete the markers, then `git add` the file and `git commit`.
* **For notebooks:** Conflict markers usually break the notebook's JSON, so editing them by hand is error-prone. The simplest fix is to keep one person's version, `git add` and commit it, and then re-apply the other person's changes by hand.

### Using Google Colab with GitHub

Google Colab provides a great way for teams to work together without worrying about local Python environments.

1. **Opening a Notebook from GitHub:**
    * Open [Google Colab](https://colab.research.google.com/).
    * Go to `File > Open notebook`.
    * Select the **GitHub** tab.
    * Enter the repository URL (e.g., `https://github.com/UC-Berkeley-I-School/200-FA26-EDA-Climate-Change`) and press Enter.
    * Click on the notebook you want to open.

2. **Saving a Notebook to GitHub:**
    * After making your changes in Colab, go to `File > Save a copy in GitHub`.
    * You'll be asked to authorize Colab to access your GitHub account. To see your private team repository, check **Include private repos**; if it still doesn't appear, you may need to grant Colab access to the `UC-Berkeley-I-School` organization in your GitHub settings (Settings > Applications > Authorized OAuth Apps).
    * Choose the correct repository and branch from the dropdown menus.
    * Add a clear commit message describing your changes and click **OK**.

This method allows team members to easily access and contribute to the project from any machine with a web browser. Be aware that saving from Colab commits directly to the repository **without pulling or merging first**: if a teammate pushed changes to the same notebook after you opened it, saving will overwrite their work. Coordinate with your team so only one person edits a given notebook at a time, and reopen the notebook from GitHub before each work session.


## Example Project Structure

Below is a sample of how an EDA might be structured. This is not a prescriptive requirement, and your sections should change based on the dataset you've selected.


### 1. Introduction & Guiding Questions

* **Purpose:** Start here to set the stage for your analysis.
* **Content:**
    * Briefly introduce your chosen topic and why it's interesting.
    * State the primary dataset(s) you are using.
    * Clearly list the 2-4 main questions your analysis will explore. These questions will guide the rest of your report.

### 2. Data Preparation & Cleaning

* **Purpose:** Show how you got from raw data to the data you analyzed. As noted in **Document Everything** above, you must document your decisions, such as removing observations or transforming variables.
* **Content:**
    * **2.1. Describing the Data:** Describe your primary and any supplemental datasets: their source, size (rows and columns), and the key variables you use.
    * **2.2. Merging Datasets (if applicable):** If you joined multiple datasets, explain which columns you used to perform the join.
    * **2.3. Data Cleaning:** Detail the steps you took to clean the data. Be explicit.
        * Handling missing values (e.g., "We filled missing 'Age' values with the median age.").
        * Correcting data types (e.g., "The 'Date' column was converted to datetime objects.").
        * Addressing suspicious or outlier values, and justifying whether you kept or removed them.
    * **2.4. Feature Engineering / Transformation:** Explain any new variables you created or transformations you applied (e.g., "We took the logarithm of the 'Price' variable to reduce its right skew.").

### 3. Exploratory Analysis & Findings

* **Purpose:** This is the core of your report, where you build your written argument and tell a compelling story with your data.
* **Content:** Organize this section around the questions from your introduction, with one subsection per question.
    * **3.1. Analysis for Question 1: [Your First Question]**
        * Use text, tables, and visualizations to explore the data relevant to this question.
        * Characterize relationships between variables. For example, show a scatter plot and describe the relationship you observe.
        * **Every single figure must be explained in your text.** Describe what the chart shows and why it's important for answering your question.
    * **3.2. Analysis for Question 2: [Your Second Question]**
        * Repeat the process, using analysis and well-annotated figures to guide the reader through your findings.
    * **3.3+. Remaining Questions:** Add a subsection for each additional question.

### 4. Assumptions & Limitations

* **Purpose:** The presentation guidelines require you to discuss assumptions made during the analysis. Including them in the report demonstrates critical thinking.
* **Content:**
    * Briefly list any assumptions you made (e.g., "We assumed that the data collected in 2022 is representative of the entire prior year.").
    * Mention any limitations of your dataset or analysis (e.g., "Our dataset only included information from one city, so findings may not apply elsewhere.").

### 5. Conclusion

* **Purpose:** Summarize the key takeaways from your analysis.
* **Content:**
    * Briefly recap your main findings as they relate to your initial questions.
    * Conclude your data story. What is the final message you want the reader to take away from your exploration?

[signup]: https://docs.google.com/spreadsheets/d/1BK1E7BxYBo5eVU2Vq7N6vOaKiWkZ8tRKdSukUWAp4KM/edit
