
Config { font = "-misc-fixed-*-*-*-*-13-*-*-*-*-*-*-*"
    , bgColor = "#1d2021"
    , fgColor = "#ebdbb2"
    , position = Top
    , lowerOnStart = True
    , allDesktops = True
    , pickBroadest = False
    , overrideRedirect = False
    , commands = [    Run Weather "ENNO" ["-t"," <tempC>C","-L","64","-H","77","--normal","green","--high","red","--low","lightblue"] 36000
                    , Run Network "eno1" ["-L","0","-H","32","--normal","green","--high","red"] 10
                    , Run MultiCpu ["-L","15","-H","50","--normal","green","--high","red"] 10
                    , Run Memory [] 10
                    , Run Swap [] 10
                    , Run TopProc [] 10
                    , Run Com "/bin/sh" ["-c","~/scripts/spotsh"] "music" 1
                    , Run Com "fortune" ["-n 30"] "ff" 1000
                    , Run Volume "default" "Master" [] 10
                    , Run Date "%a %b %_d %Y %H:%M:%S" "date" 10
                    , Run UnsafeStdinReader
    ]
    , sepChar = "%"
    , alignSep = "}{"
    , template = "%UnsafeStdinReader%  }  %date%  | %ENNO% { %music% | %default:Master%| %multicpu% | %memory%"
