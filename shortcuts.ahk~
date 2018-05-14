; BBG keyboard mapping:
	; Search -> F13
	; Cmnd History -> F15
	; Codes & Favourites -> F16
	; News -> F17
	; Quote Line -> F19
	; Quote Function -> F20
	; Message -> F21
	; IB -> F23
	; Menu -> F24
	; 1/16 -> F14
	; 1/32 -> F18
	; 1/64 -> F22
	; Panel -> <C-F24>

sharepoint= https://shp.swissre.com/sites/finace/ntp/Collateral Team Dox

; Numpad Keys

; https://shp.swissre.com/nepsearch/Pages/Results.aspx?k=S16RZM

ResizeWin(Width = 0,Height = 0, X=0, Y=0)
{
  WinGetPos,Xr,Yr,W,H,A
  If %Width% = 0
    Width := W

  If %Height% = 0
    Height := H

  If %X% = 0
    X := Xr

  If %Y% = 0
    Y := Yr
  WinMove,A,,%X%,%Y%,%Width%,%Height%
}

^Numpad0::
SetTitleMatchMode, 2
IfWinExist laser
    WinActivate laser
else
run, \\CHRB1025.CORP.GWPNET.COM\homes\7\S3QH78\Documents\L_Laser\mk_laser_v3.jar
return  

^Numpad1::
SetTitleMatchMode, 2
IfWinExist ahk_exe OUTLOOK.EXE
    WinActivate ahk_exe OUTLOOK.EXE
else
run, "C:\ProgramData\Microsoft\Windows\Start Menu\Programs\Microsoft Office 2013\Outlook 2013.lnk"
return    

^Numpad2::
IfWinExist, Apex Collateral
{
    WinActivate 
; ResizeWin(2000, 1500, 1672, 0)
}
; 	ResizeWin(1696, 1066, 1672, 0)
;IfWinExist, Alert
;    WinActivate
return

^Numpad3::
Run %UserProfile%/Documents
return

^Numpad4::
;explorerpath:= "explorer /e," https://shp.swissre.com/sites/finace/ntp/Collateral Team Dox
;Run, %explorerpath%
IfWinExist, Collateral Team Dox - All Documents - Internet Explorer
{    WinActivate
	 return
}
IfWinExist, Home - Collateral Management - Internet Explorer
{    WinActivate
return
}
IfWinExist, Presentations - Topic - Internet Explorer
{    WinActivate
return
}
run % "iexplore.exe" ( winExist("ahk_class IEFrame") ? " -new " : " " ) sharepoint
;Run https://shp.swissre.com/sites/finace/ntp/Collateral Team Dox
return

^Numpad5::
IfWinExist, [PRODUCTION] Order Management - Version
    WinActivate
IfWinExist, Alert
    WinActivate
return

^Numpad6::
SetTitleMatchMode, 2
IfWinExist ahk_exe EXCEL.exe
    WinActivate
return

^Numpad7::
InputBox, SearchTerm, Search Intranet,Search:
if not ErrorLevel
{
    if SearchTerm <> ""
        Run https://shp.swissre.com/globalsearch/Pages/results.aspx?k=%SearchTerm%
}
return

::/leo::
InputBox, SearchTerm, Search Leo,Search:
if not ErrorLevel
{
    if SearchTerm <> ""
        Run https://dict.leo.org/german-english/%SearchTerm%
}
return

^Numpad8::
SetTitleMatchMode, 2
IfWinExist, AAA Rich's  Favourite
{WinActivate
    WinActivate, AAA Rich's  Favourite
}
return

^Numpad9::
ifwinexist, ahk_class CabinetWClass
{
loop
{
winclose, ahk_class CabinetWClass
IfWinNotExist, ahk_class CabinetWClass
{
EXIT
}
}
}
EXIT

^!Numpad1::
SetTitleMatchMode, 2
IfWinExist ahk_class CommunicatorMainWindowClass
    WinActivate ahk_class CommunicatorMainWindowClass
return

!Numpad1::
SetTitleMatchMode, 2
IfWinExist Inbox - Michael_Kilchenmann@swissre.com - Outlook
    WinActivate Inbox - Michael_Kilchenmann@swissre.com - Outlook
IfWinExist ahk_class rctrl_renwnd32
    WinActivate ahk_class rctrl_renwnd32
return

^+q::
SetTitleMatchMode, 2
IfWinExist ahk_class rctrl_renwnd32
    WinActivate ahk_class rctrl_renwnd32
return

^!Numpad2::
SetTitleMatchMode, 2
IfWinExist ahk_class LyncConversationWindowClass
    WinActivate ahk_class LyncConversationWindowClass
return

^!Numpad3::
SetTitleMatchMode, 2
IfWinExist ahk_exe chrome.exe
    WinActivate ahk_exe chrome.exe
return

^!Numpad4::
SetTitleMatchMode, 2
IfWinExist ahk_class CabinetWClass
    WinActivate ahk_class CabinetWClass
return

^!Numpad5::
SetTitleMatchMode, 2
IfWinExist, TweetDeck - Google Chrome
    WinActivate
return

; Mixed Hotkeys

^+e::
IfWinExist, Trades, AladdinView - BlackRock Solutions - Internet Explorer
    WinActivate
IfWinExist, AladdinView - BlackRock Solutions - Internet Explorer
    WinActivate
IfWinExist, Positions, Positions, AladdinView - BlackRock Solutions - Internet Explorer
    WinActivate
IfWinExist, AladdinView
    WinActivate
IfWinExist, Matching, AladdinView
    WinActivate
return

; AutoComplete
::/53::
SendInput S3QH78
return

::ddox::
SendInput Documents
return

::ddes::
SendInput Desktop
return

::/hh::
SendInput HiHi
return

; ------------------------------------------------------------------------------------------------

::/acc::
IfWinExist, Cash Management
    WinActivate
return

::/af::
SetTitleMatchMode, 2
IfWinExist, Apex Enterprise
	WinActivate
return

::/ai::
SetTitleMatchMode, 2
IfWinExist, ID
	WinActivate
return

::/00::
SetTitleMatchMode, 2
IfWinExist, OneNote
	WinActivate
else
run, "C:\ProgramData\Microsoft\Windows\Start Menu\Programs\Microsoft Office 2013\OneNote 2013.lnk"
return

::/vv::
SetTitleMatchMode, 2
IfWinExist, GVIM
WinActivate
return

::/rs::
SetTitleMatchMode, 2
IfWinExist ahk_exe rstudio.exe
    WinActivate ahk_exe rstudio.exe
else
return

::/vi::
SetTitleMatchMode, 2
IfWinExist ahk_exe gvim.exe
    WinActivate ahk_exe gvim.exe
else
return
return

::/cm::
SetTitleMatchMode, 2
IfWinExist ahk_exe cmd.exe
    WinActivate ahk_exe cmd.exe
else
return
return

::/r::
SetTitleMatchMode, 2
IfWinExist ahk_exe rstudio.exe
    WinActivate ahk_exe rstudio.exe
else
return
return

::/ex::
SetTitleMatchMode, 2
IfWinExist ahk_exe EXCEL.EXE
    WinActivate ahk_exe EXCEL.EXE
else
run, "C:\ProgramData\Microsoft\Windows\Start Menu\Programs\Microsoft Office 2013\Excel 2013.lnk"
return  

::/pa::
SetTitleMatchMode, 2
IfWinExist ahk_exe mspaint.exe
    WinActivate ahk_exe mspaint.exe
else
run, "%windir%\system32\mspaint.exe"
return

::/pp::
SetTitleMatchMode, 2
IfWinExist ahk_exe POWERPNT.EXE
    WinActivate ahk_exe POWERPNT.EXE
return   

^+g::
WinGetClass, ActiveClass, A
WinActivateBottom, ahk_class %ActiveClass%
return

::/rr::
SetTitleMatchMode, 2
IfWinExist, Apex Enterprise
	WinActivate
MouseClick, left, 1669, 64
return 

::/a1::
SetTitleMatchMode, 2
IfWinExist, Apex Enterprise
	WinActivate
MouseClick, right, 103, 242
return 

::/a2::
SetTitleMatchMode, 2
IfWinExist, Apex Enterprise
	WinActivate
MouseClick, right, 103, 259
return 

::/a3::
SetTitleMatchMode, 2
IfWinExist, Apex Enterprise
	WinActivate
MouseClick, right, 103, 270
return 

::/l1::
SetTitleMatchMode, 2
IfWinExist, Apex Enterprise
	WinActivate
MouseClick, right, 103, 262
return 

::/l2::
SetTitleMatchMode, 2
IfWinExist, Apex Enterprise
	WinActivate
MouseClick, right, 103, 289
return 

::/l3::
SetTitleMatchMode, 2
IfWinExist, Apex Enterprise
	WinActivate
MouseClick, right, 103, 306
return 

::/s::
run, "C:\SRDEV\B_Bash\python_screenshot.bat"
return

::/w::
SetTitleMatchMode, 2
IfWinExist RepoPricer.xlsm
    WinActivate RepoPricer.xlsm
return   

::/da::
SetTitleMatchMode, 2
IfWinExist Daily_.xlsx
    WinActivate Daily_.xlsx
return   

::/fi::
SetTitleMatchMode, 2
IfWinExist Mozilla Firefox
    WinActivate Mozilla Firefox
return  

::/t30::
SetTitleMatchMode, 2
IfWinExist, T+30
WinActivate
return

; Shift + Wheel for horizontal scrolling
^WheelDown::WheelRight
^WheelUp::WheelLeft


::/t1::
ResizeWin(350,1005, 1, 1)
return

::/t2::
ResizeWin(1283,1005, 397, 1)
return

; width height x y
::/t3::
ResizeWin(1283,640, 397, 370)
return

; width height x y
::/t4::
ResizeWin(736,600, 937, 400)
return

; width height x y
::/t5::
ResizeWin(1140,1050, 3360, 1)
return

; width height x y
::/bf::
ResizeWin(2544,516, 1000, 500)
return

^!NumpadSub::
SetTitleMatchMode, 2
IfWinExist, Cash Management
{
{
    WinActivate
	ResizeWin(1283,640, 397, 370)
}
IfWinExist, AAA Rich's  Favourite
{
    WinActivate, AAA Rich's  Favourite
	ResizeWin(1283,1005, 397, 1)	
}
IfWinExist, Apex Collateral
{
	WinActivate  Apex Collateral
;	ResizeWin(1696, 1050, 1672, 1)
	ResizeWin(1685, 1050, 1680, 1)
	WinWait, Apex Collateral 16.2.96.SRE.2
	WinMaximize
}
IfWinExist, IB - All chats
{
	WinActivate  IB - All chats
	ResizeWin(740,1050, 3360, 1)
}
IfWinExist, Apex Enterprise 15.1.62
{
}
return
}
return

; ALWAYS ON TOP ----------------------------------------------------------------
; ^SPACE::  Winset, Alwaysontop, , A
;Alt+T = Toggle AlwaysOnTop state of the active window
^!SPACE::
{
WinSet, AlwaysOnTop, Toggle, A
SplashTextOn ,800 ,800 , Afloat Toggle
Sleep 300
SplashTextOff
}
return

::/o::
{
run, "C:\SRDEV\B_Bash\R_OTC.bat"
return
}

::/l::
{
run, "C:\SRDEV\B_Bash\R_SLB.bat"
return
}

::/c::
{
run, "C:\SRDEV\B_Bash\R_collateral.bat"
return
}

::/r1::
{
run, "C:\SRDEV\B_Bash\R_FIN_1.bat"
return
}
return

; FINACE 3000 ----------------------------------------------------------------
::-l1::
SetTitleMatchMode, 2
IfWinExist, Apex Enterprise
	WinActivate
MouseClick, right, 103, 262
return 

::-l2::
SetTitleMatchMode, 2
IfWinExist, Apex Enterprise
	WinActivate
MouseClick, right, 103, 289
return 

::-l3::
SetTitleMatchMode, 2
IfWinExist, Apex Enterprise
	WinActivate
MouseClick, right, 103, 306
return 

::-a1::
SetTitleMatchMode, 2
IfWinExist, Apex Enterprise
	WinActivate
MouseClick, right, 103, 242
return 

::-a2::
SetTitleMatchMode, 2
IfWinExist, Apex Enterprise
	WinActivate
MouseClick, right, 103, 259
return 

::-a3::
SetTitleMatchMode, 2
IfWinExist, Apex Enterprise
	WinActivate
MouseClick, right, 103, 270
return 

::-2-::
IfWinExist, Apex Enterprise
    WinActivate
IfWinExist, Alert
    WinActivate
return

::-0-::
SetTitleMatchMode, 2
IfWinExist laser
    WinActivate laser
else
run, \\CHRB1025.CORP.GWPNET.COM\homes\7\S3QH78\Documents\L_Laser\mk_laser_v3.jar
return  

::-3-::
SetTitleMatchMode, 2
IfWinExist, T+30
WinActivate
return

::-5::
SetTitleMatchMode, 2
IfWinExist, Apex Enterprise
	WinActivate
return 

::-s::
SendInput yours pls
return

::-b::
SendInput mine pls
return

::- ::
SendInput can you bid
return

::-f::
SendInput can you offer
return

::-m::
run, "C:\SRDEV\B_Bash\get_REPO_PX.bat"
return

^j::
settitlematchmode, 2
ifwinexist laser
    winactivate laser
else
run, \\chrb1025.corp.gwpnet.com\homes\7\s3qh78\documents\l_laser\mk_laser_v3.jar
return 

^l::
run, "C:\SRDEV\B_Bash\get_isin.bat"
return

::-1-::
IfWinExist, Cash Management
    WinActivate
return


; Activate single Bloomberg Screens	
	::-b1::
	IfWinExist, 1-BLOOMBERG
	    WinActivate
	IfWinExist, 1-Bloomberg
	    WinActivate 1-Bloomberg
	return
	
	::-b2::
	IfWinExist, 2-BLOOMBERG
	    WinActivate
	IfWinExist, 2-Bloomberg
	    WinActivate 2-Bloomberg
	return 
	
	::-b3::
	IfWinExist, 3-BLOOMBERG
	    WinActivate
	IfWinExist, 3-Bloomberg
	    WinActivate 3-Bloomberg
	return
	
	::-b4::
	IfWinExist, 4-BLOOMBERG
	    WinActivate
	IfWinExist, 4-Bloomberg
	    WinActivate 4-Bloomberg
	return


; FINACE 3000 - REPO ACTIVATION
::-f1::
SetTitleMatchMode, 2
IfWinExist, Apex Enterprise
	WinActivate
MouseClick, right, 103, 242
return 

::-f2::
SetTitleMatchMode, 2
IfWinExist, Apex Enterprise
	WinActivate
MouseClick, right, 103, 259
return 

::-f3::
SetTitleMatchMode, 2
IfWinExist, Apex Enterprise
	WinActivate
MouseClick, right, 103, 270
return 

; FINACE 3000 - SLB
::--1::
SetTitleMatchMode, 2
IfWinExist, Apex Enterprise
	WinActivate
MouseClick, right, 103, 262
return 

::--2::
SetTitleMatchMode, 2
IfWinExist, Apex Enterprise
	WinActivate
MouseClick, right, 103, 289
return 

::--3::
SetTitleMatchMode, 2
IfWinExist, Apex Enterprise
	WinActivate
MouseClick, right, 103, 306
return 

::/pf::
SetTitleMatchMode, 2
IfWinExist, PortfolioMonitor
	WinActivate
return 

; Messenger
::/m::
SetTitleMatchMode, 2
IfWinExist, App for Messenger™
	WinActivate
IfWinExist, All-in-One Messenger
	WinActivate
return 

; eod
::/eod::
SendInput `
( 
HIHI FRNDS
EOD
BIBI
MEIKEL
)
return

; hi
::/*/::
SendInput `
( 
hi
hope all gd
)
return

^NumpadMult::
SetTitleMatchMode, 2
IfWinExist ahk_exe WFICA32.EXE
    WinActivate ahk_exe WFICA32.EXE
return

; NGT
::/ngt::
SetTitleMatchMode, 2
IfWinExist, Next Gen Trading
	WinActivate
return 

; Portfolio Construction
::/pc::
SetTitleMatchMode, 2
IfWinExist, PortfolioConstruction
	WinActivate
return 

; Portfolio Construction
::/te::
SetTitleMatchMode, 2
IfWinExist, TradeEntry
	WinActivate
return 

; Portfolio Construction
::/pm::
SetTitleMatchMode, 2
IfWinExist, PortfolioMonitor
	WinActivate
return 

; Portfolio Construction
::/oa::
SetTitleMatchMode, 2
IfWinExist, OANDA Web Trading Platform
	WinActivate
return 

::/repo1::
SetTitleMatchMode, 2
IfWinExist, Apex Enterprise
	WinActivate
MouseClick, left, 103, 242
return 

::/loans1::
SetTitleMatchMode, 2
IfWinExist, Apex Enterprise
	WinActivate
MouseClick, left, 103, 262
return 

::/77::
SetTitleMatchMode, 2
IfWinExist ahk_exe pycharm64.exe
    WinActivate ahk_exe pycharm64.exe
return

::-ttt::
run, "C:\SRDEV\B_Bash\repo_tx.bat"
return

::/tw::
IfWinExist, TW
    WinActivate 
return
