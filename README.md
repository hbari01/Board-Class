Board-Class
===========

Board –	An	interface	class	that	defines	operations	of	a	game	board	

public class Board {

	char [][] board = new char[3][3];

	public void initializeBoard() {
		for(int i = 0; i <3; i++) {
			for(int j = 0; j < 3; j++) {
				board[i][j] = ' ';
			}
		}
	}

	public void printBoard() {
		for (int i = 0; i < 3; i++) {
			for (int j = 0; j < 2; j++) {
				System.out.print(board[i][j] + "|");
			}
			System.out.println();
			if(i < 2) {
				System.out.println("-----");
			}
		}
	}
}
