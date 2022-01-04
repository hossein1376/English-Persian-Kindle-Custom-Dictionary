Follow the instructions here and inside the content.html and dict.opf files. (You can use Notepad++ for editing them.)
Read the Amazon's own "Publishing Guide for Creating Dictionaries" if you need more insight.

# Content.html
Prepare your data based on the given structure and style. We're going to edit the strings between the <‌mbp:frameset‌> to the </mbp:frameset> tag.

Each entry starts with a <‌idx:entry‌> tag and ends by a </idx:entry> one.

Every entry will start by the <‌idx:entry name="default" scriptable="yes" spell="yes"‌> tag. You can change the "default" to any name you desire, especially if your dictionary contains sub-dictionaries for different entries.
Note: whatever name you choose for it, it must be stated exactly the same in the .opf file. You cannot change the other values of this tag.

The defined word/expression and its inflections are placed between the <‌idx:orth‌> and </idx:orth> tags.

Inflections are placed between the <‌idx:infl‌> and </idx:infl> tags. Each inflection itself is put between the two quotation mark inside the <idx:iform value=""‌> and it ends with the </idx:iform> tag.

The definition goes right after the </idx:orth> tag. I had inserted a <‌p‌> tag for better readability.

If you're working with a big database, I suggest breaking down the html file into smaller pieces for better and faster results.

# dict.opf
Edit the opf file and insert the dictionary name, the author name, input and output languages.

Reference the content.html file(s) in the manifest, spine and guide section based on the template.

Also, you can add cover image and more, follow the instructions inside the "Publishing Guide for Creating Dictionaries".

# Finishing the project:

Download and Install the Kindle Perviewer. (Put all the files you have just made inside a single folder.)
Open the .opf file with Kindle Perviwer and wait until the program does it's job.
(If it's taking unsually long or it was finished too quickly, there's a possiblity that something has gone wrong.)
Upon completion, you're going to be able to view your work. Finish your project by exporting it from File -> Export (ctrl+X in Windows) and export a .mobi file. Then, sideload it into your Kindle device.

Congratulations!

# Note:
While trying to export, it is possible to encounter an error and not be able to export your dictionary file.
Fear not. All you need to do is finding the Temp folder name and its location. For each book project, a unique folder will be created inside the path "C:\Users\You\AppData\Local\Temp\" directory.
You may find the folder's name by navigating to View -> Conversion log (ctrl+G in Windows), an exel file will be opened which will probably contain the path and the folder name.
The naming of the folder is something random like: 0c832824-e260-240d-a72f-193940d98a44. Checkout the date and time of the files inside each folder if you're still unsure.
Inside the aforementioned folder, there is your dictianory MOBI file named according your .opf file name. Treat the .mobi file as the exported result and sideload it into your device.
