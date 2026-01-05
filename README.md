# How-to-enable-Photo-Image-on-the-Windows-Server
How to enable Photo Image on the Windows Server 

1. Register dll as app \
regsvr32 "C:\Program Files\Windows Photo Viewer\PhotoViewer.dll"

2. Create reg file and import it

Windows Registry Editor Version 5.00

[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows Photo Viewer\Capabilities\FileAssociations] \
".jpg"="PhotoViewer.FileAssoc.Tiff" \
".jpeg"="PhotoViewer.FileAssoc.Tiff" \
".png"="PhotoViewer.FileAssoc.Tiff" \
".bmp"="PhotoViewer.FileAssoc.Tiff" \
".gif"="PhotoViewer.FileAssoc.Tiff" \
".ico"="PhotoViewer.FileAssoc.Tiff" \
".jfif"="PhotoViewer.FileAssoc.Tiff" \
".webp"="PhotoViewer.FileAssoc.Tiff"

3. And you can use Windows Image View as the default app for viewing image files
