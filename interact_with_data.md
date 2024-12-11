### **Step 3: Implement functions to interact with the data (interact_with_data.md)**

```markdown
# Step 3: Implement Functions to Interact with the Data

1. **Update the `data_storage.py` file**:

   def add_item(item):
       data = load_data()
       data.append(item)
       save_data(data)

   def list_items():
       data = load_data()
       if not data:
           print("No data available.")
       else:
           for i, item in enumerate(data, start=1):
               print(f"{i}. {item}")

   def remove_item(index):
       data = load_data()
       try:
           data.pop(index - 1)
           save_data(data)
           print(f"Item {index} removed successfully.")
       except IndexError:
           print("Invalid index.")
