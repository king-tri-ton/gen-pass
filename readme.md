
# Password Generator



https://github.com/king-tri-ton/gen-pass/assets/53092931/a581ebc1-f01f-4e7f-b4cb-a80fca51deb8



A simple password generator with a system tray icon. This Python script uses the **pystray** library to create a system tray icon. When the user clicks on the icon, it provides the option to generate a random password and copy it to the clipboard.



## Prerequisites
Make sure you have the required libraries installed:

```bash
pip install pystray Pillow pyperclip
```

## Compilation

To compile the script, you'll need to install PyInstaller first:

```bash
pip install pyinstaller
```

Then, you can use PyInstaller to create a standalone executable:

```bash
pyinstaller --onefile --noconsole --name="GenPass" --icon=C:\python\gen-pass\Logo.ico app.py
```

This will generate a standalone executable file named "GenPass.exe" without a console window.
## Usage

- Run the script.
- The script will create a system tray icon.
- Right-click on the icon to access the menu.
- Click on "Generate and copy" to generate a random password.
- The generated password is copied to the clipboard.
- Click on "Exit" to close the program.


## Customize

You can customize the password length and character set by modifying the **generate_password** function.

```python
def generate_password(length=12):
    # Customize the character set as needed
    all_characters = ['A', 'B', 'C', ...]
    password = random.sample(all_characters, length)
    password_str = ''.join(password)
    return password_str
```


## License

This project is licensed under the [MIT](https://choosealicense.com/licenses/mit/) License.

