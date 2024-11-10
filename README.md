# Sharp-MCP-72BGA
Breakout adapter for Sharp MCP chips in BGA72 package

Most Sharp MCP flash chips use the same main pinout for the the flash interface, but provisions have been made on the adapter board to allow for changes if necessary.
1. Pin 47 can either be NC, CE2, or VCCQ depending on the chip. It is prewired to ball H3, but if necessary, cut the trace where indicated and wire a jumper wire from Pin 47 to wherever it's needed. 
2. A10 and H10 have functions on some chips, so they are broken out to allow for easy access if necessary. Otherwise, these can be left as NC. Ball H10 is CE2 on a few single-die Sharp chips, but so far every MCP has featured CE2 on ball H3.
3. Chips under 32mbits use a slightly different DIP pinout that this adapter maps to the BGAs. For chips of this size, either swap pins 9 and 15, or simply read the chip as 64mbit and truncate the file to the necessary size.
