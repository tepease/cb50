If you look at the file in the browser, however, you'll notice that nothing has changed. What's up with that?
The .md extension, or suffix, like any extension, is simply an instruction to your computer about how it should render the file's data. Maybe you've heard of files with different suffixes referred to as a *format*. That's because, much of the time, when you save a file as a certain format, the program you're using translates and *encodes* the data a certain way. It will expect all files with this suffix to share the same encoding, or format.

You can test this by creating a text file. You can do this in a simple text editor like Notepad or TextEdit, or for style points you can do it in vim, from your console. [Vim instructions](https://github.com/tepease/cb50/tree/master/projects/1/try-vim.md). Type a few words and save it as a .txt.

Now locate your new text file in File Explorer/Finder, and right click (or control click) it to 'open with' a more advanced word program like LibreOffice or Word. Once its open, make no changes, but save it as a .docx, odt or some other non-txt format. 
Now open your new file with Notepad / TextEdit.

Change the .txt suffix on your first file to the same suffix as your second one by editing its name in File Explorer / Finder or console (```mv myfile.txt myfile-1.newsuffix``` from the correct directory). Now open this one in Notepad / TextEdit.

Now double click both to open them with the default word program. Take some notes about what you think is going on here so we can discuss it next Thursday!
