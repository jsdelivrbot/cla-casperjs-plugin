
# CasperJS plugin

CasperJS plugin will allow you to launch PhantonJS and CasperJS scripts from Clarive's instance.

## Requeriments

This plugin requires CasperJS and PhantomJS to be installed in the instance to work properly.

To install PhantomJS you need to click [here](http://phantomjs.org/download.html) and follow the instructions.

To install CasperJS you need to click [here](http://docs.casperjs.org/en/latest/installation.html#installing-from-git) and follow the instructions.

If you are going to run on a remote server, check the server to have both requeriments mentioned above plus [`Expect`](http://expect.sourceforge.net/) installed

## Installing

To install the plugin place the cla-casperjs-plugin folder inside `CLARIVE_BASE/plugins`
directory in Clarive's instance.

## How to use

Once the plugin is placed in its folder, you can start using it going to your Clarive's
instance.

You will have now one new palette service called "Run CasperJS code":

### Run CasperJS Code:

This palette service will allow you to choose between choose an already existing phantom or casper js file, or create it with the code editor and execute that code

- **Server -** This option let you choose the way to execute the code. It can be from an existing file, or creating the js code in the editor.
- **Running a test?-** Check this option if you are running a CasperJS test.
- **File path** - Write the path where the script file is located. It must be the full path to the file.
- **CasperJS arguments -** Fill this if you want to send arguments to CasperJS. For more than one argument you must separate them by white spaces.
- **Script arguments -** Fill this if you want to send arguments to the script. For more than one argument you must separate them by white spaces.

Configuration example:

	Server: Clarive_server
    Running a test?: true
    File path: /opt/clarive/examples/casperTest.js
    CasperJS arguments: 
    Script arguments: arg1 arg2
