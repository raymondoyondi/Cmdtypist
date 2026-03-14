# Cmdtypist ⌨️

A lightweight, high-performance command-line typing tutor written in C. Designed for developers and terminal enthusiasts who want to sharpen their typing speed (WPM) and accuracy without leaving the console.



## 🚀 Features

* **Real-time Metrics:** Tracks Words Per Minute (WPM) and accuracy percentage as you type.
* **Guided Lessons:** Structured practice sessions to help you master specific key rows and patterns.
* **Minimalist Interface:** Zero distractions; just you and the code.
* **Lightweight:** Minimal dependencies and extremely low memory footprint.

## 🛠 Installation

### Prerequisites
* A C compiler (e.g., `gcc` or `clang`)
* `make` utility (optional, but recommended)
* Standard C libraries

### Build from Source
1. Clone the repository:
   ```bash
   git clone [https://github.com/raymondoyondi/Cmdtypist.git](https://github.com/raymondoyondi/Cmdtypist.git)
   cd Cmdtypist
   ```

2. **Compile the project:**
   ```
   gcc main.c -o cmdtypist
   ```
   
3. **Run the application:**
   ```
   ./cmdtypist
   ```
   
## 📊 How it Works
Cmdtypist calculates your performance using standard typing industry formulas:

**WPM Calculation:**
$$WPM = \frac{(\text{Total Characters} / 5)}{\text{Time in Minutes}}$$

**Accuracy:**
$$Accuracy = \left( \frac{\text{Correct Characters}}{\text{Total Characters}} \right) \times 100$$

## 📂 Project Structure

| File/Folder | Description |
| :--- | :--- |
| `main.c` | Entry point and core logic for the typing engine. |
| `lessons/` | (Planned) Directory containing text-based practice files. |
| `utils.h` | Helper functions for timer and terminal handling. |

## 🛠 Roadmap
- [ ] Add support for custom text file imports.
- [ ] Implement a "Ghost" mode to race against your previous high score.
- [ ] Add `ncurses` support for a more robust TUI.
- [ ] Save user progress to a local SQLite database or JSON file.

## 🤝 Contributing
Contributions are welcome! If you have ideas for new lessons or feature improvements:

1. **Fork** the Project.
2. **Create** your Feature Branch (`git checkout -b feature/AmazingFeature`).
3. **Commit** your Changes (`git commit -m 'Add some AmazingFeature'`).
4. **Push** to the Branch (`git push origin feature/AmazingFeature`).
5. **Open** a Pull Request.

## 📄 License
Distributed under the MIT License. See `LICENSE` for more information.
