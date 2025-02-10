Below is the `.md` code for your GitHub README file:

```markdown
# Blood Donation Management System

## Main Objective
A portal that enables users to donate and receive blood at scheduled dates and times while keeping track of blood stock levels for various blood groups in hospitals.

---

## Features Implemented

### 🚑 **Donate Blood**
- 🩸 Schedule appointments to donate blood.
- 📅 Track scheduled donation appointments under the `Appointments` dropdown menu.
- ❌ Prevents users with permanent diseases from donating blood.
- 🤒 Restricts users with temporary conditions (e.g., flu, pregnancy) from donating blood.
- 🕒 Prevents users from scheduling appointments before the current date.
- 🚸 Restricts minors and senior citizens (>65) from donating blood.

### 🩸 **Receive Blood**
- 📅 Schedule appointments to receive blood.
- 🔍 Track scheduled receiving appointments under the `Appointments` dropdown menu.
- ⏳ Prevents scheduling appointments before the current date and within two days after the current date (to help with urgent blood requirements).
- 🏥 Limits the maximum blood units a recipient can receive to **10 units** (required for a total transfusion).
- ✅ Assigns appointments based on the compatibility table.
- ⚠️ If stock isn’t available at a selected hospital, prompts users to choose another hospital.

### 📅 **Appointments**
- `Appointments` dropdown menu allows users to track their scheduled appointments.

### ❓ **Help**
- Provides guidance on the program’s functionalities.

### 👤 **Profile**
- 🔐 Allows users to log in to their profiles.
- 🛠️ Enables users to update their profile details and change passwords.

### 🏠 **Home Page**
- 🎉 Displays a welcome message personalized with the user's name.
- 🏥 Shows information about all hospitals in a city, including their blood stock levels.
- 🔍 Filters displayed hospitals based on city, area, and hospital name selected in the combo box.

---

## 📊 Schema of the Tables

### 📌 **User Table**
- Stores user information collected during signup.
- **`UserId`**: Primary key (auto-generated).
- Other attributes are user inputs stored in the table.

### 🏥 **Hospitals Table**
- Stores hospital details.
- **`HosId`**: Primary key (manually assigned by the programmer).
- Other attributes are manually entered by the programmer.

### 🩸 **Donor Appointments Table**
- Stores scheduled donor appointments.
- **`DID`**: Primary key (auto-generated).
- **`UserId`**: Foreign key referencing the `UserId` in the **User** table.
- Other attributes are collected from user inputs and stored in the table.

### 🩸 **Recipient Appointments Table**
- Stores scheduled recipient appointments.
- **`RID`**: Primary key (auto-generated).
- **`UserId`**: Foreign key referencing the `UserId` in the **User** table.
- Other attributes are collected from user inputs and stored in the table.

---

📌 _This project aims to streamline the blood donation and transfusion process, ensuring efficiency and ease of access for users in need._
```
