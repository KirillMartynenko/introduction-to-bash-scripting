# Bash Variables

As in any other programming language, you can use variables in Bash Scripting as well. However, there are no data types, and a variable in Bash can contain numbers as well as characters.

To assign a value to a variable, all you need to do is use the `=` sign:

```bash
name="DevDojo"
```

>{notice} as an important note, you can not have spaces before and after the `=` sign.

After that, to access the variable, you have to use the `$` and reference it as shown below:

```bash
echo $name
```

Wrapping the variable name between curly brackets is not required, but is considered a good practice, and I would advise you to use them whenever you can:

```bash
echo ${name}
```

The above code would output: `DevDojo` as this is the value of our `name` variable.

Next, let's update our `devdojo.sh` script and include a variable in it.

Again, you can open the file `devdojo.sh` with your favorite text editor, I'm using nano here to open the file:

```bash
nano devdojo.sh
```

Adding our `name` variable here in the file, with a welcome message. Our file now looks like this:

```bash
#!/bin/bash

name="DevDojo"

echo "Hi there $name"
```

Save it and run the file using the command below:

```bash
./devdojo.sh
```

You would see the following output on your screen:

```bash
Hi there DevDojo
```

Here is a rundown of the script written in the file:

* `#!/bin/bash` - At first, we specified our shebang.
* `name=DevDojo` - Then, we defined a variable called `name` and assigned a value to it.
* `echo "Hi there $name"` - Finally, we output the content of the variable on the screen as a welcome message by using `echo`

You can also add multiple variables in the file as shown below:

```bash
#!/bin/bash

name="DevDojo"
greeting="Hello"

echo "$greeting $name"
```

Save the file and run it again:

```bash
./devdojo.sh
```

You would see the following output on your screen:

```bash
Hello DevDojo
```

Note that you don't necessarily need to add semicolon `;` at the end of each line. It works both ways, a bit like other programming language such as JavaScript!
