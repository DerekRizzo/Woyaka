#NoEnv  ; Recommended for performance and compatibility with future AutoHotkey releases.
; #Warn  ; Enable warnings to assist with detecting common errors.
SendMode Input  ; Recommended for new scripts due to its superior speed and reliability.
SetWorkingDir %A_ScriptDir%  ; Ensures a consistent starting directory.
#IfWinActive GTA:SA:MP
#SingleInstance, Force
#Include samp3.ahk
	F2::
		Sleep 300
		a:=1
		menu:=1
		ShowDialog("2", "Test", "Test1`nTest2`nTest3", "Закрыть")
	return
	$~ESC::
		menu:=0
		return
	~UP::
		if a>1
	{
		a:=a-1
	}
	return
	~Down::
		if a<b
	{
		a:=a+1
	}
	return
	$~Enter::
		if (isDialogOpen())
	{
		if (menu==1){
		punk:="pabel"+a
		Gosub, %punk%
		menu:=0
	return
	}
	}
	pabel1:
	Test1=Цитрамон
	{
		Sleep 300
		SendChat("т."Test1)
	}
	return
