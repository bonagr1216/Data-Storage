### **Step 4: Test and verify data storage (test_data_storage.md)**

```markdown
# Step 4: Test and Verify Data Storage

1. **Create a Python file** for testing named `test_storage.py`.

2. **Write the test code**:

   from data_storage import add_item, list_items, remove_item

   add_item("Item 1")
   add_item("Item 2")
   add_item("Item 3")

   print("Current items:")
   list_items()

   print("\nRemoving Item 2...")
   remove_item(2)

   print("\nItems after removal:")
   list_items()
