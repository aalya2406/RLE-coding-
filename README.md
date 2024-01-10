# RLE-coding-
Methods in RLEconverter Class
Compression Methods
compressFile(String fileName)

Reads an uncompressed ASCII image file.
Applies RLE compression to each line.
Writes the compressed data to a new file.
compressLine(String line, char[] fileChars)

Implements the RLE compression algorithm on a single line of ASCII data.
compressAllLines(String[] lines, int dataSize, char[] fileChars)

Iterates through all lines, applying compression to each line.
getCompressedFileStr(String[] compressed, char[] fileChars)

Assembles the compressed lines for writing to a file.
Decompression Methods
decompressFile(String fileName)

Reads an RLE compressed ASCII image file.
Applies RLE decompression to each line.
Writes the decompressed data to a new file.
decompressLine(String line, char[] fileChars)

Decodes a line that was encoded by the RLE compression algorithm.
decompressAllLines(String[] lines, int dataSize)

Iterates through all compressed lines, applying decompression.
getDecompressedFileStr(String[] decompressed)

Assembles the decompressed lines for writing to a file.
Utility Methods
discoverAsciiChars(String[] decompressed, int dataSize)

Discovers the two ASCII characters that make up the image file.
writeFile(String data, String fileName)

Writes data to a specified file.
Unit Tests
The ProjectTests class in the test package contains JUnit tests for various aspects of the compression and decompression processes. These tests verify the correctness of the implemented methods.
