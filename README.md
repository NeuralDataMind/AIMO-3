Here are the final steps to deploy your **Specialist SC-TIR Solver** to the AIMO 3 leaderboard.

### 📋 Step 1: The Setup Checklist
Before hitting save, ensure your Kaggle Notebook settings are correct:
* **Accelerator:** Set to **GPU T4 x2** (or whatever GPU quota you have available).
* **Internet:** Set to **OFF**. (Competition rules require this).
* **Input:** Ensure **`AI-MO/NuminaMath-7B-TIR`** is added in the right sidebar.
    * *Path Check:* The code expects `/kaggle/input/math_numina_7b_tir/pytorch/default/1/NuminaMath-7B-TIR`. If your added model has a different path name (e.g., just `numinamath-7b-tir`), update `MODEL_PATH` in the code to match.

### 🚀 Step 2: The Code
Ensure the `main.py` file in your editor contains the **final version** we just polished. It must include:
1.  `SpecialistAIMO3Solver` class.
2.  `identify_topic` (The Router).
3.  `run_python_code` with the **Auto-Print Fix**.
4.  `solve` method using the **Manual Chat Template** (`<|user|>...`).

### 💾 Step 3: Save & Commit
This runs your code from top to bottom to generate the submission file.
1.  Click the **"Save Version"** button (top right corner).
2.  Select **"Save and Run All (Commit)"**.
3.  Click **"Save"**.
4.  *Wait.* It will run the "Local Test Mode" (calculating factorial, etc.) and then generate the `submission.csv`. This might take 5-10 minutes.

### 🏆 Step 4: Submit
Once the version finishes saving:
1.  Click on the **Version Number** to open the Viewer.
2.  Scroll down to the **Output** section.
3.  You should see `submission.csv`.
4.  Click the **"Submit"** button next to it.

### 🔮 What happens next?
Kaggle will take your code and run it against the **Hidden Private Test Set** (50 problems).
* **Runtime:** Expect it to run for **2-5 hours** (depending on how many retries it triggers).
* **Score:** You will see a score on the leaderboard once it finishes.

**You are cleared for launch. Good luck!** 🚀
