# Run Figures 6 and 7

Use Windows with Python 3.10 or newer added to PATH and Smokeview installed in its default location.

In File Explorer, open the parent folder containing `CWALE_reproduction`. Type `powershell` in the address bar and press Enter.

First, paste these two lines to enter the code folder and install the required packages:

```powershell
Set-Location -LiteralPath '.\CWALE_reproduction'
python -m pip install -r '.\requirements.txt'
```

Then paste this complete line to read the original slices, recompute the fields, and generate the figures:

```powershell
python -X utf8 '.\run.py' --source '.\raw_data' --out '.\my_reproduction'
```

Let Smokeview open and close automatically without manual interaction. When finished, open `Figure6.png` and `Figure7.png` in the `my_reproduction` folder inside the code folder.

If you need to run the program again, change `--out '.\my_reproduction'` to `--out '.\my_reproduction_2'` in the command. The output folder must be new or empty.
