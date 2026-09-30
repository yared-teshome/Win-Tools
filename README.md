<#
.SYNOPSIS
    Remote Server Cleanup GUI

.DESCRIPTION
    Windows Forms administrative utility for performing selected cleanup
    operations against one or more remote Windows servers through
    PowerShell remoting.

    Provides:
    - Multi-server processing
    - WinRM connectivity validation
    - Optional alternate credentials
    - WhatIf / preview mode
    - User and Windows temporary-file cleanup
    - Recycle Bin cleanup
    - SCCM / Configuration Manager cache cleanup
    - Windows Update download-cache cleanup
    - DISM component-store cleanup
    - IIS log cleanup
    - Optional custom-path cleanup
    - Live Process Viewer
    - Remote CSV and log output
    - Integrated Help and command reference

.COMPATIBILITY
    Windows PowerShell 5.1
    Windows Server 2016 and later

.REQUIREMENTS
    - Run from an elevated Windows PowerShell session
    - PowerShell remoting / WinRM must be available on target systems
    - Operator must have the required administrative permissions

.OUTPUT
    Default remote output location:

        C:\ProgramData\ServerCleanup

    Output includes:
    - Timestamped log file
    - Timestamped CSV results file

.SAFETY
    This tool performs destructive cleanup operations when WhatIf mode
    is disabled.

    Recommended practice:
    1. Test against a non-production server first.
    2. Run in WhatIf mode before performing cleanup.
    3. Review selected cleanup options.
    4. Review custom paths carefully.
    5. Use an approved maintenance window where appropriate.
    6. Review generated logs after execution.

.NOTES
    Project:
        Remote Server Cleanup

    Script:
        Remote-Server-Cleanup.ps1

    Version:
        1.0.0

    Status:
        Archived baseline / controlled administrative utility

    Maintainer:
        Infrastructure / Systems Administration

    Source Control:
        Store in an approved Git repository or equivalent version-control system.

    Important:
        Historical versions should not be overwritten.
        Changes should be committed as new versions with release notes.

    Last Reviewed:
        2026-09-30
#>
