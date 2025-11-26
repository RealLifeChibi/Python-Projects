# ✅ **Step-by-Step Plan**

## **STEP 1 — Set Up Your Project**

- Create a folder for the project
- Create a Python file: `habit_tracker.py`

---

## **STEP 2 — Plan Your Data Structure**

Start simple.

Store habits in a **list of dictionaries**, for example:

`habits = [     {"name": "exercise", "completed": False},     {"name": "read", "completed": True} ]`

Later, you can upgrade to classes if you want.

---

## **STEP 3 — Build a Menu System**

Your program should show options like:

`1. Add a habit 2. Mark habit as completed 3. View habits 4. Save and quit`

Use a `while True:` loop to keep the app running until the user quits.

---

## **STEP 4 — Add "Add a Habit" Feature**

- Ask user for a habit name
- Create a dictionary
- Add it to the list

Practice: input(), append(), loops.

---

## **STEP 5 — Add "Mark Habit as Completed" Feature**

- Show numbered list of habits
- Ask user which habit they completed
- Set `completed = True`

This reinforces indexing and updating dictionaries.

---

## **STEP 6 — Add "View Habits" Feature**

Print each habit and its status:

`exercise — completed read — not completed`

Good practice for loops and formatting.

---

## **STEP 7 — Save Data to a File**

Use JSON so it’s easy:

### Saving:

`import json with open("habits.json", "w") as f:     json.dump(habits, f)`

### Loading:

`with open("habits.json", "r") as f:     habits = json.load(f)`

This teaches file handling — a real-world skill.

---

## **STEP 8 — Reset Completion Daily (Optional)**

When the app launches:

- Check if the last saved date is today
- If not, reset all `completed` to False

You’ll learn about `datetime` here.

---

## **STEP 9 — Add Stretch Features (If You Want More Challenge)**

### ⭐ Track streaks

`{"name": "exercise", "completed": False, "streak": 4}`

### ⭐ Add weekly stats

How many habits completed in the last 7 days?

### ⭐ Export to CSV

Great practice with Python’s `csv` module.

### ⭐ Turn it into a GUI later

Use Tkinter or PyQt once you’re comfortable.
