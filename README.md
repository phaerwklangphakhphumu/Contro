# Contro
Wnd = WinGetHandle("[CLASS:RegEdit_RegEdit]")      $hControl = ControlGetHandle($hWnd, "", "[CLASS:SysTreeView32; INSTANCE:1]")        $aKey = StringSplit($sKey, '')      $sKey = '#0'      For $i = 1 To $aKey[0]          ControlTreeView($hWnd, "", $hControl, "Expand", $sKey)          $sKey &amp;= '|' &amp; $aKey[$i]      Next
