#### 0.73
- Bug fix: GetSystemFirmwareTable should take `resultBufferSize` as an argument for the second call.
- Bug fix: nullref exception in timing.cpp.
- New: Add more checks for VMware related processes.
- New: Add more checks for VMware related files.
- New: Add more checks for VMWare related registry: SYSTEM\\ControlSet001\\Control\\SystemInformation.
- New: Add more checks for system firmware tables (SMBIOS and ACPI for VMware).
- New: Add more loaded dlls check inside process context:  avghookx.dll, avghooka.dll, snxhk.dll.
- New: Add write watch debugger detection.
- New: Add service anti-VM checks.
- New: Add checks for VM related services.
- Enhancement: add some macros to enable/disable a particular category of checks to easy debugging.


#### 0.72
- Bug fix: PEB offset in NumberOfProcessors() thanks to @Nxgr.
- Bug fix: array with duplicate strings in process_tools check thanks to @stxletto.
- Bug fix: ascii_to_wide_str() wrong argument thanks to @stxletto.

### 0.71
- New: Add kernel debugger check using the KUSER_SHARED_DATA struct.
- New: Add kernel debugger check using NtQuerySystemInformation with SystemKernelDebuggerInformation.
- New: Added process job anti-debug check.
- New: Added system firmware tables with GetSystemFirmwareTable (SMBIOS and ACPI for VirtualBox).