# Godenticon

## What's this about?

Given a piece of personal information such as an email address, IP address, or a public key, the program will generate a
unique avatar.
This package allows the generation of such avatars taking color-contrast and symmetry into account.

## Usage

```bash
# See Help
go run . -h

# General Usage
go run . <identifier> [--complexity=<level>] [--width=<widthInPx>] [(--output=<filePathAndName> [--overwriteExistingFile])]

# Example: output result into filename.png (overwrites if it already exists)
go run . MY_UNIQUE_STRING --complexity=4 --width=200 --output=filename.png --overwriteExistingFile

# Example: pipe output from stdout into file `myfile.png`
go run . MY_UNIQUE_STRING > myfile.png

# Example: Compile and run
go build .
./godenticon MY_UNIQUE_STRING > myfile.png
```

## Resources

* http://golang.org/pkg/crypto/
* http://golang.org/pkg/image/
* http://en.wikipedia.org/wiki/Identicon
* http://haacked.com/archive/2007/01/22/Identicons_as_Visual_Fingerprints.aspx/
