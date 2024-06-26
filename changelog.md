# CLApp Changelog

# What's New (v1.6.0)

- Support for making Python apps
- Support for making Node apps
- Built-in unit test code for each type of app
- Built-in settings code for bash apps
- Under the hood improvements
- Auto updates
- Shorthand style
- Settings
- Alternative arg handling functions (Bash)
- State-based processing option for (Bash)
- Command mode option (Bash)
- Cross compatibility (Bash)
- System-install variant for when you want any user to access the app
- Versioning controlled by semver (not the node package, general bash script for updating version files of various kinds made by me)

# What's Next (v1.7.0)

- I guess we will see what else

# Bugs
## Key:
**CB=CLApp Bug**
**R=Resolved**
**O=Outstanding**
**D=Deleted**

- CB000000 [R]: Auto-update sometimes results in unexpected code being run or app crashing errors to be thrown, only use if you are sure you can reverse the operation!
            **Resolution**: If you experience issues, just run the command again, cleaning up rogue files, generally due to files not being fully copied yet and bash still parsing the app code (copy-run conflicts)

- CB000001 [R]: Shorthand style would take over when arg style is desired
            **FIX**: No longer unexpectedly runs shorthand style when running in arg style

- CB000002 [O]: Short-hand style does not recognize arguments properly. Name is not grabbed upon usage like so: clapp name node style=MEE
            **Fixed?**: shorthand style now correctly recognizes arguments
