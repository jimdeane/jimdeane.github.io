`- task: PowerShell@2`
&nbsp;&nbsp;&nbsp;`displayName: "Display Manifest"`
&nbsp;&nbsp;&nbsp;`inputs:`
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`targetType: 'inline'`
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`script: |`
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`$content = Get-Content -Path '$(System.DefaultWorkingDirectory)/src/Malue.App.UI.MAUI/Platforms/Android/AndroidManifest.xml'`
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`Write-Host $content`