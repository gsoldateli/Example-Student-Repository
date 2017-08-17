# Command Line for Developers
# Exercises

___
## Beginner

##### 1. Write the command that will allow you to navigate to two directories above your current directory.

	Add your answer here

##### 2. Write the command and flag that will list all of the files and directories in your current directory.


##### 3.  Write the command and flag that will list all of the files and directories in your current directory in long-format.


##### 4.  Write the command and flag that will list all of the files and directories in your current directory, including hidden files.

##### 5.  Write the command that will create a folder in your current working directory and name it clean_code_examples.


##### 6.  Write the command to create a new file. Give the file a name and use the .txt extension.


##### 7.  Write the command that will output the contents of the file socks to buy.txt, located in your current working directory, to the terminal. Assume that either socks to buy.txt already exists, or create it yourself.


##### 8.  Write the command to display your Present Working Directory.

##### 9.  Write the command to output the current user to the terminal. The current user is generally the account that is logged into the operating system and currently using the terminal.


##### 10.  Write the command to list the files and folders of the folder two above your current directory. 


##### 11.  Write the command to create the file list of best cat pictures.html.


##### 12.  Write the command that will change your current directory to C:/Users/Default User/My Documents


##### 13.  Write the command that will ping the ip address 8.8.8.8


##### 14.  Write the command to change your current directory to the folder <HOME>/documents/, where <HOME> is the single character shortcut for $HOME.

##### 15.  Write the command to display the text “My name is ” followed by your first name.


##### 16.  Write the command that will show the output of two files, one after another: tylers favorite songs.txt and sarahs favorite songs.txt


##### 17.  Write the command to show the help, or manual, for the echo command, and add it to a file called echo_options.txt.


##### 18.  Write the command, flag, and flag option to ping 127.0.0.1 two times. A flag option is an option passed immediately after a flag.


##### 19.  Write a single command to display the contents of all Markdown files (that have the extension .md) to the console.

##### 20.  Write the command to remove the file yesterdays_todo_list.md from the directory you are presently working in.

## Intermediate

*Before you start working on this part of the project assignment, read Additional Commands in the coursework.*

### Intermediate Project 1

> Use only the command line to create 5 files (one at a time) and add full sentences to each, as illustrated below:

>- Create the file myname.md and write your name in it.
>- Create the file myfavoritefoods.md and write your three favorite foods.
>- Create the file dreamproject.md and write about a project that you would like to build after Modern Developer.
>- Create the file music.md and write the genre of music, song, or artist, that you feel most comfortable listening to.
>- Create the file colors.md and write your favorite color or colors.

	Your Answer Here

### Intermediate Project 2

> Find out which of the files that you wrote in the previous step had the largest file size. Write the command and the correct flags to list the files and their file size in human readable and long format. Then add the output to this file: **filesizes.txt**.

### Intermediate Project 3

> Let’s create a backups folder and backup the files we’ve written so far. Create a new directory and name it backups. Use the tar command to archive the contents of your commandline-practice folder. Name your archived file **backup1.tar** and save it inside your **backups** folder.

### Intermediate Project 4

> Create a file **sites.txt** using the **echo** command and add to it a list of your favorite websites, each on its own line. You’ll need to type the newline character **(\n)** and the **echo** flag that *enables interpretation of backslash escapes*.

### Intermediate Project 5

> Use **curl** to get the contents of study.moderndeveloper.com and store the contents inside a file, study.html. When you request the file, it will retrieve the web page of the first web server that responds, which, in this case, is a server that indicates when the web page has been relocated. This routine occurrence is called a **redirection**. You will learn more about server redirects in an upcoming course. Use the **-L** flag to follow the redirection and receive the correct page.

### Intermediate Project 6

> Use the **mv** command and **Command Escaping** to rename your backup archive. Navigate to the **backups** directory and rename your backup1.tar archive to the output of the **date** command. That is, whatever the output (the text) of the **date** command is, use that text as the new name for your **backup1.tar** file.

### Intermediate Project 7

> Use the **wc** command and the correct flag to determine how many words you wrote inside your **dreamproject.m**d file. If the file contains fewer than 20 words (the **if** is not programmatic), append another two sentences to the file. Use those two sentences to describe your dream project.

### Intermediate Project 8

> Use the **grep ** command to find all JavaScript files located inside your **study.html** file by searching for **“\\.js**“. Save the result to a new file, **javascripts.html**

### Intermediate Project 9

> Let’s find out the total number of words inside of the text files (**.txt**) that you created. Use the **cat** command to list all of the contents of the text files inside of your commandline-practice folder; then pipe (**|**) the output of the **cat** command to the word count program (**wc**).

### Intermediate Project 10

> Your workspace has undergone many changes since your last backup. Create another backup file using **tar** and the directions in exercise 3; name your backup **backup2.tar**. Let’s clear out the workspace. **find** all Markdown files, html files, and text files, and remove them by passing the **-delete** flag to your **find** command. Be careful to not delete your backups folder.


## Advanced 

*Use your newfound knowledge on shell scripts to conquer these advanced exercises. We want you to have more than just an adequate understanding of the command line; we want you to use the command line with confidence and proficiency.*

*Complete the exercises inside a new directory named scripts. Make scripts a directory inside your commandline-practice folder used for your intermediate exercises. Add the contents of each script that you write to your exercise.md file inside of your GitHub repository.*

### Advanced Project 1

> Create a script, titled **mdextract**, that will *extract*, or *expand*, a **tar** archive into a new directory. Extracting an archive reverses the archive process, re-creating the files that were originally passed to **tar**. Write **mdextract** to have two passed-in options: the path to the archive and the path where the archive will be extracted to. Use the **mkdir** command and any necessary flags to create the directory, if the directory does not exist.

> ##### Note: We have not discussed extracting archives. You will need to refer to tar‘s man or help pages to learn to do that. But don’t use Google to find the answer. The answer is right there in tar‘s man pages. Read it; you will see.

> The following illustrates how to use the mdextract script:

	$ ./mdextract path/to/archive.tar ./backup2

> The script should automate the following executions:

>1. **Echo** a one-line description of what your script is doing, such as “*Expanding path/to/archive.tar into ./backup2.*”
>
>2. Create a new directory named **backup2**, if the directory does not exist.
>
>3. Use the **tar** command to expand the **backup2** archive into the newly created **backup2** directory.
>
>4. **Echo** “done” to the terminal display.

	Your Answer Here
	
### Advanced Project 2
	
> Create a script titled **mdtemplate** that will create the file structure of a website. Write your **mdtemplate** script to have the following positional parameters:

>- **$1**, the name of a new directory where your template files will be created
>- **$2**, a title, which will be used inside your template **index.html** for HTML document title, and an **h1** tag

>Design your **mdtemplate** so that it creates the following files inisde of the new folder:
>
>- A **css** directory
>- An **images** directory
>- a **js** directory
>- A **style.css** file inside the **css** directory
>- A **main.s** file inside of the **js** directory
>- An **index.html** file, which should be a completely valid HTML5 document

> Include a CSS ruleset inside of **style.css**, and include an **h1** element inside of your **index.html**.

> The following is a usage example of the **mdtemplate** script.

	$ ./mdtemplate ./mysite 'Template Site Title'
	
> Good luck!

### Advanced Project 3

>Create a script named **web_bundler** that concatenates—or **adds** the contents of—all files of a specified type, from a specified directory, into a single file.
>Create web_bundler to have the following positional parameters:
>
>- **$1**, the name of the output file.
>
>- **$2**, the find pattern, which tells the script which file path to follow, and which file names to bundle. Examples of file patterns include *.html, *.txt, and template-*.
>
>Here’s an example of how to use web_bundler:
>
>	$ ./web_bundler bundle.js "./js/partials/*.js"
>	
>And don't forget: If you get stuck on this question, or any of the above questions, you can use our [QA Board](qa.moderndeveloper.com) to get help!