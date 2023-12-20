#Hashing Exercise


This repository was created as part of my operational systems class project.
Here you will find a bash script of a simple hashing exercise.

This script takes as an input a 4-digit integer, hashes it using SHA-256 and stored the hash in a file.

##Usage

1. Make sure you have bash installed on your computer.

2. Clone the repository or simply download the `hash_script` file.

3. Open a terminal and go to the directory that you have stored the script in.

4. Make sure the script is executable:
	```bash
	chmod +x hash_script
	```
5. Call the bash script like this:
	```bash
	./hash_script <number>
	```
   Where `<number>` is any 4-digit number you want to hash. 

6. The output will be stored in the file `hash_output.txt`.

##Example


I have hashed the number 0554 like this:
	```bash
	./hash_script 0554
	```
and the output is stored in the `hash_output.txt` as such:
`Hashed output: d3d29bda9ce1dd0de4c57fc488b35bc1ccecfb98a874e5527d9ee59e58072927`

You can verify this on your own by executing the command `cat hash_output.txt` or running the example on your own.

Notice when running sha256sum the output has usually a `-` or `*-`. Since we don't need it i have used the command cut to remove it and keep only the hash.
