# WABACL (Wallix Bastion Access Control List viewer)


## 📝 Description
A lightweight, offline tool delivered as a single HTML file that provides a clear, at-a-glance view of all created access permissions

 In the Wallix Bastion system, there is no unified view for access permissions, and you must manually inspect each user's individual access.  
 
This tool, which is fully contained in a single `.html` file, works completely `OFFLINE` and uses exported `.CSV'` files only from the system to display access lists either by user or by target.

## 🛠️ Usage

1. In **Wallix Bastion**, go to the left menu → **Import/Export** → **CSV**.

2. Set the separators **exactly** as follows:

```
Field separator: ;   (semicolon)
List separator: ,   (comma)
```

3. In the export options, make sure to select the following sections:

```
Authorizations
Devices (or Resources or Targets)
Target groups
User groups
Users
```

4. Export the data and unzip the downloaded `.zip` archive.

5. Open the provided `.html` file in any modern web browser.

6. Drag and drop the extracted CSV files into the application interface.


## 🔑 Key Features

- Fully `offline` — no internet connection required  
- No installation needed  
- Entire project contained in a single `.html` file  
- Runs directly in any modern web browser  
- Works with exported `CSV` files from Wallix Bastion


## ✨ Advanced Capabilities

- Filter access data by users, targets, IP addresses, and more  
- Highlight targets with no assigned access  
- Highlight users with no assigned access  
- Toggle visibility of optional columns  
- Multi-level column sorting  
- Built-in dark mode support
- and more...


## 🖼️ Screenshots

### Light theme
![WABACL first load light](screenshots/WABACL%20first%20load%20light.png)  
*WABACL first load light*


![WABACL data loaded light](screenshots/WABACL%20data%20loaded%20light.png)  
*WABACL data loaded light*


![WABACL data loaded and filtered light](screenshots/WABACL%20data%20loaded%20and%20filtered%20light.png)  
*WABACL data loaded and filtered light*


![WABACL data loaded and access type column light](screenshots/WABACL%20data%20loaded%20and%20access%20type%20column%20light.png)  
*WABACL data loaded and access type column light*



### Dark theme
![WABACL first load dark](screenshots/WABACL%20first%20load%20dark.png)  
*WABACL first load dark*


![WABACL data loaded dark](screenshots/WABACL%20data%20loaded%20dark.png)  
*WABACL data loaded dark*


![WABACL data loaded and filtered dark](screenshots/WABACL%20data%20loaded%20and%20filtered%20dark.png)  
*WABACL data loaded and filtered dark*


![WABACL data loaded and access type column dark](screenshots/WABACL%20data%20loaded%20and%20access%20type%20column%20dark.png)  
*WABACL data loaded and access type column dark*


## 📘 Full Feature Guide

### 🧭 View Settings

- **Data Grouping**  
  Choose how access entries are grouped: either by **User → Target** or by **Target → User**. This determines which column appears first in the table.

- **Target Source Display**  
  Configure how access types defined in **Target Groups** (e.g., *Interactive login*, *Account mapping*, etc.) are shown:
  - Inline next to the target name  
  - In a dedicated column  
  - Or hidden entirely


### 🔍 Data Filters

- **Filter by Username**  
  Display access entries for a specific user.  
  You can also choose to show **User Groups** that have access assigned but contain no actual users.

- **Filter by Target/Resource**  
  Display access entries for a specific server or resource.  
  You can also choose to show **Target Groups** that have access assigned but contain no actual targets.

- **Filter by Host IP**  
  Same as *Filter by Target/Resource*, but filters based on IP address.

- **Filter by Authorization Name**  
  Filter the table by specific authorization names.

- **Filter by Target Group**  
  Show only entries related to selected target groups.

- **Filter by User Group**  
  Show only entries related to selected user groups.


### 🧩 Orphaned Entities

- **Users with No Access**  
  Lists all users who have no access to any target.

- **Host IPs with No Access**  
  Lists all servers (by IP) that no user has access to.

- **Targets with No Access**  
  Same as above, but based on target names instead of IPs.


### 🧱 Optional Columns

You can show or hide additional fields related to **Authorizations**:

- `Recorded` — Indicates whether the session is recorded  
- `Critical` — Marks the access as critical  
- `Require approval` — Indicates if access requires approval  
- `Approver groups` — Lists the user groups that can approve this access  
- `Approvers` — Lists the individual users who can approve this access  
- `Sub-protocols` — Lists allowed sub-protocols for this access

> For better UX, the cells in `Recorded`, `Critical`, and `Require approval` are color-coded: **green** for enabled, **red** for disabled.


### 📊 Table Behavior & UI Tips

- Click any column header to sort the table ascending/descending by that column.
- You can select multiple headers to enable **multi-level sorting**. Each level is numbered beside the header.
- In the **bottom-right corner**, you'll see:
  - The total number of unique access entries
  - The number of entries currently visible after filtering
- In the **top-right corner**, you can toggle between **light** and **dark** themes.

