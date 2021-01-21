Experimental environment: win10 x64    
Software official website::https://huorong.cn  
Software version::5.0.56.2
Affected Component: TopsecDaemon.exe
  
The root cause of this vulnerability is that ordinary users can open Tinder security and can open the recovery area of Tinder security software. When recovering malicious samples, the file parsing point is not judged, the simulation token is not used, and the target file has no write permission. As a result, symbolic link hijacking can be used to restore to C:\Windows\system32, creating arbitrary file names, resulting in escalation of local privileges
