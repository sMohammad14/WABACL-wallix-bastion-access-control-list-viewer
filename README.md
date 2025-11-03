# 🚀 WABACL (Wallix Bastion Access Control List viewer) - V2.0.1

## 🌟 Overview

This is a **Single-Page Application (SPA)** packaged as a single `.html` file. It runs **offline** in any modern web browser and **requires no installation**.

By importing the five essential CSV export files (**Authorizations**, **Resources/Targets**, **Target Groups**, **Users**, and **User Groups**), the application allows you to:

> 💡 **Visualize exactly what access** is granted: Which **User** has access to which **Resource/Server**, and under what conditions.

---

## 🛠️ How to Use

> It is recommended to carefully read the "📖 Full Guide to Application Features" section.

Follow these steps to generate the required data from your Wallix Bastion environment:

1.  In Wallix Bastion, go to the left menu → **Import/Export** → **CSV**.
2.  Set the separators **exactly** as follows (This is CRUCIAL for correct parsing):

> [!CAUTION]
> ### 🛑 REQUIRED Separator Settings
> **Field separator**: `;` (semicolon)
> 
> **List separator**: `,` (comma)

3.  In the export options, make sure to select the following sections:

> [!IMPORTANT]
> ### 📥 Mandatory Export Sections
> You **must** select these 5 sections to ensure all relationships can be established:
> 
> * **Authorizations**
> * **Devices** (or **Resources** or **Targets**)
> * **Target groups**
> * **User groups**
> * **Users**

4.  Export the data and unzip the downloaded `.zip` archive.
5.  Open the provided **`.html` file** in any modern web browser.
6.  **Drag and drop** the extracted CSV files into the application interface.

---

## ⚡ Quick Reference: Access Table

> It is recommended to carefully read the "📖 Full Guide to Application Features" section.

The **Access Table** lists every single granted access, regardless of group memberships.

### Key Features:
* **Sorting**: Supports simple and **multi-level** sorting on most columns.
* **Filtering**: Data can be instantly filtered by **User**, **Server**, **IP**, and **Authorization Name**.
* **Visualization**: Uses color coding in the 'No.' column to indicate the protocol integrity of the access.

### Color Status (Protocol Integrity):

| Color | Status | Meaning |
| :--- | :--- | :--- |
| **🟢 Green** | **Full Access** | The **entire set of protocols** allowed by the Authorization is fully supported and accessible on the Target Server. Access is **Clean**. |
| **🔴 Red** | **No Access** | The protocols allowed by the Authorization **do not align** with the protocols granted to the Target Server. Access is **Broken/Impossible**. |
| **🟡 Yellow** | **Partial Access** | A **mix** of accessible (Green) and inaccessible (Red) sub-protocols exists. Access is **Partial**. |

> [!NOTE]
> ### Sub-protocol Visibility
> By enabling the optional **Sub-protocols** column, you can see which protocols are **available** to the server entity (granted to the server AND allowed by the Authorization) **[Green color]** and which protocols are **not available** (NOT granted to the server entity but allowed by the Authorization) **[Red color]**.

### Crucial Logic:

> **The colors highlight conflicts:** An access record (row) exists because groups are linked, but the color indicates if the underlying **protocols match** between the server and the authorization object.

---

## 🔑 Key Features

* **Fully offline**: The application requires **no internet connection** after the initial download.
* **No installation needed**: Simply open the `.html` file.
* **Single-file deployment**: The entire project is contained in a **single `.html` file**.
* **Browser-native**: Runs directly in any modern web browser.
* **Wallix Integration**: Works seamlessly with exported **CSV files from Wallix Bastion**.

---

## ✨ Advanced Capabilities

* **Filter access data** by users, targets, IP addresses, and more.
* **Highlight targets with no assigned access**.
* **Highlight users with no assigned access**.
* **Toggle visibility of optional columns** (e.g., *Recorded*, *Critical*).
* **Multi-level column sorting** for detailed analysis.
* **Built-in dark mode support**.
* ...and more!

---

## 📖 Full Guide to Application Features

### 📥 File Reception Box

* Supports **Drag and Drop** functionality for files.
* **Validation and Identification**: Automatically confirms and identifies the content type of each dropped CSV file (e.g., 'Authorizations', 'Users').

### ⚙️ View Settings

| Setting | Description |
| :--- | :--- |
| **First Column** | Specifies whether the access listing should be based on **User** or **Server** (Resource). |
| **Show Access Type** | Defines how the access type (e.g., `Interactive`, `Account Mapping`) is displayed: **next to the server name**, in a **separate column**, or **hidden entirely**. |
| **Show Service Name** | Defines how the dedicated profile name for the server is displayed: **next to the server name**, in a **separate column**, or **hidden entirely**. |
| **User Detail** | Toggles whether user information is displayed or hidden when **hovering the mouse** over a username. |

### 🗃️ Data Filters

| Filter | Description |
| :--- | :--- |
| **Filter by Username** | Displays only the access entries related to **specific users**. |
| **Filter by Target/Resource** | Displays access granted to **specific servers** (based on server name). |
| **Filter by Host IP** | Displays access granted to **specific servers** (based on IP address). |
| **Filter by Authorization Name** | Displays only the access entries related to **specific Authorization** objects. |
| **Filter by Targetgroup** | Displays only the access entries related to members of **specific Target Groups** (Server Groups). |
| **Filter by Usergroup** | Displays only the access entries related to members of **specific User Groups**. |

### 👤 Ungrouped Entities

This box helps identify entities that are not part of any defined group:

| Section | Description |
| :--- | :--- |
| **Users without Usergroup** | Displays users who are **not members of any User Group**. The number in parentheses shows the total count of these users. |
| **Targets without Targetgroup** | Displays servers (based on name) who are **not members of any Target Group**. The number in parentheses shows the total count of these servers. |
| **Host IPs without Targetgroup** | Displays servers (based on IP) who are **not members of any Target Group**. The number in parentheses shows the total count of these servers. |

### ➕ Optional Columns

These options display additional details related to each access entry:

* **Recorded**: Does the access session get **recorded**?
* **Critical**: Is the access defined as **critical**?
* **Require approval**: Does the access **require approval** from other users?
* **Approver groups**: If approval is required, which **User Group** is responsible for approval?
* **Approvers**: If approval is required, which **specific Users** are responsible for approval?
* **Sub-protocols**: Which sub-protocols are allowed for this access? By enabling the optional **Sub-protocols** column, you can see which protocols are **available** to the server entity (granted to the server AND allowed by the Authorization) **[Green color]** and which protocols are **not available** (NOT granted to the server entity but allowed by the Authorization) **[Red color]**.

### 📊 Access Table

This section lists **every single access entry**, independent of User Groups and Target Groups.

#### Table Features:

* **Sorting**: All column headers can be sorted (Ascending or Descending), except for the 'No.' column which is sorted by color status.
* **Multi-Layer Sorting**: Supports multi-layer sorting with a numerical indicator showing the sorting priority of each column (Sort by Column A, then by B, then by C, etc.).

#### Color Definitions in the 'No.' Column:

| Color | Meaning | Explanation |
| :--- | :--- | :--- |
| **🟢 Green** | **Full Access** | All Sub-protocols of the Server for that row, which were granted by the Authorization of that row to the User of that row, are **accessible** by that user. |
| **🔴 Red** | **No Access** | All Sub-protocols of the Server for that row, which were granted by the Authorization of that row to the User of that row, are **NOT accessible** by that user. |
| **🟡 Yellow** | **Partial Access** | **Some** Sub-protocols (Green status) are accessible, and **some** Sub-protocols (Red status) are not accessible. |

> #### 🤔 **Why might this happen?**
>
> Consider a scenario: You have granted only an **RDP** protocol to a server, but the **Authorization** object linked to it allows **SSH** as well. Based on the group connection logic (Target Group linked to User Group), an access entry is created (a row in the final table). However, based on the protocol logic, the protocol granted to the server conflicts with the protocol allowed in the Authorization, making the access *de facto* impossible. **The colors clearly show this discrepancy.**

#### Unique Rows and Access Counter

The **Total rows displayed** section shows the number of records currently visible in the table (based on applied filters) out of the total number of access entries in the system.

