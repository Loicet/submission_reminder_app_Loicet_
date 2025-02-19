# Submission Reminder App

A Linux-Bash script-based reminder application designed to help students manage their assignments and submit them on time. It automatically tracks submissions and sends notifications to students who have missed or are about to miss their deadlines.

## Features

- **Automated Submission Tracking** – Scans the assignment file to identify students with pending submissions.
- **Custom Reminders** – Sends timely reminders for students with upcoming or overdue assignments.
- **Easy Setup** – Set up the application quickly with a single script.
- **Configurable Settings** – Update assignment details (names, due dates, etc.) easily through the configuration file.

## How to Install

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/Christian-Regnante/submission_reminder_app_Christian-Regnante.git
```

### 2️⃣ Run the Setup Script

Navigate to the `submission_reminder_app_Loicet` directory and execute the script to create the necessary environment and files:

Before running, grant execute permissions to the `create_environment.sh` script:

```bash
chmod +x create_environment.sh
./create_environment.sh
```

### 3️⃣ Start the Reminder App

After the setup is complete, navigate to the newly created directory and run the app:

```bash
cd submission_reminder_yourName
./startup.sh
```

## Application Explained

- **Reads Submission Data**: The `submissions.txt` file contains a list of students and their submission statuses.
- **Checks for Pending Assignments**: The app compares student records against the assignment requirements and generates reminders for those who haven't submitted their work.
- **Displays Reminders**: The script outputs a list of students who are missing their assignments.
- **Configuration**: Modify the `config.env` file to customize application settings.

## Configuration

You can update both the `config.env` and `submissions.txt` files to customize your inputs. Be sure to adjust the assignment details, student names, and due dates as necessary.

---

## Example Output

After running the `./startup.sh` script, the output will look like this:

```bash
Assignment: Shell Navigation
Days remaining to submit: 2 days
--------------------------------------------
Checking submissions in ./assets/submissions.txt
Reminder: Chinemerem has not submitted the Shell Navigation assignment!
Reminder: Divine has not submitted the Shell Navigation assignment!
Reminder: Christian Regnante has not submitted the Shell Navigation assignment!
Reminder: Hirwa Armstrong has not submitted the Shell Navigation assignment!
Reminder application executed successfully!
------------------------------------
