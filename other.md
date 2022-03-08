# Other Links

This page has all links etc. that don't fit into the other categories.

- [Adrian's Diigo](http://diigo.com/user/ady_gould)
- [LeetCode](https://leetcode.com/)
- [PHP Extension Community Library (PECL)](https://pecl.php.net/)
- [AP 7th Edition for Microsoft Word](https://github.com/briankavanaugh/APA-7th-Edition)


# Keyboard shortcuts

All keyboard commands below assume you are using a combination of Windows and the Cmder CLI (easily available through Laragon (Windows only))

## PHPStorm, PyCharm and other JetBrains IDEs

1. Move a line of code up: `CTRL+SHIFT+UP_ARROW`
2. Move a line of code down: `CTRL+SHIFT+DOWN_ARROW`
3. Duplicate a line of code: `CTRL+D`
4. Reformat code: `CTRL+ALT+L`
5. Comment and Uncomment Code/Code Block: `CTRL+/`
6. Git - Commit: `CTRL+K`
7. Git - Push: `CTRL+SHIFT+K`
8. Git - Update Project: `CTRL+T`
9. Git - Add File to Tracking: `CTRL+ALT+A`

## Windows Shortcuts

1. Open 'Windows Explorer' Window: `WINDOWS_KEY + E`

## Cmder CLI Commands

1. `ls` to list all files
   1. You can use `ls -l` to get a wide view of the files (this includes permissions for each file)
   2. You can also use `ls -a` to view all files and folders in the current working directory
   3. You can also use `ls -al` to both view all files and folders in the current working directory and view the permissions and finer details for each folder/file.

# Configurations and Other Settings

## PHPStorm - PHP Template Changes

1. Ensure that anything you want to add to the template(s) is on your clipboard ready to be pasted.
2. Open Settings - `CTRL+ALT+S (PC)` or `CMD + , (MAC)`
3. Locate the `Editor` option
4. Locate the `File and Code Templates` option
5. Click on the `Includes` tab
6. Select the `PHP File Header` option
7. Click in the editor area next to (on the right of) the `PHP File Header` option
8. Paste/Make the changes in this space
9. Click `Ok`
10. Verify it works be generating a new PHP file inside of a PHPStorm project.

Example PHP header template:

```php
/**
 * Title of Application/Code/Class
 *
 * Short Description if required (delete if not)
 *
 * Filename: ${FILE_NAME}
 * Project Name: ${PROJECT_NAME}
 * Author: FULL_NAME <FIRST_NAME.LAST_NAME>
 * Date Created: ${DATE}
 *
 */
```

## PHPStorm - PHP CLI Interpreter Configuration

1. To enable the built in PHP development server(s) use:
2. Open Settings (CTRL+ALT+S)
3. Click on PHP, Locate CLI Interpreter, and click on the ...
4. Click on the `+` symbol on the newly opened window to add a new interpreter
5. Select the "Local Path to Interpreter" option.
6. Rename the interpreter from the default `PHP` to `PHP 8.1` (or whatever version you intend to use)
7. Navigate to your PHP interpreter (php.exe) (typically located in your C drive on Windows)
8. Click `Apply` then `Ok`
9. Back in the Settings window you should now see the interpreter in the `CLI Interpreter` box.
10. You may now also change the `PHP language level` to matcch your PHP version. Doing so will enable PHPStorm to check that your code follows appropriate standards.
11. Now to ensure that it is working:
    - Hover over an open PHP document in PHPStorm.
    - The browser icons should show.
    - Click on the icon of the browser you wish to use to open the file.

# Other Information

## Python - PEP-8 Requirements

 - Line Length of `72`




{% include_relative footer.md %}
