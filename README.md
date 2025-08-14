To build MCP Server .
1. Download Claude Desktop from Anthropic portal and install it .
2. Set enviromental path of Claude Desktop , you will find it here . -->C:\Users\mihir\AppData\Roaming\Claude

4. Install uv.exe from pip install uv or the best run cmd/powershell command --> powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
5. After successfull installation of uv.exe set it vatiable path so you can use it in cmd .
6. Run uv init my-mcp-server to create a project directory
7. after creating directory  go to that directory ...via terminal/cmd and make command -----> uv sync ( this will install all dependencies for your mcp server)
8. Run uv add "mcp[cli]" to add mcp cli in your project
9. Few folks may get type errors for which you can run pip install --upgrade typer to upgrade typer library to its latest version.
10. Create Your Server file[filename.py] , Write code in filename which will include the tools and functions etc .. for instance in this project the server file is Main.py for leave management server
11. Run command in terminal ---> uv run mcp install main.py
   After running Above command you will get Response like Below --->
   <img width="784" height="240" alt="image" src="https://github.com/user-attachments/assets/7313831e-0e64-41d6-b9b8-f28c79ef0ba7" />
12. Now you will see claude_desktop_config.json file in [C:\Users\mihir\AppData\Roaming\Claude] directory.
13. Make sure you have claude_desktop_config.json file in above directory. if not set your tool will not be visible in claude desktop application .
14. Edit the file if its not proper configuration or you encounter the problem .


    -----------------> HOW TO CHECK IF  YOUR MCP SERVER WORKS OR NOT<----------------------------------------------
1. Kill any running instance of Claude from Task Manager. Restart Claude Desktop.
1. Go to Claude Desktop Application and in New Chat ask Query Like " Give me Employee Name/ID  Who is On Leave " it will ask you Employee ID or EMployee Name ?
2. Give The Employee Name /ID and it will return the response like below from MCP server it implies Your Server is Working .
   <img width="1920" height="1080" alt="Screenshot (424)" src="https://github.com/user-attachments/assets/4e40a7bb-3f3e-4d88-9514-3786af24909c" />

4. In Claude desktop, now you will see tools from this server
   <img width="828" height="396" alt="image" src="https://github.com/user-attachments/assets/9ed54463-8a71-4664-97e1-38ef8cfef545" />
Also ,

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/65ec65aa-f375-4795-894f-e10b2722d2fd" />


This AI tool helps an HR with leave management related tasks. The codebase here is for MCP server that interacts with mock leave database and responds to MCP client queries



Thank you ! 
Bhavik Vasava


