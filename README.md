pm10bp-tools
============

Git tools for Pacemaker-1.0 backporting

Managing the backport status of each commits using git notes.

* bin/git-bpstatus
  add/modify/delete status and memo
* bin/git-bplog
  print backport status and short log in one line
* bin/git-bpmkpatch
  a wrapper for git-format-patch

setup for using git notes

    git config --add remote.origin.fetch +refs/notes/*:refs/notes/*
    # TODO: add push default refspecs
    git config --add remote.origin.push refs/notes/*:refs/notes/*
    git config --add notes.displayRef refs/notes/backport-1.0-*
