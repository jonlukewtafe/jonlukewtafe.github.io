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

{% include_relative footer.md %}
