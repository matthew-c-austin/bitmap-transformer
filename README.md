# bitmap-transformer

The bitmap transformer app can take an `input-file` from the command line and apply a transformation, saving to the specified `output-file`. The app can be run with Gradle and requires 3 command line arguments.

To Use:
- Place your .bmp file to be transformed in the bitmap-transformer/app/src/main/resources directory. The existing file "baldy-8bit.bmp" will be used in this example.
- Decide on your transform. Supported transformations are:
  - "f" to flip the image horizontally.
  - "g" - to convert the image to grayscale
  - "i" to invert the colors of the image
- Apply the transform to the output file you specify (.bmp)
```bash
./gradlew run --args "input-file.bmp output-file.bmp transform"
```
The transformed image can be found in the same folder that the input file was placed.
