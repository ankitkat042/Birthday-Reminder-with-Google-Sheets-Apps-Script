# 🎂 Birthday Reminder with Google Sheets & Apps Script

I used to forget birthdays, even for people I really care about. Of course, I remember birthdays of my closest ones, but I care for too many awesome people to remember them all!

So I built this little tool: a Google Apps Script that reminds me every day whose birthday it is. It’s simplea nd just works, and it can help you remember the birthdays of people you care about too :)

Feel free to use it, improve it, or suggest changes, I'm open to improvements!

---

## ✨ What It Does

- Checks a Google Sheet every day for birthdays.
- Sends you an email if it's someone's birthday today.
- If the year of birth is included, it tells you how old they’re turning!
- Automatically runs daily once you set it up.

---

## 📋 Sheet Format

Create or copy a Google Sheet with the following structure (start from row 2):

| Name        | Birthday    |
|-------------|-------------|
| Ankit Kumar | 01/01       |
| JD   | 15/05/1995  |
| AG | 07/08       |

>The script supports:
> - `dd/mm` (e.g., `15/05`)
> - `dd/mm/yyyy` (e.g., `15/05/1995`)
>
> Only `/` is supported as the separator (not `-` or `.`).

---

## 🚀 How to Use It

### 1. **Make a Copy**

Click here to make a copy of the sheet and the script:

👉 [Make a Copy of the Birthday Reminder Sheet](https://docs.google.com/spreadsheets/d/1A9AAklmdZuRYKLI6qgBKrTwoxiyzNZF0htsJcrh8lck/copy)


---

### 2. **Set It Up**

- Go to **Extensions > Apps Script**.
- The script is already loaded.
- Click the `main` function and click ▶️ **Run**.
- **Authorize the script when prompted (just once).**
- This lets it access your sheet and send you an email.

---

### 3. **Set Up Daily Reminder**

To automate it daily:

- In Apps Script, click the **Triggers** icon (⏱️).
![image-1](https://github.com/user-attachments/assets/28126bb9-778f-4b80-9ee2-35af1ed74ecc)
- Click **Create a new Trigger** in blue.
- Choose:
  - Function: `main`
  - Event source: `Time-driven`
  - Type: `Day timer`
  - ![image-2](https://github.com/user-attachments/assets/dcec9d59-8667-46dc-b869-2bb47b90c833)
- Save the trigger — done!

---

## 📬 What the Email Looks Like
![image-3](https://github.com/user-attachments/assets/bbf9f8b2-a147-4e3b-858a-454e0bd1d24c)


Now just add the list of birthdays in the spreadsheet and the script will handle everything else, but do not forget to run the script at least once to give permissions.

![image](https://github.com/user-attachments/assets/1feff4da-75aa-4310-8b2e-020b90c5b3b5)

