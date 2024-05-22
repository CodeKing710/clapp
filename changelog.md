# CLApp Changelog

# What's New (v1.4.4)

- Support for making Python apps
- Support for making Node apps
- Built-in unit test code for each type of app
- Built-in settings code for bash apps
- Auto updates
- Shorthand style
- Settings
- Alternative arg handling functions
- Command mode option
- Under the hood improvements
- Cross compatibility good so far

# What's Next (v1.5.0)

- System-install variant for when you want any user to access the app
- Cross-platform compatibility
  - [DONE] Add quotes to all variables
  - [DONE] Use param-exp notation where possible for better variable interpolation
  - [DONE] Adjust Bash assets to reflect compatible app style (mimic CLApp)

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
