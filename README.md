# HotShell
A set of tools for augmenting basic Unix commands, using Perl and Korn Shell
Introduction:
        The following is the User and Installation Guide for 
        HotShell.  Included are Software Requirements, Size, 
        Permissions, and internal manual pages needed by
        end-users for using HotShell.  For information on
        design aspects, see HotDesignDoc.txt, the design
        document for HotShell and its features.


Software Requirements:
        HotShell is meant to run on the Unix platform, and so, in order
        to invoke HotShell, the user needs to be running a common shell
        and know how to set the path to the HotShell directory to be
        able to call HotShell from anywhere.  The most common shells
        are Bourne, Korn and C Shells.  The installation guide below
        describes how to set your PATH variable in these shells.
        Moreover, since HotShell is written in Perl and Korn Shell,
        your Unix system must have Perl installed in
        /usr/local/bin/perl and Korn Shell in /bin/ksh.

        HotShell comes with its own files for hprint and htalk, so
        there is no need to have access to /etc/hosts and the global
        printers.conf file.  Standard Unix utilities are also required,
        such as ls, tar, uuencode, mailx, etc.  If when running
        HotShell, you notice that one of the commands will not work,
        try reading the man page for that command (all manual pages are
        also listed below) and look in the SEE ALSO section.  Often
        times, there may be a basic Unix command that is listed that
        you do not have on your system.  If this is so, ask your
        Systems Operator to install that command.

Size:
        HotShell requires 460K amount of space for the self-extracting
        installation file and about 212K amount of space for the HotShell
        directory and all file which will be in $HOME.  So, the user
        should allocate about 700K for the whole process, and once
        the installation file is removed, HotShell will require 
        about 300K of space to ensure that there is enough space
        for utilities such as hmail to store files. For more
        information on the installation process, see installation below.

Permissions:
        HotShell is designed to have read write and execute permissions
        for the $USER depending on the file type (scripts are
        executable and manual pages are readable.  Write permissions
        have been maintained for developers).  If the user, designated
        by $USER, installs HotShell in their own $HOME directory, they
        will have access to run all available HotShell functions and
        specifications.

Environment:
        The HotShell directory should be placed in the user's $HOME
        directory.  Within the $HOME/HotShell directory, there are
        three other visible directories:

        1.  hcmds contains all HotShell-specific commands.
        2.  hdesign contains this User Guide and the Design Document
        3.  hmangs contains all manual pages for HotShell (see also
        below)

        Additionally, $HOME/HotShell contains the hotshell executable,
        and all .hxxx files (.hothosts, .hotprinters, .htrash
        directory, .hmail).

        HotShell also has its own variables, as set up in .hotshrc upon
        load-up (see hotshrc below for more details), and it gets
        environmental variables from a built-in Perl hash, designated
        by the system.  However, the user can change the environment
        variables.  See the man pages for hotshell below as well as the
        Help section for more details on setting environmental
        variables.

Installation of HotShell
        The HotShell command, heds, was used to mail HotShell to you.
        See heds below for more information on distributing this
        package to others.  You may remember that the attached file
        also had an installation description at the beginning of it.
        Details are in the User Document.

	For instructions on how to run HotShell as well as
	a tutorial, there is a User Guide, HotUserDoc.txt,
	in the $HOME/HotShell/hdesign directory.  Also in
	this directory is the Design Document, HotDesignDoc.txt,
	for Unix tool developers.
