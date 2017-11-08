# Visual Studio Code Snippets for the Pure Storage Toolkits
Code snippets for Visual Studio Code that cover Pure Storage support for Python and PowerShell. 

![vscode-snippet_example1](/docs/vscode-snippets_example1.png)

Snippets:
* pfaconnect -- Creates completed cmdlet with tab marks for connecting to the Pure Storage FlashArray.

```powershell
# Connect to the Pure Storage FlashArray
FlashArray = New-PfaArray -EndPoint  -Credentials (Get-Credential) -IgnoreCertificateError
```
Note: Still working to figure out why the "FlashArray" at the beginning is not picking up the $ (I know its syntax related) and also tabbing past the "EndPoint" tab mark ($2). 

* pfavolsnap -- Creates completed cmdlet with tab marks for creating a Pure Storage FlashArray volume snasphot based on a source volume. 

```powershell
# Create new volume snapshot.
New-PfaVolumeSnapshots -Array $1 -Source $2
```
