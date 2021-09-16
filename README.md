This repo is to enable change documentation following mod edits for a valhiem server. 

Current issue exists in the github changelogs - the comments in the config files being uploaded break the git parser when it attempts to execute > git dff

Here is a code snippet from the broken changelog : 

```cfg
@@ -7,19 +7,19 @@ enabled = true

mainMenuLogo = true	mainMenuLogo = true
```

where it should be : 

``` cfg
[ValheimPlus]

; Change false to true to enable this section. https://valheim.plus/documentation/list#ValheimPlus
enabled = true

; Display the Valheim Plus logo in the main menu
mainMenuLogo = true

; Display the advertisement of our server hosting partner on the server browser menu
serverBrowserAdvertisement = false

[AdvancedBuildingMode]

```
