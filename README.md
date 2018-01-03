# AutoHotKey Automation
Keyboard shortcuts to automate daily life using AutoHotKey scripts. Open websites, folders, start applications or expand custom abbreviations.
## Getting Started
### Synopsis
AutoHotKey is a powerful tool that can help automate any task that is done repeatedly on a computer. In this repo, I am only covering a portion of the tool based on how I use it in on my Windows PC to automate my daily tasks. The code in this repo is the current version of my script. 
### Prerequisites
There is no prerequisite knowledge needed to write AHK scripts. The only knowledge of AHK needed is to know the following set of Key combinations.
```
; use semi colons to comment
; # is Windows Key
; ! is Alt Key
; ^ is Control Key
; + is Shift Key
; & can be used between any two keys or mouse buttons to combine them into a custom hotkey
```
Any combination of the above keys along with the letter or numpad keys triggers a task to run. An example of the usage is provided in the **Code Example** section.
### AutoHotKey Installation
Install AutoHotKey from [their webiste](https://autohotkey.com/download/). Their docs are pretty concise, comprehensive and easy to follow. You can access them on [AutoHotKey Docs](https://autohotkey.com/docs/AutoHotkey.htm) link.
## Code Example
Below are a few examples of the code I used in the script with their description of what they do.
* For Web Links:
```
;Opens YouTube on your default browser with the combination -> Windows Key + y
#y::run, https://www.youtube.com
Return

;Opens my profile on GitHub.com on your default browser with the combination -> Windows Key + Alt + g
#!g::run, https://github.com/sinharaksh1t
Return
```
* For Folder Shortcuts:
```
;Opens the Dropbox folder of my local computer with the combination -> Ctrl + Shift + d
^+d::run, C:\Users\Rakshit Sinha\Dropbox
Return

;Opens the Downloads folder with the combination -> Windows key + q
#q::run, C:\Users\Rakshit Sinha\Downloads
Return
```
* For Starting Applications:
```
;Opens the Windows Camera application with the combination -> Alt + c
!c::run, microsoft.windows.camera:

;Opens the Windows Calendar application with the combination -> Windows key + c
#c::run, outlookcal:
```
* Abbreviation Expansions:
```
;Expands "btw" into "by the way" (without quotes)
::btw::by the way

;Expands "scanin" to "Scanner in = new Scanner(System.in);"
::scanin::Scanner in = new Scanner(System.in);

;This is a special script I use for Web Development. Easily import Bootstrap link simply by typing "bscss". an addition thing to note
;here is the :o: before the abbreviations to be used which removes any additional spaces after the expansion has taken place.
:o:bscss::<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">
```
## Motivation
On an average day, I spend about over 60% of my waking hours on my laptop. Being utterly uninterested in wasting my time doing common repeated tasks that I do each day, this idea of automation struck me. I dug deep into finding out the ways of achieving my needs and that's when I came across AutoHotKey. It has helped save quite a few hours of my life until now and it'll continue to save some more in the future.
If it helps you or you draw inspiration from this tiny project, consider giving it a star. :)
