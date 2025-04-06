### compiler_23115059
### 🟥 Area of Square TAC Compiler
This project is a simple compiler that takes square expressions in the form:

scss
Copy
Edit
square(side);
And it generates:

✅ Three Address Code (TAC)
⚙ Optimized Code to Compute Area
🖥 Area Output Using Register-Like Execution Flow

Built using Flex and Bison in C++, this compiler demonstrates how source code is broken down, compiled into intermediate code, and executed in a minimal register-based manner.

📥 Installation Guide (Windows with MSYS2)
🔧 Step 1: Install MSYS2 Terminal
👉 Download & install MSYS2 from the official site:
🔗 https://www.msys2.org/wiki/MSYS2-installation/
Make sure to follow all the setup instructions and initialize your environment properly.

🛠 Step 2: Install Required Tools
Open the MSYS2 terminal and run:

bash
Copy
Edit
pacman -Su                   # Update all packages  
pacman -S base-devel gcc     # Install base tools and compiler  
pacman -S flex bison         # Install Flex and Bison  
pacman -S git                # (Optional) Version control  
🛠 Build Instructions
Ensure flex, bison, and g++ are installed.

To compile the project, run:

bash
Copy
Edit
make
This will:

Generate lexer and parser files

Compile all source files

Output an executable: square

🚀 How to Use
Run the compiler like this:

bash
Copy
Edit
./square
Enter your square expression in this format:

c
Copy
Edit
square(5);
### ✅ Example Output
Section	Output
Input	square(5);
Three Address Code	
ini
Copy
Edit
t1 = 5  
t2 = t1 * t1  
Area = t2
| Final Output | Area value = 25 |

### Project Structure
bash
Copy
Edit
.
├── lexer.l         # Lexer (Flex)

├── parser.y        # Parser + TAC generation (Bison)

├── main.cpp        # Entry point

├── Makefile        # Build script

├── README.md       # You're here!
### ⚙ Optimization Potential
This compiler lays the foundation for more advanced optimization and parsing features. Ideas for future versions include:

Pattern	Future Optimization Suggestion
a * a	Constant folding, loop strength reduction
Input validation	Check for negative or invalid input
Variable support	Assign and reuse side variables
Control flow	Add support for conditional expressions
### 📸 Screenshots
You can add screenshots of the compiler's terminal output or generated TAC here for demonstration.
![Screenshot 2025-04-06 173811](https://github.com/user-attachments/assets/2935f652-71fd-4f79-9117-c95a368a60bd)


### 👨‍💻 Nithin Munavath
🎓 B.Tech CSE, NIT Raipur
🌐 GitHub: Nithin842
🔗 LinkedIn: Nithin Munavath

### 📜 License
MIT License – Free to use, improve, or extend!
