---
title: '02b Files'
documentId: 1S06GgaCmPzqv6eZy_XkGK-T21B3s7KZhjsrOnIMt8aA
revisionId: ALBJ4LtMDYIWy_WEPtFDUU8NCdwz0p16ydAR0ZDpfk4evVad20tmI2Ttp24KClG4sY2EdEpFTHynvpxtvgR3Ww
documentLink: https://docs.google.com/document/d/1S06GgaCmPzqv6eZy_XkGK-T21B3s7KZhjsrOnIMt8aA/
---
  
![image](../../../images/02b_Files/1.png)

<a id="h.5zmrgda33ct3" name="h.5zmrgda33ct3"></a>

## Files

_Suzanne Little, suzanne.little@dcu.ie_&nbsp;

In a computer system:

<!---->
- It must be possible to store large amounts of information \(data\).

- The information must survive the termination of the process using it.

- Multiple processes must be able to access the information concurrently.

Therefore a **file** is: 

<!---->
- a named section of disk \(but not necessarily contiguous …\) holding data.

- stored on disks or other media units.

- persistent \(i.e. not affected by process creation or termination\).

**File system**: a method for storing and organising computer files and the data they contain to make it easy to find and access them.

Files of one form or another are the most common way that computers store data. In fact from a computer’s perspective, most content is a file. 

The different file formats, sometimes indicated by the extension, are processed in different ways depending on the programme and their purpose. When you have data in files, it’s good to consider whether the file is:

<!---->
1. Text or binary.

2. Open or proprietary. 

3. Structured or unstructured. 

A simple way to distinguish between **text**&nbsp;and **binary**&nbsp;files is to open the file in a text viewer like Notepad or Gedit. In Figure 1 below, you can see a screenshot from trying to open a binary file \(a PDF file\) in a text viewer, it looks like complete nonsense\! But the proper programme \(a PDF reader like Acrobat\) is able to interpret the binary data and render or show the PDF document. Text files are easier to read using programmes and libraries. A binary file is simply a non\-text file and common file formats include PDFs and older Microsoft Office documents \(note: newer Microsoft Office documents use an XML based text format\).

![image](../../../images/02b_Files/2.png)

_Figure 1: Screenshot of binary file open in text viewer_&nbsp;

Another consideration when looking at data files is to identify those that may have a **proprietary**&nbsp;format. Proprietary formats belong to a company and usually require a specific programme to read and manipulate the contents. 

The most common **structured**&nbsp;or tabulated data format is CSV \([comma separated values](https://en.wikipedia.org/wiki/Comma-separated_values)\). This is a really useful format for data interchange as it is very simple and widely available as a format for reading or writing data from most programmes. There are limits with CSV and we will take a look at some of these in the exercises at the end of this section. You might also come across TSV or other variations where there is a different separator character used. Can you find out what TSV stands for?

Other text\-based structured data formats that you should be familiar with include:

<!---->
- JSON: JavaScript Object Notation is often used in web\-based APIs and is a compact way to record an object and attribute\-value pairs.

- XML: \(eXensible Markup Language\) is an abstract format to build structured text documents based around tags \(e.g., \<names\>\) to mark up a document. There are many common XML\-based formats \(e.g. YAML, ATOM, RSS\) and most programs can read or export these formats.

- \[[KML](https://developers.google.com/kml/documentation/kml_tut?csw=1)\]: \(keyhole markup language\) a specific XML\-based file format for geographic data used by Google in Google Maps.

- \(X\)HTML: the format used for web pages is more concerned with how to structure and view data \(text, links and images\) but sometimes you need to process data that may only be available in HTML format. 

Many database programs \(such as SQLite, MariaDB and PostgreSQL\) may use text files to store the data, e.g., DB, SQL. The programs are optimised to process, store and retrieve from these files but often they are text\-based and can be viewed and read by other programs. 

There are other specialist data formats \(for example, GDP and ASX\) some of which may require a specific programme or library to read. 

You might like to take a look at the [Wikipedia list of file formats](https://en.wikipedia.org/wiki/List_of_file_formats) to see just how many different variations there are\!

<a id="h.xxq9wpw0n4zo" name="h.xxq9wpw0n4zo"></a>

### File types \- there are many\!

You can sometimes tell from the file extension \(ie, the letters after the . in the file name\) but Linux is an extensionless system so it doesn’t rely on the extension to determine the file type.

<!---->
- Programs \(or applications\):

   - Machine Readable: class, exe, com, o, obj, a, dll

   - Source Code: java, c, cxx, h, hxx, pas, asm 

   - Human Readable \(interpretable scripts\): js, php, sh, bat, pl, py

   - Program data \(configuration files\): dat, cfg, rc, yaml, json

<!---->
- Data files

   - Database files: db, myd, myi

   - Documents for display or printing

      - Binary \(machine readable\) e.g. Word docs \(doc\), ps, pdf, rtf, dvi

      - Text \(human readable\):HTML docs \(htm, html, shtml\), xml, Office xml \(docx\), tex, txt

   - Multimedia files \(images, audio, video\) gif, jpg, jpeg, mpg, mpeg, avi, qt, mp3

   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

- Log files

- Archive or compressed files: tar, zip, 7z, gz, Z

**Almost everything on a system is actually a file** \- the documents, the programs, the printer, the monitor, etc.

<!---->
- a directory \(or folder\) is a special type of file with a list of file names and other information related to these files.

- special files: represent physical devices like disks, terminals, printers, networks, external drives etc.

<a id="h.i06tsgupq9lo" name="h.i06tsgupq9lo"></a>

### File names

<!---->
- Conventions vary from system to system

   - [Windows 10](https://docs.microsoft.com/en-us/windows/win32/fileio/maximum-file-path-limitation): 260 characters is the maximum length of a file path 

   - [Linux](https://askubuntu.com/questions/859945/what-is-the-maximum-length-of-a-file-path-in-ubuntu): 255 characters for a file name, 4096 characters for a file path

- Historically: 8 characters, a dot and a file extension due to earlier limit on length of name that could be stored.

   - E.g. fish.dat

- May be case sensitive \(Fish.dat is different to fish.dat on Linux\)

- File extension

   - MS\-DOS: 1 – 3 chars; Unix: variable

   - Sometimes just conventions; sometimes required \(e.g. C compiler\)

   - Examples: file.bak, file.c, file.dat file.doc, file.lib, file.man, file.obj, file.txt

File extension list \- [http://filext.com/alphalist.php?extstart=%5EA](http://filext.com/alphalist.php?extstart=%5EA)

<a id="h.ivxq405xuzfx" name="h.ivxq405xuzfx"></a>

### Linux

<!---->
- Everything is a file \(even directories, devices, configuration, libraries, data, etc.\)

- Linux is an _extensionless_ system

- It is also _case sensitive_&nbsp;
   - `$ ./program.txt   // run the file called program.txt`&nbsp;
   - `$ cat badname.obj  // display contents of badname.obj`&nbsp;
- Use `stat` or `file` to ask the file about itself

- Watch for “hidden” files that start with **`.`** Show them using `ls -a`.

<a id="h.34fr69i4mp0c" name="h.34fr69i4mp0c"></a>

### File operations

\(ie, what can you do to a file?\)

<!---->
- Create, delete, open, close, read, write

- Append \(only add data to end of file\)

- Seek \(repositions the pointer to the current position to a specific place in the file\)

- Get attributes \(e.g. Unix\), set attributes \(e.g. flags\)

- Rename

Python: explore the [os module](https://docs.python.org/3/library/os.html) or file objects \(`f = open(‘path_to_file’, ‘r’)`\)

<a id="h.juw44xun85d1" name="h.juw44xun85d1"></a>

### Line endings? 

In a plain text file, to tell the computer that a line of text doesn't continue forever, the end of each line is marked by a sequence of one or more invisible characters, called control characters. While there are many control characters for different purposes, the relevant ones for line endings are the carriage return \(CR\) and line feed \(LF\) characters.

Unfortunately, the programmers of different operating systems have represented line endings using different sequences:

<!---->
- All versions of Microsoft Windows represent line endings as CR followed by LF.

- UNIX and UNIX\-like operating systems \(including Mac OS X\) represent line endings as LF alone.

Therefore, a text file prepared in a Windows environment will, when copied to a UNIX\-like environment such as a NeSI cluster, have an unnecessary carriage return character at the end of each line. To make matters worse, this character will normally be invisible, though in some text editors it will show up as ^M or similar.

You can convert between UNIX or DOS using programs like `dos2unix` or `unix2dos` though good text editors like notepad\+\+, sublime etc will probably offer to handle it for you.

<a id="h.hkxk7dhful96" name="h.hkxk7dhful96"></a>

### File attributes

<!---->
- Type \(e.g, normal or directory\)

- Size \(blocks, bits, bytes etc.\)

- Creator \(or owner\)

- Activity

   - Creation time

   - Last access time

   - Last change time

- Permissions  → important\! Not having the correct permissions to read data in or to save data out can cause problems in your programming\!

   - Read \(r\), Write \(w\), Execute \(x\)

   - Owner, Group, Others

   - `chmod`&nbsp;to change permissions in Linux

Below is a screenshot of a Linux \(ubuntu\) shell showing some files \(`ls -l`\) and the result of the `file`&nbsp;and `stat` commands.

![image](../../../images/02b_Files/3.png)

<a id="h.zg1d55ed1q4y" name="h.zg1d55ed1q4y"></a>

### Directories

<!---->
- Hierarchical file systems

   - Concept of **root**&nbsp;directory \(/ or c:\), with levels of sub\-directories and then files

- Path names

   - **Absolute path name** consists of the path from the root directory to the file e.g. `/usr/ast/mailbox` \(in unix\)

   - **Relative path name**&nbsp;is when the path names are taken relative to the current \(working\) directory e.g. mailbox if the user is currently in `/usr/ast`&nbsp;
- 2 special entries:

   - . \(dot\): refers to the current directory  \[You’ve seen this in `git add .`\]

   - .. \(dot dot\): refers to the parent directory

   - E.g. `cp /usr/lib/dictionary .` \(unix\)

- Operations:

   - \(unix\) Create, delete, opendir, closedir, readdir, rename, link, unlink

<a id="h.ftt9m83885a2" name="h.ftt9m83885a2"></a>

### General Linux Directory Structures 

\[you don’t need to learn these\!\]

![image](../../../images/02b_Files/4.png)

<span style="font-size:10pt;">[http://www.thegeekstuff.com/2010/09/linux\-file\-system\-structure/](http://www.thegeekstuff.com/2010/09/linux-file-system-structure/)</span><span style="font-size:10pt;"> 
</span>

<a id="h.87sm7mv0vddu" name="h.87sm7mv0vddu"></a>

### Windows Directories

<!---->
- Variations between versions of Windows

- Typically called “folders”

- root equivalent is “C:\\ drive”

- Why C?

- Why \\ and not /?

- History:

   - [http://www.todayifoundout.com/index.php/2015/04/c\-drive\-default\-windows\-based\-computers\-2/](http://www.todayifoundout.com/index.php/2015/04/c-drive-default-windows-based-computers-2/) 

   - [https://www.howtogeek.com/181774/why\-windows\-uses\-backslashes\-and\-everything\-else\-uses\-forward\-slashes/](https://www.howtogeek.com/181774/why-windows-uses-backslashes-and-everything-else-uses-forward-slashes/) 

<a id="h.2r18m2416r1u" name="h.2r18m2416r1u"></a>

### Action: Common data science file types

<!---->
1. CSV \(& TSV & TXT\)

2. JSON

3. XLS or XLSX 

4. SQL

5. PDF

6. HTML

7. DOC or DOCX

8. HDF5

9. ZIP \(or GZ or TGZ\)

10. XML

<!---->
1. Can you identify the program associated with each? \(That is the programme that normally creates files of this type\)

2. Which of these file types do you know how to read into python? 

3. For each file type is it a binary or a text file?

<!--
<style>
th {
  font-weight: normal;
}
td {
  border: 2px solid black;
}
ol ol { 
  list-style-type: lower-alpha; 
}
ol ol ol { 
  list-style-type: lower-roman; 
}
img {
  max-width: 100%;
  height: auto;
  object-fit: contain;
}
</style>
-->
