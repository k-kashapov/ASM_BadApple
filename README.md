# ASM_BadApple
BadApple running on DOSBox + Assembly

# Description
Plays BadApple in DOS. Waits for any key to be pressed after each frame. File bits.txt contains encrypted frame data. Encryption is neccessary to fit all the frames into 64 Kb segment of DOS. Assembly code decrypts the binary and prints bytes into video memory.

# Usage
1) Compile bad.ASM using any preferable compiler into a .COM file.
2) Copy contents of bits.txt into the end of .COM file. This action is required, because Turbo Assembly can't compile file of size 63 Kb.
3) Run .COM file. Press any key to proceed to the next frame

# Known Issues:
1) While drawing a frame, a few bytes are skipped
2) After approximately 1 minute of original video, program will stop showing any decent picture.

The reasons behind these are yet to be dicovered.
