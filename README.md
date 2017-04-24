A.
	The encoded identifiers used for the functions:
		0000000000400555 T main
		000000000040052d T _Z7averageif
		00000000004004ed T _Z7averagePdRd


B.
	Output:
			1 8
			4 8
			4 8
			8 8
	
	Why:
		因為指標是用來存取變數空間的位址，所以不管指標宣告成指向哪一種型別的變數，編譯器都是配置相同大小的記憶體空間給指標變數。在64位元系統並搭配64位元編譯器，則指標將佔8個位元組。因此sizeof(pa)==sizeof(pb)==sizeof(pc)==sizeof(pd)==8 。
