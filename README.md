# Read03

## Introduction:

In this reading we are going to talk about version control and more spacily aout a distributed version control Git .

## summary:
 1. What is a version control:
 2. GIT 
   2.1 Setting up a Git Repository
   2.2 cloning:
   2.3 Check File Status
   2.4 Tracking and Staging a New File
   2.5 Committing Changes
   2.6 Pushing Changes
   2.7 Remote Repositories


## 1. What is a version control:

Version Control is a system that allows you to revisit various versions of a file or set of files by recording changes.there is 3 kind of version control 
- Local Version Control:A Local VCS entails one database on your hard disk that stores changes to files.
- Centralized Version Control:This system entails a single server storing all changes and file versions, which can be accessed by various clients.
- Distributed Version Control: allows clients to create mirrored repositories. These data backups can be easily placed on the server to replace any lost information. Git is an exemple of a DCVS

## 2. GIT :

Git stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it.

## 2.1 Setting up a Git Repository

To import an existing project or directory into Git we have to follow these steps:
 Switch to the target project’s directory .Example:

   >$ cd test (cd = change directory)

Use the git init command

   >$ git init

To start tracking these repository files, perform an initial commit by typing the following:

   >$ git add *.c

   >$ git add LICENSE
        
   >$ git commit -m “any message here”

## 2.2 cloning:

You can also create a copy of an existing Git repository from a particular server by using the clone command with a repository’s URL: 

   > $ git clone https://github.com/test\

Or we can clone a repository into a directory with another name of your choosing, using:

   > $ git clone https://github.com/test mydirectory

## 2.3 Check File Status:

To determine the state of files, utilize the git status command:

   >$ git status

## 2.4 Tracking and Staging a New File:

Single File: Track one file only by using the following format:

   >$ git add filename

 All Files: Track all files in a repository by using the following command:

   > $ git add *

## 2.5 Committing Changes:

After staging one or multiple files, you should commit the changes and record what you did within the commit message:

   >$ git commit -m “made change x,y,z”

   >$ git commit -a

## 2.6 Pushing Changes:

push changes to a remote repository using the push message:

   > $ git push origin master

## 2.7 Remote Repositories:

By running the **git remote command**, you can view the short names, such as “origin,” of all specified remote handles.

By using git **remote -v**, you can view all the remote URLs next to their corresponding short names.

To create a new remote Git repository with a short name, use the following format:

   >git remote add shortname url

