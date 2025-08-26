
# GitHub Workflow for Course Materials and Submissions

This section provides a step-by-step guide on how to set up your GitHub repositories to manage course materials and submit your exercises.

## Step 1: Clone the Master Repository
First, clone the master repository where the course materials are hosted:

   ```bash
   
   # Clone the master repository (replace USERNAME with the instructor's GitHub username)
   git clone git@github.com:baracoma/meteo203-2526.git

   # Navigate to the cloned repository
   cd meteo203-2526
   
   
   ```

## Step 2: Set Up Your Own GitHub Repository
1. **Create Your Own Repository**:
   - On your GitHub account, create a new repository (e.g., `meteo203-2526-yourname`).

2. **Add Your Repository as a Remote**:
   - Add your newly created repository as a remote named `origin`:

   ```bash
   
   git remote rename origin upstream  # Rename origin to upstream (points to the master repository)
   git remote add origin git@github.com:YOUR_GITHUB_USERNAME/meteo203-2526-yourname.git  # Add your own repository as origin
   
   
   ```

## Step 3: Pull Updates from the Main Repository
To ensure your local repository is up to date with the latest course materials, pull updates from the master repository:

   ```bash
   # Navigate to the main repository
   cd meteo203-2526
   # Pull updates from the main repository (upstream) without affecting your work
   git pull upstream main
   
   
   ```

## Step 4: Work on Exercises and Push Submissions
1. **Create a Directory for Your Submissions**:
   - For each exercise, create a new directory under `submissions/` to store your files. For example:

   ```bash
   
   mkdir -p submissions/exercise_01
   
   
   ```

2. **Work on the Exercise**:
   - Complete your exercises within the created directory.

3. **Stage, Commit, and Push Your Work**:
   - Once you've completed the exercise, stage your changes:

   ```bash
   
   git add submissions/exercise_01/
   
   
   ```

   - Commit the changes with a descriptive message:

   ```bash
   
   git commit -m "Completed Exercise 01"
   
   
   ```

   - Push your changes to your GitHub repository:

   ```bash
   
   git push origin main


   ```
## Step 5: Update your README.md to log your recent updates.
Keep latest updates at the top. Suggested formatting of README.md
```markdown
## Date today (i.e. latest updates)
What you did today

## Date previous (i.e. previous updates)
What you did previous.


```