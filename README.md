### Question 2: Git LFS Integration (Total: 10 Points)  
1. Create a branch `lfs`.  
2. Upload a large file (>200MB) and track it using Git LFS.  
3. Push the file to the repository.  
4. Clone the repository on another machine to verify the file is downloaded correctly.  

### Steps Involved:
## Step 1: 
A. Enable Git LFS by running the following command in the terminal:
    ```bash
    git lfs install
    ```
    
B. Create the `lfs` branch by running:
    ```bash
    git checkout -b lfs
    ```
## Step 2:
A. Upload the file and track it using Git LFS:
   - We can replace "*.ext" with your file type or specific file name:
     ```bash
     git lfs track "*.ext"  
     ```
    
B. Ensure the file is tracked by Git LFS using:

   ```bash
   git lfs ls-files
   ```
C. Make sure .gitattributes is tracked:

    ```bash
    git add .gitattributes
    ```
## Step 3:
A. Push the changes to the repository:
   ```bash
   git push origin lfs
   ```

### Step 4:
A. `Clone the repository on another machine to verify the file is downloaded correctly:`

    1. `Clone the repository using:`
       ```bash
        git clone https://github.com/<your-username>/git_assignment_HeroVired.git
        ```

    2. `Navigate to the repository folder:`
        ```bash
        cd git_assignment_HeroVired
        ```

    3. `Switch to the `lfs` branch:`
        ```bash
        git checkout lfs
        ```

    4. `Pull the branch to ensure Git LFS downloads the large file:`
        ```bash
        git pull
        ```
