---
layout: post
title: notes2
date: 2017-05-16 11:09:33
tags:
---

programming notes of the past weeks :  

copy and paste pwd form command line:  
pwd | pbcopy --> to copy current dirctory to clipboard
then cd $(pbpaste) --> to cd in different terminal

## Copying when sshed in
commandThatMakesOutput | ssh desktop pbcopy

Source: http://stackoverflow.com/questions/1152362/getting-items-on-the-local-clipboard-from-a-remote-ssh-session

## scroll up in terminal:  
shit + fn upkey (page up)

## iTerm2 command overlord
command + shift + i = send commmand to all terminal windows

## Webstorm
command 1 = project view
command 2 = favorites
command 3 = search thingy
esc 	  = return to editor

## Mongo - 'the mongo shell speaks js'
db.quotes.find({'drivers.lName':'King'}, {'policy.clutchQuoteType':1})

JSON.stringify

decodeURIComponent(query that returns stringified stuff)

## `npm test`
exit status 0 is added to the end of npm test calls

Use `; exit 0` to replicate this for other npm scripts.

source of info and link to code source: http://stackoverflow.com/questions/23286017/npm-error-elifecycle-while-running-the-test

## `grep` files with regex 

grep -c -F /\**
grep  ^\ *function

grep options
-c count
-F fixed string

control-R to search command history!!

## Broken Fetch?
git config remote.origin.fetch "+refs/heads/*:refs/remotes/origin/*"

## Running in background
node server.js >std.txt  2>err.txt &

src: https://kb.iu.edu/d/afnz

## Timestamp in name
$(date +%s)

## What does /etc stand for?
http://www.aboutlinux.info/2007/03/what-does-etc-stands-for-in-linuxunix.html

## JSON Pretty print curl response:
json_pp

## PM2
pm2 start trafficcontroller.json --only s2