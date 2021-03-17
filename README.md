# BFS-DAN-DFS-GRAPH
Complete BFS dan DFS

#analisa menurut saya ferdy berliano putra
terdapat nilai A, B, C, D, E, F, G, H, I, J, K, L

awal A tujuan I

yang mana :
A level 0

B level 1

C F G level 2

D   H level 3

E  I J level 4

	pada depth first search di lakukan cek pertama peta A
		jika kita jalankan programnya maka akan mencetak "A, B, C, D, E, F, G, H, I"
		kenapa demikian?
		pertama pada A terdapat cabang B
		kemudian dilakukan cek pada B yang terdapat cabang C F G tidak ditemukan I
		lalu di cek pada C (karena cabang pertama pada peta B adalah C) tidak ditemukan 
		kemudian dilakukan cek pada D yang terdapat cabang E tidak ditemukan juga
		kemudian dilakukan cek pada E tidak ditemukan juga dan di kembalikan ke cabang F yang terdapat pada cabang B
		kemudian dilakukan cek pada F tidak ditemukan juga dan di kembalikan ke cabang G yang terdapat pada cabang B
		kemudian dilakukan cek pada G yang terdapat cabang H tidak ditemukan juga
		lalu pada H ditemukan I.
		Dari sini dapat diambil kesimpulan bahwa depth first search melakukan cek satu persatu tidak berdasarkan levelnya 
		Langkah pengcekan dari A ke B ke C ke D ke E ke F ke G ke H
		setiap proses yg dilalui direkam

	pada breadth first search dilakukan cek pertama peta A
		jika kita jalankan programnya maka akan mencetak "A, B, G, H, I"
		kenapa demikian?
		pertama pada A terdapat cabang B (level 1) setelah di cek tidak ditemukan I
		kemudian di cek pada setiap cabang di B yaitu C F G (level 2)
		pada cabang C tidak ditemukan dilanjutkan ke F tidak ditemukan juga dilanjutkan ke G tidak ditemukan juga
		kemudian berlanjutkan ke level 3 yang terdapat D dan H yaitu D cabang dari C dan H cabang dari G setelah dilakukan cek tidak ditemukan
		kemudian berlanjutkan ke level 4 yang terdapat E, I dan J yaitu E cabang dari D dan I J cabang dari H setelah dilakukan cek ditemukan I yaitu cabang dari H
		Dari sini dapat diambil kesimpulan bahwa breadth first search melakukan cek perlevel tidak berdasarkan cabang seperti depth first search 
		Langkah pengcekan dari A ke B ke C F G ke D H ke E I
		setiap proses yg dilalui direkam

