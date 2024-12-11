### **Step 2: Create the basic data storage program (data_storage_program.md)**

```markdown
# Step 2: Create the Basic Data Storage Program

1. **Create a Python File**:
   Create a new file named `data_storage.py` in your project folder.

2. **Write the Basic Code**:

   ```python
   import json
   import os

   DATA_FILE = "data.json"

   if not os.path.exists(DATA_FILE):
       with open(DATA_FILE, "w") as file:
           json.dump([], file)

   def load_data():
       with open(DATA_FILE, "r") as file:
           return json.load(file)

   def save_data(data):
       with open(DATA_FILE, "w") as file:
           json.dump(data, file)