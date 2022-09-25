# Manual Registry Edit

Here are the steps for bringing back the older style right click menu.

Open the registry editor and navigate to

```Computer\HKEY_CURRENT_USER\Software\Classes\CLSID```

**_Alternatively_** you can use `win+r` and type `regedit` click `enter` and `ok`

#### Create a new key using this text:

```{86ca1aa0-34aa-4e8b-a509-50c905bae2a2} ```

From this new key, create another key named `InprocServer32`

Double-click on Default on the right pane. Then click on OK without changing any values

# Shell Script Auto Registry Edit
run shell script as Admin or copy and paste code into an Adminstrator command prompt or shell program. 

```
reg add "HKCU\Software\Classes\CLSID\{86ca1aa0-34aa-4e8b-a509-50c905bae2a2}\InprocServer32" /f /ve
```

After running or manually configuring open up Task Manager find "File Explorer" and click "Restart" or Reboot your PC.

---

with love, sweet.
