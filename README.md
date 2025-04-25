# Qodana Configuration Examples

## Summary
I highly recommend if you randomly stumbled here than you should read this whole README. This will be the centralized document for all configuration files in here.

## Security only
There may be a time when you want to have a separate UI endpoint for security folks then for software engineers. If this is the case then [security-only.yaml](https://github.com/alexMcosta/qodana_configuration/blob/main/security-only.yaml) will be the route you want to go. It is configured for all security inspections for every linter/language to make it universal. Only thing it does not include is Taint Analysis since at this time its only available for Java and PHP and only visible on Jetbrains IDE’s
When using this you will need it to run as a [monorepo](https://www.jetbrains.com/help/qodana/monorepo-project.html) by setting up two scans; One for your regular scan, and one for Security. If you happen to be adding this to a monorepo then just configure it as a third scan.
