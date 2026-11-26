# Practical 6

Source PDF: practical 6.rtf.pdf

--- Page 1 ---

Practical 6
Aim
To install Python inside a Virtual Machine (VM) and create and execute a simple Hello World
Python program using Command Prompt.



In this practical, Python is installed inside the Windows Guest OS running on VMware. After
installation, a Python file with the .py extension is created using Command Prompt and opened
directly in Notepad. A simple Python program is then written, saved, and executed through
CMD.

Basic Working Flow

Host Computer
         ↓
VMware Workstation
         ↓
Windows Virtual Machine
         ↓
Install Python
         ↓
Create .py File
         ↓
Write Python Program
         ↓
Run Using CMD
         ↓
Display Output


3. Requirements

   •   VMware Workstation

   •   Windows Virtual Machine

   •   Internet connection inside VM

   •   Python

--- Page 2 ---

•   Command Prompt



4. Procedure

Step 1: Start the Virtual Machine

   1. Open VMware Workstation.

   2. Select the Windows Virtual Machine.

   3. Click Power On.

   4. Wait for Windows to start.



Step 2: Download Python

Open the official Python website:

Python Downloads- python.org

Download the latest Python version for Windows.



Step 3: Install Python

   1. Open the downloaded Python installer.

   2. Select Add python.exe to PATH.

   3. Click Install Now.

   4. Wait for the installation to complete.

   5. Click Close.

Important: Selecting Add python.exe to PATH allows Python to be executed directly from CMD.



Step 4: Verify Python Installation

Open Command Prompt.

Run:

python --version

--- Page 3 ---

Example output:

Python 3.x.x

This confirms that Python has been successfully installed.



5. Create Python File Using CMD

Step 6: Go to Desktop

cd Desktop

Step 7: Create and Open the Python File

notepad hello.py



Step 6: Write the Python Program

Enter the following program in Notepad:

print("Hello World")

Save the file using:



Step 7: Run the Python Program

In CMD, type:

python hello.py

Output:

Hello World



 Complete Command Sequence

For the practical demonstration, the main CMD commands are:

python --version

cd Desktop

notepad hello.py

--- Page 4 ---

After writing and saving the program:

python hello.py



 Result

Python was successfully installed inside the Virtual Machine. A .py file was created and
opened using CMD, a simple Hello World program was written, and the program was
successfully executed using Command Prompt.
