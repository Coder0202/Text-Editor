# Text-Editor
This is a Java Swing application that creates a simple graphical text editor. The program provides a window with a text area where a user can type and edit text, along with two buttons: Open and Save.

Here's a breakdown of what the code does:

GUI Components
JFrame: The main window of the application, titled "Text Editor."

JTextArea: The central component where the text is displayed and edited.

JScrollPane: Wraps the JTextArea to add scrollbars, allowing the user to view content that exceeds the window size.

JButton: Two buttons, Open and Save, are used to trigger file operations.

JPanel: A container for the buttons, placed at the top of the window.

BorderLayout: A layout manager that organizes the components within the window, placing the buttons at the top (PAGE_START) and the text area in the center (CENTER).

Functionality
The application implements the ActionListener interface, which allows it to respond to button clicks.

Open Button: When a user clicks the Open button, a JFileChooser dialog opens. This dialog allows the user to browse their file system and select a text file. The file chooser is configured to only show files with the .txt extension. If the user selects a file and clicks "Open," the program reads the content of that file and displays it in the JTextArea.

Save Button: When a user clicks the Save button, another JFileChooser dialog opens. This allows the user to choose a location and filename to save the current text. The file chooser is also set to suggest the .txt extension. The program then writes the content from the JTextArea into the specified file.

Both the open and save functionalities use Java's FileReader, BufferedReader, and FileWriter classes to handle reading from and writing to files. The code includes a try-catch block to handle potential IOException errors that may occur during file operations.

In essence, this program is a basic text editor with fundamental file-handling capabilities.
