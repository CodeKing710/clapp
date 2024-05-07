# CLApp Changelog

# What's New

- Support for making Python apps
- Support for making Node apps
- Built-in unit test code for each type of app
- Auto updates
- Settings!

# What's Next

- Move file heredocs to variables outside of the function (will allow proper folding and use less cpu at the cost of more RAM)
- Convert some defaults to settings
- Support for code that loads settings within the generated app (bash focus)
- Add option to use new handoff-arglist style of arg parsing (bash)
- Move app generation files to HereDoc Files (*.hdf)

# Bugs
## Key:
**CB=CLApp Bug**
**R=Resolved**
**O=Outstanding**
**D=Deleted**

- CB000000 [R]: Auto-update sometimes results in unexpected code being run or app crashing errors to be thrown, only use if you are sure you can reverse the operation!
                **Resolution**: If you experience issues, just run the command again, cleaning up rogue files, generally due to files not being fully copied yet and bash still parsing the app code (copy-run conflicts)
