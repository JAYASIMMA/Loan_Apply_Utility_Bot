## 💰 Loan Utility Bot — UiPath RPA Project

The **Loan Utility Bot** is an automated RPA solution built with **UiPath** to help financial institutions or admin teams process loan applications efficiently.
It reads loan application data, performs eligibility checks, calculates EMI, generates reports, and can send notifications automatically.

---

## 📌 Key Features

✅ Read loan application data from Excel, CSV, or Forms
✅ Validate applicant information (age, income, credit score, etc.)
✅ Calculate loan eligibility & EMI instantly
✅ Auto-generate approval/rejection letters (PDF/Word)
✅ Send email notifications to applicants (optional)
✅ Logs every transaction for audit

---

## 🗂️ Project Structure

```
LoanUtilityBot/
│
├── Main.xaml             # Entry point workflow
├── Inputs/               # Input files (applications, rules)
├── Outputs/              # Generated reports, letters
├── Assets/               # Templates (Word/PDF), config files
├── project.json          # UiPath project settings
├── Screenshots/          # (Optional) Demo screenshots
└── Documentation/        # (Optional) Extra docs
```

---

## ⚙️ Requirements

* **UiPath Studio** (2021.x or later)
* Excel/CSV input files
* Outlook or SMTP email access (if sending emails)
* Microsoft Word (if generating Word docs)

---

## 🚀 How to Run

1️⃣ **Clone the Repository**

```bash
git clone https://github.com/<YourGitHubUsername>/LoanUtilityBot.git
```

2️⃣ Open `Main.xaml` in **UiPath Studio**.

3️⃣ Place your input files in the `Inputs/` folder. Example: `loan_applications.xlsx`.

4️⃣ Update your configuration in the workflow if needed (interest rate, thresholds, email settings).

5️⃣ Click **Run** to execute the bot.

6️⃣ Generated reports and letters will be saved in the `Outputs/` folder.

---

## ⚙️ How it Works

1. **Read Applications** → Reads new loan requests from an Excel or database.

2. **Validate Data** → Checks mandatory fields (name, income, loan amount).

3. **Calculate EMI** → Uses a simple EMI formula:

   ```
   EMI = [P x R x (1+R)^N] / [(1+R)^N – 1]
   ```

   where P = loan amount, R = monthly interest rate, N = number of months.

4. **Generate Report** → Creates a PDF/Word letter for approval or rejection.

5. **Send Email (Optional)** → Mails the result to the applicant.

---

## ⚠️ Notes

* Make sure your input Excel has the required columns (e.g., `Applicant Name`, `Amount`, `Tenure`, `Interest Rate`, `Email`).
* Update your SMTP/Outlook settings if sending email.
* Test with sample data first to verify calculations.

---

## 📌 Example Input

**loan\_applications.xlsx**

| Name       | Amount | Tenure | Income | CreditScore | Email                                       |
| ---------- | ------ | ------ | ------ | ----------- | ------------------------------------------- |
| John Smith | 500000 | 60     | 75000  | 720         | [john@example.com](mailto:john@example.com) |
| Mary Adams | 250000 | 36     | 50000  | 680         | [mary@example.com](mailto:mary@example.com) |

---

## 🏷️ License

This project is licensed under the **MIT License** — feel free to use and adapt!

---

## 🙌 Author

**Your Name**
**Email:** jayasimmamomdad@email.com(mailto:jayasimmamomdad@email.com)

---

**Automate loan approvals in seconds!** 🚀
**Star ⭐️ this repo if you find it helpful!**

---
