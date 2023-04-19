# MenuProject
## Synopsis
A simple ordering software project that displays the menu, takes the name of the order and prints the name and order.
## How it works
The menu is displayed with items and their IDs. The customer types in their name, and the ids of the order. After pressing enter, the order is printed to the console.
## Code Example
This is the main method:
```
	public static void main(String[] args) {
		
		drink[] coke = new drink[3];
		coke[0] = new drink('S', "Coke", 0.5, 11, "Small Coke");
		coke[1] = new drink('M', "Coke", 1.0, 12, "Medium Coke");
		coke[2] = new drink('L', "Coke", 1.5, 13, "Large Coke");
				
		burger[] sandwich = new burger[6];
		sandwich[0] = new burger(1, true, 21, "Single with cheese", 3.00);
		sandwich[1] = new burger(2, true, 22, "Double with cheese", 4.00);
		sandwich[2] = new burger(3, true, 23, "Triple with cheese", 5.00);
		sandwich[3] = new burger(1, false, 24, "Single without cheese", 2.50);
		sandwich[4] = new burger(2, false, 25, "Double without cheese", 3.50);
		sandwich[5] = new burger(3, false, 26, "Triple without cheese", 4.50);
		
		side[] fry = new side[6];
		fry[0] = new side('S', "Fry", 31, "Small Fry", 1.50);
		fry[1] = new side('M', "Fry", 32, "Medium Fry", 2.00);
		fry[2] = new side('L', "Fry", 33, "Large Fry", 3.00);
		fry[3] = new side('S', "Cheese Stick", 34, "Small Cheese Sticks", 2.50);
		fry[4] = new side('M', "Cheese Stick", 35, "Medium Cheese Sticks", 3.50);
		fry[5] = new side('L', "Cheese Stick", 36, "Large Cheese Sticks", 5.00);
		
		showMenu(coke, sandwich, fry);
		
		askOrder();
	}
```
