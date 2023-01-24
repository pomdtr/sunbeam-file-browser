# File Browser Extension for Sunbeam

This extension adds a file browser to [Sunbeam](https://pomdtr.github.io/sunbeam).

## Installation

```bash
sunbeam extension install file-browser https://github.com/pomdtr/sunbeam-file-browser
```

If the `file-browser` command is not available, you will need to choose another name for the extension.

## Usage

Show a file browser with the `file-browser` command.

```bash
# Show a list of predefined roots
sunbeam file-browser

# Show a list of files in a specific root
sunbeam file-browser browse-files --root /path/to/root
```

If you want to add a new item to the root list, add the following snippet to your sunbeam config file.

```yaml
rootItems:
    - title: Browse Dev Folder
      extension: file-browser
      command: browse-files
      with:
        root: /path/to/dev/folder
```
