This is a repo that contains helping commands.

```
# utilsxl.py

from openpyxl import load_workbook, Workbook

def get_row_count(file_path, sheet_name):
    """Return the number of rows with data in the given sheet."""
    wb = load_workbook(file_path)
    sheet = wb[sheet_name]
    return sheet.max_row

def get_column_count(file_path, sheet_name):
    """Return the number of columns with data in the given sheet."""
    wb = load_workbook(file_path)
    sheet = wb[sheet_name]
    return sheet.max_column

def read_data(file_path, sheet_name, row, column):
    """Read the value from a specific cell."""
    wb = load_workbook(file_path)
    sheet = wb[sheet_name]
    return sheet.cell(row=row, column=column).value

def write_data(file_path, sheet_name, row, column, data):
    """Write a value to a specific cell and save the workbook."""
    wb = load_workbook(file_path)
    sheet = wb[sheet_name]
    sheet.cell(row=row, column=column).value = data
    wb.save(file_path)

def create_new_file(file_path, sheet_name='Sheet1'):
    """Create a new Excel workbook and save it."""
    wb = Workbook()
    sheet = wb.active
    sheet.title = sheet_name
    wb.save(file_path)

def get_all_data(file_path, sheet_name):
    """Return all data from a sheet as a list of lists."""
    wb = load_workbook(file_path)
    sheet = wb[sheet_name]
    return [[cell.value for cell in row] for row in sheet.iter_rows()]

def find_value(file_path, sheet_name, value):
    """Find the first cell matching the value. Return (row, column) or None."""
    wb = load_workbook(file_path)
    sheet = wb[sheet_name]
    for row in sheet.iter_rows():
        for cell in row:
            if cell.value == value:
                return (cell.row, cell.column)
    return None

```
