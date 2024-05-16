# CLApp Changelog

# What's New (v1.4.1)

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

# What's Next (v1.5.0)

- Not sure

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
