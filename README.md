# Unpacked Godot Loader

For those who want to distribute their godot project with it's resources unpacked. Looks for a `res://shared/startup.tscn` in its current directory and transfers control to it. Simply export the binary and pack you want from this project with the desired name, unpack the actual target project into the same directory, and it will launch your `shared/startup.tscn`!

## Building

This project was made in Godot 3.4.4, but since it contains only a basic node and one line of GD Script, there is reason to believe it will work in many other versions. If not, feel free to copy my entire line of code to an empty project of your own!

## Usage

1. Generate an executable with the desired name and settings from this project in a new directory.
2. Build the project you actually want to run, ensuring that it has a `res://shared/startup.tscn` as its startup scene. Avoid having a directory named `res://unpacked_godot_loader/`, as contents may conflict with this project.
3. [Unpack](https://github.com/hhyyrylainen/GodotPckTool) the resulting Godot pack into the directory created for this loader.
4. Run.

If all went well, this executable should load its own pack which immediately chains to your unpacked resources, allowing you to distribute and run games with all files accessible.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change. I'm really not sure what you would change or what would constitute a major change, since a second line of code would literally double the size of this project.

There are no tests. So sorry.

## License
[MIT](https://choosealicense.com/licenses/mit/)
