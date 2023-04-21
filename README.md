# bitmap-transformer

The bitmap transformer app can take an `input-file` from the command line and apply a transformation, saving to the specified `output-file`. The app can be run with Gradle and requires 3 command line arguments.

To Use:
- Place your .bmp file to be transformed in the desired directory. Note: by default a relative path given searches from `bitmap-transformer/app/`. The options are:
  - Use a full path to specify input/output file locations if a directory above the /app directory is desired.
  - Use a relative path that starts from `bitmap-transformer/app/`.
- Decide on your transform. Supported transformations are:
  - "f" to flip the image horizontally.
  - "g" to convert the image to grayscale
  - "i" to invert the colors of the image
- Apply the transform to the output file you specify (.bmp)
```bash
./gradlew run --args "input-file.bmp output-file.bmp transform"
```

## Collaborators

Stephen Levesque
Matt Austin