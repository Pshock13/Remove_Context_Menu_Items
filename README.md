# Remove_Context_Menu_Items
Simple .reg file used to remove some of those pesky context menu items

## How to use
1. Back up your current registry
    - Hit the Windows key or press the 'Start menu' button on your task bar
    - Start typing 'regedit.msc' to search for the Registry Editor
    - Press [Enter] or click 'Registry Editor' to open the Registry Editor
    - While in Registry Editor select 'File > Export' from the selection menu
    - In the window that opens, navigate to a location for back up, name you registry backup file whatever you'd like, and be sure to select 'All' as the option for 'Export Range'
    - Click 'Save'

    ---

2. Edit Remove_context_menu_items.reg
    - Right click on the downloaded file named 'Remove_context_menu_items.reg'
    - Click on the context menu 'Edit' (or you can edit in any text editor of your choosing)
    - Clicking 'Edit' will give you a security warning dialog box asking if you're sure you want to run this. Hit [Run]. This will not actually run the file, but rather it will open in notepad to edit.
    - Once in the editor you will find groups like '; `Share with Skype`'. This denotes what would show in the context menu. Under that, you will find registry key entries that handle that context menu item. If you want to remove that item, make sure the lines are not commented (there is no leading semicolon (;)). Should you wish to leave the context menu item, go ahead and add a semicolon (;) to the start of the lines in that group and they will be ignored when we run the .reg file
    - Save & Exit
    ---
3. Run Remove_context_menu_items.reg
    - Double click on the file Remove_context_menu_items.reg
    - Once again, you'll see the security warning, click [Run]
    - Now you may have a User Access Control window pop up, click [Yes]
    - And then one final warning stating that you are about to edit values that could cause components to stop working (which, in this case, is the intended outcome). Click [Yes]
    - You should end up at one final dialog stating that registry keys and values from the file have been added (or rather removed) to the registry

# Q & A
- Q:  I borked things and need to fix it
- A: You did back up your original registry like I said right? If you did, open registry editor and instead of going to 'File > export' select 'File > import' then navigate to and select the backup you created previously.