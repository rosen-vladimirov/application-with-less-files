# application-with-less-files

Demonstrates an issue in `nativescript-dev-less` plugin when application has `nsconfig.json` in which the path to `app` directory has been changed.

## Steps to reproduce

1. Clone this repository: `git clone https://github.com/rosen-vladimirov/application-with-less-files.git`
2. In the terminal, navigate to the cloned directory: `cd application-with-less-files`
3. Run `tns prepare android` or `tns run android`
The command will fail with error: `The "path" argument must be one of type string, Buffer, or URL. Received type undefined.`
<br/>
Expected behavior: application should work fine and you should be able to apply changes in `app.less` file.