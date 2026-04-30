# 🌐 Browser History Management System

<div align="center">

[![C++](https://img.shields.io/badge/Language-C%2B%2B-blue?logo=cplusplus&logoColor=white)](https://en.wikipedia.org/wiki/C%2B%2B)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Active-brightgreen)](https://github.com)
[![Version](https://img.shields.io/badge/Version-1.0.0-blue)]()
[![Terminal](https://img.shields.io/badge/Interface-Terminal%20Based-lightgray?logo=linux&logoColor=white)]()

A **powerful terminal-based browser history management system** written in C++. Manage, organize, and control your browsing history with advanced features including back/forward navigation, bookmarks, incognito mode, and more!

[✨ Features](#-features) • [🚀 Getting Started](#-getting-started) • [📖 Usage](#-usage) • [🎯 Commands](#-commands) • [🛠️ Technology](#️-technology)

</div>

---

## ✨ Features

### 🔗 **Navigation**
- ⬅️ **Back/Forward Navigation** - Navigate through your browsing history using stack-based implementation
- 📍 **Current Page Tracking** - Always know which page you're currently on
- 🎯 **Seamless Navigation** - Jump between pages with intuitive commands

### 📚 **History Management**
- 📋 **Full History Tracking** - All visited sites are recorded with timestamps
- 🔍 **Search History** - Search for specific URLs or keywords in your browsing history
- 🗑️ **Selective Deletion** - Remove unwanted entries from your history
- 📊 **Visit Statistics** - Track how many times you've visited each site
- 📈 **Session Summary** - Get detailed insights about your browsing session

### 🔖 **Bookmarks**
- ⭐ **Categorized Bookmarks** - Organize bookmarks into custom categories
- 🔐 **Password Protected** - Secure your bookmarks with password protection
- 📁 **Easy Organization** - Group related sites together for quick access

### 🎭 **Privacy & Security**
- 🕵️ **Incognito Mode** - Browse privately without recording history
- 🔒 **Password Protected Access** - Secure sensitive bookmarks
- 🛡️ **Data Control** - Complete control over your browsing data

### 💾 **Import/Export**
- 📤 **Export History** - Save your history to a CSV file
- 📥 **Import History** - Load history from previously saved files
- 📦 **Data Portability** - Easily backup and restore your browsing data

---

## 🚀 Getting Started

### Prerequisites

- **C++ Compiler** (GCC, Clang, or MSVC)
- **Standard C++ Library**
- **Terminal/Command Prompt**

### Installation

1. **Clone the repository** (or download the source)
   ```bash
   git clone https://github.com/yourusername/Browser-History-Management-Terminal-Based.git
   cd Browser-History-Management-Terminal-Based
   ```

2. **Compile the program**
   ```bash
   # Using GCC
   g++ -std=c++11 -o browserhistory browserhistorymanagement.cpp
   
   # Using Clang
   clang++ -std=c++11 -o browserhistory browserhistorymanagement.cpp
   
   # Using MSVC (Windows)
   cl browserhistorymanagement.cpp /Fe:browserhistory.exe
   ```

3. **Run the program**
   ```bash
   # Linux/macOS
   ./browserhistory
   
   # Windows
   browserhistory.exe
   ```

---

## 📖 Usage

Launch the program and you'll be greeted with an interactive menu:

```
==============================
Browser History Manager
==============================
1.  Visit Site
2.  Go Back
3.  Go Forward
4.  Show Current Page
5.  Show History
6.  Search History
7.  Bookmark Current Site
8.  Show Bookmarks (Password Required)
9.  Delete from History
10. Export History to File
11. Import History from File
12. Session Summary
13. Toggle Incognito Mode
0.  Exit
```

Simply enter the number corresponding to your desired action and follow the prompts.

---

## 🎯 Commands

| Command | Description |
|---------|-------------|
| **1** | Visit a new URL and add it to your history |
| **2** | Navigate back to the previously visited page |
| **3** | Navigate forward to the next page |
| **4** | Display the current page you're viewing |
| **5** | View your complete browsing history with timestamps |
| **6** | Search for a specific URL or keyword in history |
| **7** | Bookmark the current page under a custom category |
| **8** | View all bookmarks (requires password) |
| **9** | Remove a specific URL from your history |
| **10** | Export all history to a CSV file |
| **11** | Import history from a previously saved CSV file |
| **12** | Get statistics about your browsing session |
| **13** | Toggle private browsing mode |
| **0** | Exit the application |

---

## 💡 Example Workflow

```
1. Enter "1" → Visit "google.com"
2. Enter "1" → Visit "github.com"
3. Enter "1" → Visit "stackoverflow.com"
4. Enter "2" → Go back to "github.com"
5. Enter "5" → View all visited sites with timestamps
6. Enter "6" → Search for "github" → Displays matching history
7. Enter "7" → Bookmark "github.com" under "Development"
8. Enter "12" → View session summary with top visited sites
```

---

## 🛠️ Technology

### Built With
- **Language**: C++11
- **Data Structures**:
  - Stack (Back/Forward navigation)
  - Vector (History storage)
  - Map (Visit counting & categorization)
  - Set (Bookmark organization)

### Architecture Highlights
- 🏗️ **Object-Oriented Design** - Clean encapsulation using C++ classes
- 📊 **Efficient Data Structures** - Optimized for performance
- ⚙️ **Modular Methods** - Easy to extend and maintain
- 💪 **File I/O Operations** - CSV import/export support

---

## 📋 Features Breakdown

### Data Structures Used
```
├── Back Stack        → Previous pages for backward navigation
├── Forward Stack     → Next pages for forward navigation
├── History Vector    → All visited URLs with timestamps
├── Visit Map         → URL → Visit count mapping
└── Bookmarks Map     → Category → Set of URLs mapping
```

### Key Methods
- `visitSite()` - Record a new site visit
- `goBack() / goForward()` - Navigation control
- `showHistory()` - Display browsing history
- `searchHistory()` - Find URLs by keyword
- `bookmarkCurrentSite()` - Save bookmarks by category
- `toggleIncognitoMode()` - Enable private browsing
- `exportHistory() / importHistory()` - Data persistence

---

## 🔐 Security Notes

- **Default Bookmark Password**: `admin`
- 🔑 **Change the password** in the code for production use
- 🕵️ **Incognito Mode** doesn't record to permanent history
- 💾 **Exported files** are plain text CSV - handle with care

---

## 📈 Potential Enhancements

- [ ] GUI implementation using Qt or wxWidgets
- [ ] Database support (SQLite)
- [ ] Advanced analytics and visualization
- [ ] Multi-user support
- [ ] Encryption for sensitive data
- [ ] Browser extension integration
- [ ] Cloud sync capabilities
- [ ] Custom time-based filtering

---

## 🤝 Contributing

Contributions are welcome! Feel free to:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---
