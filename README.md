# pdf-parser-app
Parsing an invoice pdf and matching data from a SQL Server

# Problem
Existing import tool
- Macro (written in VB)
- connects to local SQL Server
- Takes an PDF file
- use PDF2HTML executable and parses the pdf
- based on the parsed text, it looks up the information by executing SQL queries and tries to find existing data.
- If exists, it will update certain data elements, else create new data entries into SQL Server
- If there are errors, programs shut down and doesn't tell the error
- This fails the import and user has to manually import the data

# Requirement
- Show better error messages
- Fix the import tool's logic so it parses correctly

# Approach
- Reqwrite the tool in a better high level programming language with better UI
  # Questions
  - Which lirary to use for parsing PDF ?
  - How to connect to SQL server, execute CRUD operations ? 
  
  # Options
  - Python has notebooks, pdf extracting libraries, can share libraries easily
  - Supports connecting to SQL Server
  - C# natively connects to SQL, but no good pdf parsing libraries


# Backend
- Need 
-
