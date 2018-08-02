Please visit https://gpuopen.com/decoding-radeon-vulkan-versions/ for more information.

Iterate over `<amd_drivers>` and interrogate the following:
```xml
<amd_drivers>
    <!-- many of the following -->
    <driver version="DRIVER_VERSION" operating-system="OS">
        <whql>WHQL</whql>
        <download-url>DOWNLOAD_URL</download-url>
        <internal-version>INTERNAL_VERSION</internal-version>
        <windows-version>WINDOWS_VERSION</windows-version>
        <vulkan-version>VULKAN_VERSION</vulkan-version>
    </driver>
</amd_drivers>
```

- `version`: Public version number, queried via AGS
  - `AGSGPUInfo->radeonSoftwareVersion` [link](https://gpuopen-librariesandsdks.github.io/ags/struct_a_g_s_g_p_u_info.html)
- `operating-system`: _Windows_
- `whql`: _WHQL_ or _Optional_
- `download-url`: Download link
- `internal-version`: AMD internal development version number
- `windows-version`: Windows Driver Store version number
- `vulkan-version`: AMD Vulkan ICD version number  
