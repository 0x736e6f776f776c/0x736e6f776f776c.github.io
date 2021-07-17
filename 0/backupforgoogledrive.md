# Backup for Google Drive
If you use a lot of Google Drives, you know what a hussle it can be to copy all your files from one place to another, especially if they're all in different folders. I had the same issue, and so I went and coded a small tool to make fast backups of full Drives or folders. You just give the program the info it needs, authenticate with your Google account, and you can sit back while all your files are being copied to your desired destination(s).

## What exactly does the program do, and why does it need access to sensitive data?
In order for the program to be able to view your files, make copies of them and place the copies in the given destiantion(s), you will have to give the program access to your files to do exactly that. In order for the program to make proper copies, it also needs access to the metadata of files in your Drives. The information is only used by the program in order to do its job, and the info is not collected by me and certainly not shared with anyone. For more information on the use of data, check the [Privacy Policy](https://sites.google.com/view/privacypolicybackupfordrive/home)

## How to use the program
If you wish to use the program, just go the program's [Github repository](https://github.com/techsnowowl/Backup-for-Google-Drive), scroll down, and you'll see the ReadMe with instructions on how to download and run the program.

## Important things to know about the program
- In order for the program to be able to copy the files from one place to another, the Google account you log in with must have access to said files, and it must also have the permissions to make copies, and move those copies to another Drive, if that's what you want to do.
- There's a smart backup feature build into the program. I've made this so that you can save what files you've already backed up, and in the future choose to leave those files out of the backup to avoid duplicates. The way this works is that the program will list all the id's of the files in a text(.txt)-file, and the next time it makes a backup and that file is selected as previous smart backup, it will check for every file whether or not it's in that file.
- If you're going to back up an entire Drive, and there are any trashed files, meaning files in the trashcan, present in that Drive, they will be backed up to the trashcan of the destination(s).
- You might already have noticed that I keep saying destination(s). This is because the program gives you the choice to backup your files to multiple destinations.
- One of the annoyances of copying by hand, is that the filename gets 'Copy of' get put in front of the filename of the copies. However, the copies made by this program will have the exact same name as the original files.
- The entire project is coded in Python 3. 
- As of now, all files get copied into the root of the chosen destination(s). That means the filestructure is not replicated, hence the original folders will not be there. This is something I plan to change in the future, but for now, this is just the way it is.

I hope you find this program to be useful. You can check out any of my other projects on [my Github page](https://github.com/techsnowowl). Have a nice day!
