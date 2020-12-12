# Coin-Flip
public class CoinFlipExperiment {
	
	static public int coinFlipExperiment () {
		int winnings;
		winnings = 0;
		
		for(int i = 0; i <100; i++) {
		double flip = Math.random();
		if (flip < 0.505)  { 
		System.out.println ("Heads");
		winnings++;
		} 
		else {
		System.out.println ("Tails"); 
		winnings--;
		} 
		}
		
		return winnings;
		
	}
	
	public static void main(String[] args) {
		
		int amount = coinFlipExperiment (); 
		System.out.println ("Win/loss amount: " + amount);
		
	}
}
