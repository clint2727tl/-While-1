# -While-1
    While 1         $sTMP = StderrRead($iPID, False, False)         If @error Then ExitLoop         If $sTMP &lt;> "" Then             $sTMP = StringReplace($sTMP, @CR &amp; @CR, '')             $sSTD &amp;= $sTMP             Call($sCallBackFunction,$sTMP) ;~          ConsoleWrite($sTMP)             Sleep($iDelay)
